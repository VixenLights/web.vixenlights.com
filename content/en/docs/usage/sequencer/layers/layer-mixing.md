---
title: Layer Mixing
author: Vixen Team
weight: 20
description: This section covers examples of using Layers.
---
### Intensity Overlay

![Effect Fade Layering](/images/docs/usage/sequencer/layers/layer-mixing/EffectFadeLayerFullColor.png)

Layers can be used to dim effects that do not currently have a level curve over the entire effect by using the Intensity Overlay mixer in a defined layer. As shown below the white pulse is in the Intensity Overlay layer and the Alternating is in the Default layer. The alternating effect will fade out in relation to the ramp on the pulse effect. The color of the pulse is not important on full color elements.

![Effect Fade Layering](/images/docs/usage/sequencer/layers/layer-mixing/EffectFadeLayer.png)

On discrete items that have color defined, the same principle applies with a bit of a spin. Here I am placing this on some led string lights with defined color. There are multiple strings of Red, Green, and Blue. Here I am alternating from red to green. I have added a red pulse to the intensity overlay layer. Here the red lights will dim as they match the red of the pulse. The green will stay at full intensity.

![Effect Fade Layering Discrete](/images/docs/usage/sequencer/layers/layer-mixing/EffectFadeLayerMultiDiscrete.png)

To dim both colors I add green to the pulse.

### Mask

![Spiral Butterfly Preview](/images/docs/usage/sequencer/layers/layer-mixing/SpiralButterflyPreview.png)

![Spiral Butterfly Effect](/images/docs/usage/sequencer/layers/layer-mixing/SpiralButterflyEffect.png)

The Mask mixing method allows you to mask out areas of an effect with another effect. You can accomplish this in a similar manner as depicted above. Areas that are lit in the layer that has a the Mask mixer will turn off areas in the effect in the layer beneath it. One example of this is a spiraling butterfly effect. By placing a Spiral effect in the Mask layer and a Butterfly effect in the default layer, the lit spirals in the Spiral effect will create spiral cut outs in the Butterfly. This gives the effect of Spirals where the spokes have the Butterfly pattern on them. The colors of the spirals themselves are irrelevant for using it as a mask. You really only need one color and you configure the spirals to the look you want. The example below was created by just dropping the two effects with defaults, mining them up and setting the spiral to the layer that has a Mask mixer setup.

### Mask and Fill

Mask and fill is very similar to the Mask mixing, except instead of leaving unlit areas where the masking effect is, it will replace those areas with the effect in the Mask and Fill layer. In the spiral example above, the colored spirals in the Spiral effect will be visible and replace those areas of the Butterfly. Thus you end up with a spiral overlaid on the Butterfly. Without layering, these would mix and give mixed results. Here you get the exact colors of the Spiral on top of the Butterfly effect so in this case the colors are relevant and you can configure them as needed to obtain the effect you want. Here is how this looks in the preview. I used one color of blue and I reduced the thickness of the spiral by about half to get this look.

![Spiral Fill Butterfly Effect](/images/docs/usage/sequencer/layers/layer-mixing/SpiralFillButterflyPreview.png)

### Conclusion

These are just simple examples of the power of layers. There are other mixers that allow for combining in many different ways. Layers are also cumulative, so you can mix multiple effects in higher layers to affect lower layers. We will be adding more in the future as need arise.

### Tutorials

[Videos]({{< ref layer-videos>}})
