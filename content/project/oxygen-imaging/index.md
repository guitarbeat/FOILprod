---

title: Oxygen Imaging
summary: We developed imaging systems for use with oxygen-sensitive phosphorescent dyes in order to map cortical oxygen tension (pO2) and study its impact on the progression of ischemic stroke.

tags:
- Oxygen
- Multiphoton Microscopy
- 2P
- Phosphorescence
- Lifetime

weight: 7

image:  
  caption: "Vascular oxygen tension map ([Sullender, 2018](/publication/sullender-2018/))"

  # Placement options: 1 = Full column width, 2 = Out-set, 3 = Screen-width
  placement: 1

  # Focal point options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point: Center

  # Set `preview_only` to `true` to just use the image for thumbnails
  preview_only: false

aliases:
  - /research/oxygen-tension-imaging

---

We use oxygen-sensitive porphyrin probes for noninvasive, highly-sensitive optical oxygenation measurements based on phosphorescence quenching. While an injection of the dye is required, absolute oxygen tension ($p_{\ce{O2}}$) can be directly calculated from the
lifetime ($\tau$) of the measured phosphorescence using the Stern-Volmer relationship:

\begin{equation}
  \frac{I_0}{I} = 1 + k_q\tau_0[Q]
\end{equation}

In order to localize the phosphorescent signal, we use either [two-photon excitation]({{< relref "/project/multiphoton-microscopy" >}}) or structured illumination with a digital micromirror device (DMD). The latter is combined with [laser speckle contrast imaging]({{< relref "/project/laser-speckle-contrast-imaging" >}}) for multimodal imaging of cortical hemodynamics (cerebral blood flow + $p_{\ce{O2}}$). These systems are used to study both the acute and chronic dynamics of ischemic stroke.

{{< figure src="pO2_roi.png" caption="**Multimodal Hemodynamic Imaging:** Blood flow and oxygen tension imaged simultaneously during and after photothrombotic stroke. An arteriole (A1/red) was occluded using DMD-targeted photothrombosis to induce ischemic stroke. ([Sullender, 2018](/publication/sullender-2018/))." >}}

{{< figure src="2P_pO2.png" caption="**3D Mapping of Oxygen Tension:** Two-photon phosphorescence lifetime imaging is used to characterize the oxygen tension in individual cortical vessels. As arterioles descend deeper into the brain, the oxygen tension rapidly decreases. ([Kazmi, 2013](/publication/kazmi-2013-2/))." >}}
