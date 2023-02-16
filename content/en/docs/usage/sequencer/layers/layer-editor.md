---
title: Layer Editor
author: Vixen Team
weight: 20
description: This section covers the Layer Editor.
---

### Overview

Layers are a method of controlling how seperate Effects on the same element interact with each other. It can be very powerful to create variations on the existing effects. The Layer Editor is the docking window in the Sequencer that controls how the layers are confgured. The layer editor is a docking window like most of the other editor type windows. It can be positioned in any fashion typical of a docking style window. If it is not visible it can be enabled under the View menu in the sequence editor. The menu name is **Layer Editor Window**.

Layers are stacked in the editor by their order of precedence. Layers on top will be processed first, working down to the default layer at the bottom. The Default layer is fixed and will always be at the bottom. No mixing occurs in this layer.

### Editor

Buttons at the top of the editor allow new layers to be added, or selected layers to be deleted. If any effects are associated with a layer when it is deleted, all those effects will be automatically moved to the default layer.

Layers can be reordered by dragging them in the list to the position you want them to be in. In order to drag the layer, you need click in the blue area surrounding the Layer expander. It will highlight in blue as you hover over it.

Expanding the layer provides a way to name the layer as desired as well as change its configration if it has options. The drop down box allows you to choose the type of mixer used to combine color between this layer and the layer below it. If the type of mixer has confguration options, there will be a Configuration button once it is expanded. Clicking on that will bring up the configration dialog for that type.

As you work on your sequence, you may find that you need multiple sets of layers in different orders to accomplish what you need. Keep in mind that layers and their order are applied across the entire sequence.
