---

title: Laser Speckle Contrast Imaging
summary: We develop blood flow imaging systems based on laser speckle contrast imaging (LSCI) to study the effects of ischemic stroke and to better understand the physics of dynamic light scattering.

tags:
- LSCI
- MESI

weight: 1

image:  
  caption: "Speckle contrast image of cortical blood flow ([Sullender, 2022](/publication/sullender-2022-1/))"
  
  # Placement options: 1 = Full column width, 2 = Out-set, 3 = Screen-width
  placement: 1
    
  # Focal point options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point: Center

  # Set `preview_only` to `true` to just use the image for thumbnails
  preview_only: false

aliases:
  - /research/laser-speckle-contrast-imaging

---

There has been increasing interest in using laser speckle contrast imaging (LSCI) as a tool for imaging blood flow in preclinical research and clinical applications. LSCI utilizes intrinsic tissue contrast from dynamic light scattering to offer a relatively simple technique for visualizing detailed spatiotemporal dynamics of blood flow changes in real-time.

Laser speckle is the random interference pattern produced when coherent light scatters from a medium that can be imaged onto a detector such as a camera. Motion from scattering particles, such as red blood cells in the vasculature, leads to spatial and temporal variations in the speckle pattern. Speckle contrast analysis quantifies the local spatial variance ($K$), or blurring, of the speckle pattern that results from blood flow.

\begin{equation}
    K = \frac{\sigma_{s}}{\langle{I}\rangle}
\end{equation}

 Areas with greater motion have more rapid intensity fluctuations and therefore more blurring of the speckle pattern during the camera exposure ([Fig. 1](#figure-raw-sc)). LSCI can be used to quantify relative changes in blood flow, and has been studied both in animal models and in the clinic.

{{< figure src="raw-sc.png" caption="Objective speckle pattern (left) and resulting laser speckle contrast image (right). The region with higher flow (red) has lower contrast than the region with low flow (blue)." numbered="true" id="raw-sc" >}}

In our lab, we focus on functional brain imaging and use LSCI to study cerebral blood flow (CBF) dynamics. CBF is an important hemodynamic parameter in the brain that can be used to study neurological events such as stroke, cortical spreading depression, and functional activation. We use LSCI in animal models as a tool to better understand the neurophysiological mechanisms behind these events. [In the clinic]({{< relref "/project/clinical-speckle-imaging" >}}), LSCI is being leveraged as a non-invasive monitoring tool for neurosurgery that could help reduce the risk of postoperative blood flow deficits.

{{< figure src="webcam.jpg" caption="**Using a webcam to perform LSCI:** Post-stroke blood flow deficit imaged using an inexpensive LSCI system comprised of a webcam, plastic aspheric lenses, and a laser pointer. This image shows baseline speckle contrast imagery overlaid with the percent reduction in blood flow following a stroke in a mouse. ([Richards, 2013](/publication/richards-2013/))." width="50%" >}}

{{< figure src="PID.gif" caption="**Peri-Infarct Depolarizations:** Spreading depolarizations cause significant alterations in cerebral blood flow following photothrombotic stroke ([Sullender, 2018](/publication/sullender-2018/))." >}}

#### Resources

* [MATLAB code for calculating speckle contrast](https://github.com/shiruken/speckle)