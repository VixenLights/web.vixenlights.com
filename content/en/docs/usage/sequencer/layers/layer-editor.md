---
title: Layer Editor
author: Vixen Team
weight: 20
description: This section covers the Layer Editor.
---

## Overview

Layers are a method of controlling how separate Effects on the same element interact with each other. It can be very powerful to create variations on the existing effects. The Layer Editor is the docking window in the Sequencer that controls how the layers are configured. The layer editor is a docking window like most of the other editor type windows. It can be positioned in any fashion typical of a docking style window. If it is not visible it can be enabled under the View menu in the sequence editor. The menu name is **Layer Editor Window**.

Layers are stacked in the editor by their order of precedence. Layers on top will be processed first, working down to the default layer at the bottom. The Default layer is fixed and will always be at the bottom. No mixing occurs in this layer.

### Editor

At the very top of the editor are two buttons for importing and exporting layers:

- **Import Layers** — loads a previously exported `.v3l` layer file and adds its layers to the current sequence.
- **Export Layers** — saves all non-default layers in the current sequence to a `.v3l` file. This button is disabled when only the default layer exists.

Below the import/export buttons, the **Add Layer** and **Remove Layer** buttons allow new layers to be created or selected layers to be deleted. If any effects are associated with a layer when it is deleted, all those effects will be automatically moved to the default layer.

Layers can be reordered by dragging them in the list to the position you want them to be in. In order to drag the layer, you need to click in the blue area surrounding the Layer expander. It will highlight in blue as you hover over it.

![Layer Editor Overview](/images/docs/usage/sequencer/layers/layer-editor/LayerEditorOverview.png)

Expanding the layer provides a way to name the layer as desired as well as change its configuration if it has options. The drop down box allows you to choose the type of mixer used to combine color between this layer and the layer below it. If the type of mixer has configuration options, there will be a Configuration button once it is expanded. Clicking on that will bring up the configuration dialog for that type.

Next to the layer name text box there is a **Quick Rename** button. Clicking it renames the layer to the display name of its currently selected mixing filter type. For example, if the layer uses a filter named `Mask and Fill`, clicking Quick Rename sets the layer name to `Mask and Fill`. If another layer already uses that name, a numeric suffix is automatically appended (`Name - 2`, `Name - 3`, and so on).

![Layer Editor Expanded Row](/images/docs/usage/sequencer/layers/layer-editor/LayerEditorExpanded.png)

As you work on your sequence, you may find that you need multiple sets of layers in different orders to accomplish what you need. Keep in mind that layers and their order are applied across the entire sequence.

### Exporting Layers

Clicking **Export Layers** opens a save-file dialog. The default file extension is `.v3l` (Vixen 3 Layers). All non-default layers are saved to the chosen file as human-readable JSON, preserving each layer's name, order, mixing filter type, and mixing filter configuration. The default layer is never included in the export.

The Export Layers button is disabled when the sequence has no non-default layers, so an empty layer file cannot be created through the normal workflow.

### Importing Layers

Clicking **Import Layers** opens an open-file dialog filtered to `.v3l` files. After you choose a file, Vixen validates its contents and adds any valid layers to the current sequence above the existing layers, in the same relative order they had when exported. For example, if the sequence already has `Layer A` and `Layer B`, and the imported file contains `Imported 1` and `Imported 2`, the resulting order will be `Imported 1`, `Imported 2`, `Layer A`, `Layer B`, `Default`.

If an imported layer name already exists in the current sequence, the imported layer is automatically renamed using a numeric suffix (`Name - 2`, `Name - 3`, and so on).

If any layers in the file reference a mixing filter that is not installed, Vixen displays a warning dialog summarizing how many layers will be imported and how many will be skipped. You can choose to proceed (importing only the valid layers) or cancel (importing nothing). If all layers are valid, import proceeds immediately without a confirmation dialog. If all layers are invalid, Vixen shows an error and nothing is imported.

---

*Import Layers, Export Layers, and Quick Rename were added in build 1442.*
