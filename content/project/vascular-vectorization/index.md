---

title: Vascular Vectorization
summary: We developed an automated vectorization method to extract blood vessel geometry and vascular statistics directly from large volumes of unsegmented multiphoton microscopy imagery.

tags:
- Vectorization
- Multiphoton Microscopy
- Computational Modeling

weight: 5

image:  
  caption: "3D rendering of vectorized geometry"
  
  # Placement options: 1 = Full column width, 2 = Out-set, 3 = Screen-width
  placement: 1
    
  # Focal point options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point: Center

  # Set `preview_only` to `true` to just use the image for thumbnails
  preview_only: false

---

Remarkably little is known about the plasticity of microvasculature in the adult brain because of the barriers to acquisition and processing of *in vivo* images. However, this basic concept is central to the field of neuroscience, and its investigation would provide insights to neurovascular conditions such as Alzheimer's, diabetes, and stroke. We are developing the pipeline to image, map, and monitor the capillary blood vessels over several weeks to months in healthy mouse brains. One of the major challenges in this workflow is the process of extracting complex capillary networks from [raw volumetric microscope images]({{< relref "/project/multiphoton-microscopy" >}}). This challenge is exacerbated by *in vivo* imaging constraints such as low resolutions, poor image quality, and contrast agents that highlight different features (e.g. plasma or endothelial labels). To confront these issues, we developed a general-purpose software method, [Segmentation-Less, Automated, Vascular Vectorization (SLAVV)]({{< relref "/publication/mihelic-2021" >}}), to extract vascular network maps from low quality images, enabling researchers to better quantify the vascular anatomy portrayed in their datasets.

{{< figure src="statistics.png" caption="**Microvasculature statistics:** Three-dimensional rendering of vectorized geometry and resulting depth-resolved anatomical statistics calculated from strand objects ([Mihelic, 2015](/publication/mihelic-2021))." >}}

#### Resources

* [SLAVV Software](https://github.com/UTFOIL/Vectorization-Public)