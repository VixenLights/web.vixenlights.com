---
title: Web API
author: Vixen Team
description: This section covers the RESTful API interfaces.
---

### Overview

Vixen implements a Restful Web API. The API allows you to get get element info, search for elements, start/pause/stop a sequence, stop a running sequence and get status updates of running sequences.

You can send commands and receive responses from the Vixen web server using the API below. The key thing to learn with this API is that most of it uses JSON object data. So if a request is POSTing data to the server that data will be in JSON object notation and sent in the body of the request. All responses are in JSON.

The Postman application is a good tool to use to learn how the API works and fully supports sending RESTful requests with JSON notation.  

### GET /api/element/getElements

Retrieves a list of elements in the display.

_Example request:_

<http://localhost:8080/api/element/getElements>

_Example Response:_

```json
[
  {
    "Id": "6173c7f3-46ee-424a-8e35-54eeadb98439",  
    "Name": "Poles",  
    "Colors": ["#FFA000"],  
    "Children": [{  
    "Id": "ff48009b-b051-4584-a654-4b7ed1599080",  
    "Name": "Pole 1",  
    "Colors": ["#FFA000"],  
    "Children": null  
  }, 
  {  
    "Id": "9fb69ece-1048-48b3-b55d-067eebcd9ad3",  
    "Name": "Pole 2",  
    "Colors": ["#FFA000"],  
    "Children": null  
  }, 
  {  
    "Id": "bf00aaaa-1dc8-4e3b-a21e-2bd57fdaff44",  
    "Name": "Pole 3",  
    "Colors": ["#FFA000"],  
    "Children": null  
  }  
]  
```

### GET /api/element/searchElements

Searches for elements that start with the with prefix.

_Example Request:_ Searches for elements starting with "Po".

<http://localhost:8080/api/element/searchElements?q=Po>

Response is the same as getElements.

### GET /api/element/on

Allows you to turn on a specified element.

_Example Request:_  

<http://localhost:8080/api/element/on>

Parms:

_id:_ The guid id of the element

_duration:_ The time in seconds to stay on. 0 is indefinite._

_intensity:_ 0-100 value for brightness

_color:_ The hex code of the color. Blue=#0000FF

_Example Response:  

```json
{
  "Message":"Window Left turned on for 30 seconds at 100% intensity."
}
```

### GET /api/element/off

Allows you to turn off a specified element.

_Example Request:_  

<http://localhost:8080/api/element/off>

Parms:

_id:_ The guid id of the element

_Example Response:_

```json
{"Message":"Window Left turned off."}  
```

### POST /api/element/groupon

Since build #357

Turns on a group of elements. Like the on function, but for a collection of elements.

_Example Request:_

<http://localhost:8080/api/element/groupon>

Request JSON object format:

```json
[  
 {"id":"e80accf6-a2b0-4b26-95d6-358210ce6580","duration":"30","intensity":"100","color":"#ffff00"},  
 {"id":"6d458dbb-12b1-4463-8ae7-a87718d6c412","duration":"0","intensity":"50","color":"#ff0000"}  
]
```

_Example Response:_

```json
{ 
  "Message": "2 elements turned on.", 
  "Details": [ "Mega Tree Star turned on for 30 seconds at 100% intensity.", "Mega Tree turned on at 50% intensity." ] 
}
```

### POST /api/element/clearall

Since build #357

Turns off all active effects in the web server live context. Will not affect playing sequences.

_Example Request:_

<http://localhost:8080/api/element/clearall>

* * *

### GET /api/play/getSequences

Retrieves a list of sequence files in the Vixen 3\Sequence folder. If you are using profiles, the folder returned will be the Sequence folder in the profile folder.

_Example Request:_

<http://localhost:8080/api/play/getSequences>

_Example Response:_

```json
[
  {"Name":"Basic Patterns 1", "FileName":"Basic Patterns 1.tim"},
  {"Name":"Border Pixel Test", "FileName":"Border Pixel Test.tim"}
]
```

### POST /api/play/playSequence

Plays the sequence passed.

_Example Request:_

<http://localhost:8080/api/play/playSequence>

_Example Response:_

```json
{
  "Name":"Announcement",
  "FileName": "C:\\Users\\bob\\Documents\\Vixen 3 &#8211; Halloween\\Sequence\\Announcement.tim"
}
```

Parms: JSON Object

_Name:_ The name of the sequence.

_FileName:_ The filename of the sequence.

Both are obtained from the getSequences call.

_Example Response:_

```json
{
  "State":1,
  "Sequence":{"Name":"Announcement","FileName":"Announcement.tim"},
  "Position":"00:00:00","Message":"Playing sequence Announcement of length 00:00:12.0680000"
}
```

### POST /api/play/stopSequence

Stops the specified sequence that was started within the web API. Uses the same format as the playSequence for the request data.
  
Parms: JSON Object

_Name:_ The name of the sequence.

_FileName:_ The filename of the sequence.

Both are obtained from the getSequences call.
  
_Example Response:_

```json
{
  "State":0,
  "Sequence":{"Name":"Bedroom Gable Chases","FileName":"Bedroom Gable Chases.tim"},
  "Position":"00:00:00","Message":"Sequence Bedroom Gable Chases stopped."
}
```

### POST /api/play/pauseSequence

Stops the specified sequence that was started within the web API. Uses the same format as the playSequence for the request data.

Parms: JSON object

_Name:_ The name of the sequence.

_FileName:_ The filename of the sequence.

Both are obtained from the getSequences call.

_Example Response:_

```json
{
  "State":0,
  "Sequence":{"Name":"","FileName":""},
  "Position":"00:00:00",
  "Message":"Sequence Bedroom Gable Chases paused."
}
```

### GET /api/play/status

Provides a status on what is currently playing.

Parms: none

Response:  
State: 0 is stopped, 1 is playing, 2 is paused.  
Position is the time offset into the current sequence.

```json
{  
  "State": 1,  
  "Sequence": {"Name": "Christmas Eve Sarajevo", "FileName": "Christmas Eve Sarajevo.tim"},  
  "Position": "00:02:14.0460000",  
  "Message": null  
}
```

### GET /api/system/getControllers

Since Version 3.6

Provides a list of the output controllers defined in the system.

Parms: none

_Example Response:_  

```json
[  
  {  
    "Id": "971b0b2d-0496-4894-8ecf-744e6f9b671e",  
    "Name": "House",  
    "IsRunning": true,  
    "IsPaused": false  
  },  
  {  
    "Id": "00d0402e-c993-49b1-914a-ab2234f26705",  
    "Name": "Renard Bushes",  
    "IsRunning": false,  
    "IsPaused": false  
  }  
]
```

### GET /api/system/getController?id=guid

Since Version 3.6

Get the info for specific controller by id.

Parms: controller id as guid

_Example Response:_

```json
{  
  "Id": "971b0b2d-0496-4894-8ecf-744e6f9b671e",  
  "Name": "House",  
  "IsRunning": true,  
  "IsPaused": false  
}
```

### POST /api/system/setControllerState

Since Version 3.6

Set the state of a specific controller.

_Parms:_ JSON object

```json
{  
  "id":"971b0b2d-0496-4894-8ecf-744e6f9b671e",  
  "isRunning":"True"  
}
```

_Example Response:_

```json
{  
  "Message": "House state Not Changed.",  
  "Details": [],  
  "IsSuccessful": false  
}
```

### POST /api/system/setAllControllerState

Since Version 3.6

Set the state of all the controllers.

_Parms:_ JSON object

```json
{  
  "id":"",  
  "isRunning":"True"  
}
```

_Example Response:_

```json
{  
  "Message": "All controllers state Changed.",  
  "Details": [],  
  "IsSuccessful": true  
}
```

**POST /api/system/save

Since Version 3.6

Save the System Config.

_Parms:_ None

_Example Response:_

```json
{  
  "Message": "Save Successful",  
  "Details": [],  
  "IsSuccessful": true  
}
```

### Status updates via SignalR messaging

Status updates are published via a SignalR push mechanism. You can include the SignalR client and subscribe to receive these updates.

```js
self.initSysytemStatusHub = function () {

//register for updates  
$.connection.ContextStates.client.updatePlayingContextStates = function(states){

//Do stuff with states object

}

// Start the connection  
$.connection.hub.start();  
}

```