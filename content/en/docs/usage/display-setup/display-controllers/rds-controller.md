---
title: RDS
author: Vixen Team

---

## Description

The RDS Controller is used for triggering RDS (Radio Data System) data over a serial port to one of the supported chipsets. It also can be used to trigger some data to be posted to a url as a query parameter. That could be an RDS controller that supports web requests, or any other endpoint that may or may not be an RDS controller. It is used in combination with the [RDS Effect][1] that passes the text through to this controller at a specified time.

## Setup

There is minimal setup for this controller if your RDS device has one of the supported chipsets. Just add it to your controller list with one output and ensure it is enabled. Using the gear icon, open the setup screen and select the proper chipset for your RDS controller. The supported chipsets are MRDS192, MRDS1322, or V-FMT212R. The later being the once popular VAST transmitter. For the MRDS based controllers, select your COM port in the drop down box. There are options for bidirectional and slow which may help with certain serial port setups.

If you are using it for an HTTP controller, or some alternative device that accepts HTTP requests, select that option. You will enter the url in the URL text box. The text paramter from the effect will be used as a query string where you place the {text} macro. The following example calls an endpoint on localhost port 8080 with two query string parameters. The update_rt value will be set to the text from the RDS effect.That specific URL is typical of the VAST device, so if you are using something else, you will need to adjust how the url is configured to match your device.

`http://127.0.0.1:8080/?action=update_rt&update_rt={text}`

The following shows an example of an HTTP setup without authentication.

![RDS HTTP Setup](/images/docs/usage/controller-setup/rds/rds-setup.png)

For the VAST V-FMT212R you need to ensure the VAST Control System software is running and has the Remote HTTP Access enabled. Full configuration is shown below. Note the areas highlighted with red. The Vixen web server defaults to using port 8080, so it is recommended to change the VAST port to 8081 as noted in the image.

![VAST RDS Setup](/images/docs/usage/controller-setup/rds/vast-rds-setup.png)

## Testing

You can enter text in the Test Interface section to simulate the macro value being set to some value. This should trigger the integration.

## Patching

A single Element is normally directly patched to this controller. There should be no color breakdown or dimming handlers in the path. It should resemble the following. This example shows the Launcher controller, but the RDS controller will look the same.

![RDS Display Setup](/images/docs/usage/controller-setup/launcher/launcher-setup.png)

## Testing

On the controller setup page at the bottom is a text text box. Entering some text there and hitting send will simulate what will occur if an effect passed the same text value. Your test text will be sent out as it is configured in order to validate your configuration works.

[1]: {{< ref "docs/usage/sequencer/effects/device-action/rds">}} "RDS Effect"
