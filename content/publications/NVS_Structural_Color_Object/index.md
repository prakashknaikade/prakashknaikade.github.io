---
title: "Novel View Synthesis of Structural Color Objects Created by Laser Markings"
authors:
- admin
date: "2024-08-08T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: ""

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["thesis"]

# Publication name and optional abbreviated publication name.
publication: ""
publication_short: "(MASTER THESIS)"

# Summary. An optional shortened abstract.
summary: This work marks the beginning of novel view synthesis for structural color objects and opens up potential avenues for various future research directions and endeavors. Moreover, this thesis will act as a foundational guide for novice researchers interested in exploring the novel view synthesis of specular and shiny objects with high view-dependent colors, commonly referred to as Structural Colors and Pearlescent Colors.

tags:
- Novel View Synthesis
- Radiance Field Methods
- Gaussaian Splatting
- NeRF
- Structural Colors

featured: true

links:
- name: Demo (3D Web Viewer)
  url: https://prakashknaikade.github.io/StructColorPaintingViewer/
- name: PDF (HQ)
  url: https://www.dropbox.com/scl/fi/in79kjuyn2h8b2mmd847x/NVS_Structural_Color_Objects.pdf?rlkey=sdv7lxi3rymelltdv8u7sgl1d&st=25ixlxzf&dl=0
url_pdf: '/publications/nvs_structural_color_object/NVS_Structural_Color_Objects_compressed.pdf'
url_code: ''
url_dataset: 'https://www.dropbox.com/scl/fo/9btslfn5y71lb6ct4jy62/AJ-6C-8QmycAND85arMPBDQ?rlkey=tqq444p2k608el58aoq5tzbvf&e=1&st=qcq9xn97&dl=0'
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: '/taylor_simulation_2.mp4'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  filename: pipeline_gsplat.jpg
  placement: 1
  caption: ''
  focal_point: 'Smart'
  preview_only: true
  resampleFilter: 

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
show_date: true
reading_time: false
pager: false
show_breadcrumb: true
header:
  navbar:
    enable: true
---
### Abstract
<p style="font-size: 1.1rem;text-align: justify;">
Transforming physical object into its high quality 3D digital twin using novel view synthesis is crucial for researchers in the domain of automatic laser marking of any color image on different metal substrates. Current Radiance Field methods have significantly advanced novel view synthesis of scenes captured with multiple photos or videos. But, they struggle to represent the scene with shiny objects. Moreover, multi view reconstruction of reflective objects with structural colors is extremely challenging because specular reflections are view-dependent and thus violate the multiviewconsistency, which is the cornerstone for most multiview reconstruction methods. However, there is a general lack of synthetic datasets for objects with structural colors and a literature review on state-of-the-art (SOTA) novel view synthesis methods for this kind of materials. Addressing these issues, we introduce a novel synthetic dataset that is used to conduct quantitative and qualitative analysis on a SOTA novel view synthesis methods. We demonstrate different techniques to improve the scene representation of laser printed planar structural color objects, focusing on the 3D Gaussian Splatting (3D-GS) method, which performs exceptionally well on our synthetic dataset. Our techniques, such as using geometric prior of planar structural color objects while initializing scene with sparse structure-from-motion (SfM) point cloud and the Anisotropy Regularizer, significantly improves the visual quality of view synthesis. We design different capture setups to acquire images of objects and evaluate the visual quality of the scene with different capture setups. Additionally, we present comprehensive experimentation to demonstrate methods to simulate structural color objects using just captured images of laser-printed primaries. This comprehensive research aims to contribute to the advancement of novel view synthesis methods for scenes involving reflective objects with structural colors.
</p>

### TLDR
This work is the result of my master thesis on "Novel View Synthesis of Structural Color Objects Created by Laser Markings", in collaboration with [AIDAM](https://aidam.mpi-inf.mpg.de/?view=home), [Oraclase](https://www.oraclase.com/), [MPI-Inf](https://www.mpi-inf.mpg.de/home/), and [SIC](https://saarland-informatics-campus.de/en/).

{{% callout note %}}

<p style="font-size: 1.1rem;">
This work marks the beginning of Novel View Synthesis (NVS) of structural color objects and opens up potential avenues for various future research directions and endeavors. 
</p>
<p style="font-size: 1.1rem;">
<b>Beginners</b>: This thesis will help beginners grasp the brief history of radiance field methods and essential preliminaries, such as the mathematics, tools, and concepts necessary to understand NVS methods. Furthermore, it will serve as a foundational guide for novice researchers interested in exploring the novel view synthesis of specular and shiny objects with high view-dependent colors, commonly referred to as Structural Colors or Pearlescent Colors.
</p>

<p style="font-size: 1.1rem;">
<b>Advanced Researchers</b>: This thesis will also be a valuable reference for advanced researchers who may wish to revisit the fundamental concepts and access the <em>StructColorToaster scene</em> from new <em>Structural Color Blender Dataset</em>. Additionally, the thesis discusses approaches to improve results and outlines potential future research directions.
</p>

<p style="font-size: 1.1rem;">
<b>Technical Artists</b>: This thesis provides an overview of how the new Gaussian Splatting technology can be applied to various use cases and demonstrates the life cycle of a specific use case in interactive product visualization, from capturing the product to visualizing it in a web viewer. 
</p>
{{% /callout %}}

### Datasets
- Structural Color Blender Dataset (Synthetic Scenes)
  - *StructColorToaster* Scene: Access Blender source and dataset from 👉[here](https://www.dropbox.com/scl/fo/9btslfn5y71lb6ct4jy62/AJ-6C-8QmycAND85arMPBDQ?rlkey=tqq444p2k608el58aoq5tzbvf&e=1&st=qcq9xn97&dl=0)

- Real Scenes
  - *StructColorPainting* Scene
  - *StructColorPaintingOld* Scene
  - *StructColorPrimaries* Scene
  - *StructColorTaylorSwift* Scene

### Evaluation
#### Structural Color Blender Dataset (Synthetic Scenes)
- Evaluation of selected SOTA methods on <em>StructColorToaster</em> scene:

<figure style="width: 100%; max-width: 600px; margin: auto;">
  <table style="font-size: 0.9rem; padding: 2px; margin: auto; border-collapse: collapse;">
    <thead>
      <tr>
        <th style="padding: 2px;">Method</th>
        <th style="padding: 2px;">Iterations</th>
        <th style="padding: 2px;">PSNR &#8593;</th>
        <th style="padding: 2px;">SSIM &#8593;</th>
        <th style="padding: 2px;">LPIPS &#8595;</th>
        <th style="padding: 2px;">Train</th>
        <th style="padding: 2px;">FPS</th>
        <th style="padding: 2px;">Memory</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td style="padding: 2px;">NeRF</td>
        <td style="padding: 2px;">50K</td>
        <td style="padding: 2px;">23.359</td>
        <td style="padding: 2px;">0.8427</td>
        <td style="padding: 2px;">0.1895</td>
        <td style="padding: 2px;">1 day</td>
        <td style="padding: 2px;">0.001</td>
        <td style="padding: 2px;">22MB</td>
      </tr>
      <tr>
        <td style="padding: 2px;">InstantNGP</td>
        <td style="padding: 2px;">50K</td>
        <td style="padding: 2px;">19.659</td>
        <td style="padding: 2px;">0.8109</td>
        <td style="padding: 2px;">0.2068</td>
        <td style="padding: 2px;">23 min</td>
        <td style="padding: 2px;">6</td>
        <td style="padding: 2px;">159.2MB</td>
      </tr>
      <tr>
        <td style="padding: 2px;">Mip-NeRF</td>
        <td style="padding: 2px;">250K</td>
        <td style="padding: 2px;">22.818</td>
        <td style="padding: 2px;">0.877</td>
        <td style="padding: 2px;">0.1263</td>
        <td style="padding: 2px;">1 day</td>
        <td style="padding: 2px;">0.03</td>
        <td style="padding: 2px;">15.9MB</td>
      </tr>
      <tr>
        <td style="padding: 2px;">NeRFacto</td>
        <td style="padding: 2px;">50K</td>
        <td style="padding: 2px;">19.305</td>
        <td style="padding: 2px;">0.8056</td>
        <td style="padding: 2px;">0.2123</td>
        <td style="padding: 2px;">35 min</td>
        <td style="padding: 2px;">0.6</td>
        <td style="padding: 2px;">168MB</td>
      </tr>
      <tr>
        <td style="padding: 2px;">Ref-NeRF</td>
        <td style="padding: 2px;">250K</td>
        <td style="padding: 2px;">27.5194</td>
        <td style="padding: 2px;">0.9142</td>
        <td style="padding: 2px;">0.1286</td>
        <td style="padding: 2px;">2 days</td>
        <td style="padding: 2px;">0.3</td>
        <td style="padding: 2px;">8.2MB</td>
      </tr>
      <tr>
        <td style="padding: 2px; font-weight: bold;  background-color: yellow; color: #000;">3D-GS</td>
        <td style="padding: 2px;">30K</td>
        <td style="padding: 2px; font-weight: bold;  background-color: yellow; color: #000;">24.0435</td>
        <td style="padding: 2px;">0.9065</td>
        <td style="padding: 2px;">0.1061</td>
        <td style="padding: 2px;">20 min</td>
        <td style="padding: 2px;">140</td>
        <td style="padding: 2px;">77MB</td>
      </tr>
      <tr>
        <td style="padding: 2px;">3D-GS</td>
        <td style="padding: 2px;">60K</td>
        <td style="padding: 2px;">24.3117</td>
        <td style="padding: 2px;">0.9070</td>
        <td style="padding: 2px;">0.1052</td>
        <td style="padding: 2px;">30 min</td>
        <td style="padding: 2px;">140</td>
        <td style="padding: 2px;">77MB</td>
      </tr>
    </tbody>
  </table>
  <figcaption style="text-align: left; margin-top: 10px;">
    Table 1: Quantitative evaluation of selected methods' results computed over our <em>StructColorToaster</em> Scene. <br> (The values for the Train time and FPS are approximate.)
  </figcaption>
</figure>

- Renders of optimized <em>StructColorToaster</em> Scene using 3D-GS:
{{< figure src="/3DGS_Toaster.jpeg" caption="Figure 1: The renderings show that 3D-GS able to capture the crisp shininess appearance of the surface. However, it does improve in learning specular reflections with increasing iterations, it is still not up to the mark and suffures from  holes and aliasing effect aka popping artifacts." numbered="true">}}

#### Real Scenes
- Evalution of different choices on <em>StructColorPainting</em> and <em>StructColorPaintingOld</em> Scenes

<figure style="width: 100%; max-width: 600px; margin: auto;">
<table style="font-size: 0.9rem; padding: 2px; margin: auto; border-collapse: collapse;">
    <thead>
        <tr>
            <th style="padding: 2px;">Method</th>
            <th style="padding: 2px;">7K</th>
            <th style="padding: 2px;">30K</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td style="padding: 2px;">Vanilla 3D-GS</td>
            <td style="padding: 2px;">27.11</td>
            <td style="padding: 2px;">28.92</td>
        </tr>
        <tr>
            <td style="padding: 2px;">Cleaned-SfM</td>
            <td style="padding: 2px;">27.6715</td>
            <td style="padding: 2px;  font-weight: bold;  background-color: yellow; color: #000;">29.1789</td>
        </tr>
        <tr>
            <td style="padding: 2px;">With-Masks</td>
            <td style="padding: 2px;">9.352</td>
            <td style="padding: 2px;">9.4603</td>
        </tr>
        <tr>
            <td style="padding: 2px;">With-Cropped-Images/RGBA Images</td>
            <td style="padding: 2px;">29.1759</td>
            <td style="padding: 2px;">30.0007</td>
        </tr>
        <tr>
            <td style="padding: 2px;"> With-Cropped-Images/RGBA Images: <br> (No-Densification + No-Position Optimization)</td>
            <td style="padding: 2px;">24.4612</td>
            <td style="padding: 2px;">25.089</td>
        </tr>
        <tr>
            <td style="padding: 2px;">Densify Until Iteration = 30000</td>
            <td style="padding: 2px;">26.8325</td>
            <td style="padding: 2px;">29.4149</td>
        </tr>
        <tr>
            <td style="padding: 2px;">Densification Interval = 30</td>
            <td style="padding: 2px;">25.2634</td>
            <td style="padding: 2px;">28.6454</td>
        </tr>
        <tr>
            <td style="padding: 2px;">Densification Interval = 50</td>
            <td style="padding: 2px;">26.0189</td>
            <td style="padding: 2px;">28.2718</td>
        </tr>
        <tr>
            <td style="padding: 2px;">Reset Opacity = Every 1000 Iteration</td>
            <td style="padding: 2px;">27.7216</td>
            <td style="padding: 2px;">29.2581</td>
        </tr>
        <tr>
            <td style="padding: 2px;">Reset Opacity = Every 2000 Iteration</td>
            <td style="padding: 2px;">27.6354</td>
            <td style="padding: 2px;">29.1786</td>
        </tr>
        <tr>
            <td style="padding: 2px;">Reset Opacity = Every 5000 Iteration</td>
            <td style="padding: 2px;">27.82</td>
            <td style="padding: 2px;">29.2726</td>
        </tr>
        <tr>
            <td style="padding: 2px;">SH-Degree 0</td>
            <td style="padding: 2px;">26.4699</td>
            <td style="padding: 2px;">27.9771</td>
        </tr>
        <tr>
            <td style="padding: 2px;">White-Background</td>
            <td style="padding: 2px;">27.6579</td>
            <td style="padding: 2px;">29.2025</td>
        </tr>
        <tr>
            <td style="padding: 2px;">Random-Background</td>
            <td style="padding: 2px;">27.7607</td>
            <td style="padding: 2px;">29.3303</td>
        </tr>
        <tr>
            <td style="padding: 2px;">No-Densification</td>
            <td style="padding: 2px;">17.7919</td>
            <td style="padding: 2px;">18.3929</td>
        </tr>
        <tr>
            <td style="padding: 2px;">Reduced Number of Images = 297</td>
            <td style="padding: 2px;">27.3657</td>
            <td style="padding: 2px;">28.7223</td>
        </tr>
        <tr>
            <td style="padding: 2px;">Anisotropy-Regularizer</td>
            <td style="padding: 2px;">27.5747</td>
            <td style="padding: 2px; font-weight: bold;  background-color: yellow; color: #000;">29.4191</td>
        </tr>
    </tbody>
    
</table>
<figcaption style="text-align: left; margin-top: 10px;">Table 2: PSNR Score for ablation runs. Quantitative evaluation of results computed over our <em>StructColorPainting</em> scene using different 3D-GS settings. (The values for FPS are approximate.)</figcaption>
</figure>

- Evaluation of selected techniques’ results computed over our <em>StructColorPainting</em> scene:
<figure style="width: 100%; max-width: 600px; margin: auto;">
    <table style="font-size: 0.9rem; padding: 2px; margin: auto; border-collapse: collapse;">
        <thead>
            <tr style="border-bottom: 3px solid grey;">
                <th style="padding: 2px;">Method</th>
                <th style="padding: 2px;">Iterations</th>
                <th style="padding: 2px;">PSNR &#8593;</th>
                <th style="padding: 2px;">SSIM &#8593;</th>
                <th style="padding: 2px;">LPIPS &#8595;</th>
                <th style="padding: 2px;">Train</th>
                <th style="padding: 2px;">FPS</th>
                <th style="padding: 2px;">Memory</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td style="padding: 2px;">Cleaned-SfM</td>
                <td style="padding: 2px;">7K</td>
                <td style="padding: 2px;">27.6452</td>
                <td style="padding: 2px;">0.9221</td>
                <td style="padding: 2px;">0.1795</td>
                <td style="padding: 2px;">5.122min</td>
                <td style="padding: 2px;">150</td>
                <td style="padding: 2px;">79MB</td>
            </tr>
            <tr style="border-bottom: 3px solid grey;">
                <td></td>
                <td style="padding: 2px;">30K</td>
                <td style="padding: 2px; font-weight: bold; background-color: yellow; color: #000;">29.1789</td>
                <td style="padding: 2px;">0.9342</td>
                <td style="padding: 2px;">0.1602</td>
                <td style="padding: 2px;">27.69min</td>
                <td style="padding: 2px;">120</td>
                <td style="padding: 2px;">150MB</td>
            </tr>
            <tr>
                <td style="padding: 2px;">Anisotropy-Regularizer</td>
                <td style="padding: 2px;">7K</td>
                <td style="padding: 2px;">27.5476</td>
                <td style="padding: 2px;">0.9223</td>
                <td style="padding: 2px;">0.1780</td>
                <td style="padding: 2px;">5.134min</td>
                <td style="padding: 2px;">150</td>
                <td style="padding: 2px;">78.6MB</td>
            </tr>
            <tr style="border-bottom: 3px solid grey;">
                <td></td>
                <td style="padding: 2px;">30K</td>
                <td style="padding: 2px; font-weight: bold; background-color: yellow; color: #000;">29.9631</td>
                <td style="padding: 2px;">0.9346</td>
                <td style="padding: 2px; ">0.1572</td>
                <td style="padding: 2px;">26.35 min</td>
                <td style="padding: 2px;">120</td>
                <td style="padding: 2px;">152.4MB</td>
            </tr>
            <tr>
                <td style="padding: 2px;">Anisotropy-Regularizer:<br>297-Images</td>
                <td style="padding: 2px;">7K</td>
                <td style="padding: 2px;">26.9920</td>
                <td style="padding: 2px;">0.9238</td>
                <td style="padding: 2px;">0.1833</td>
                <td style="padding: 2px;">5.812 min</td>
                <td style="padding: 2px;">150</td>
                <td style="padding: 2px;">86.1MB</td>
            </tr>
            <tr style="border-bottom: 3px solid grey;">
                <td></td>
                <td style="padding: 2px;">30K</td>
                <td style="padding: 2px; font-weight: bold; background-color: yellow; color: #000;">29.3213</td>
                <td style="padding: 2px;">0.9339</td>
                <td style="padding: 2px;">0.1648</td>
                <td style="padding: 2px;">28.57min</td>
                <td style="padding: 2px;">120</td>
                <td style="padding: 2px;">176.2MB</td>
            </tr>
        </tbody>
    </table>
    <figcaption style="text-align: left; margin-top: 10px;">
            Table 3: Quantitative evaluation of selected techniques’ results computed over our <em>StructColorPainting</em> scene. (The values for FPS are approximate).
        </figcaption>
</figure>

-  Evaluation of renderings using our techniques’ and gsplat with cleaned SfM and additional features computed over <em>StructColorTaylorSwift</em> scene:
<figure style="width: 100%; max-width: 600px; margin: auto;">
    <table style="font-size: 0.9rem; padding: 2px; margin: auto; border-collapse: collapse;">
        <thead>
            <tr style="border-bottom: 3px solid grey;">
                <th style="padding: 2px;">Method</th>
                <th style="padding: 2px;">Iterations</th>
                <th style="padding: 2px;">PSNR &#8593;</th>
                <th style="padding: 2px;">SSIM &#8593;</th>
                <th style="padding: 2px;">LPIPS &#8595;</th>
                <th style="padding: 2px;">Train</th>
                <th style="padding: 2px;">FPS</th>
                <th style="padding: 2px;">Memory</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td style="padding: 2px;">Our Techniques</td>
                <td style="padding: 2px;">7K</td>
                <td style="padding: 2px;">30.2567</td>
                <td style="padding: 2px;">0.9338</td>
                <td style="padding: 2px;">0.1921</td>
                <td style="padding: 2px;">4.123min</td>
                <td style="padding: 2px;">150</td>
                <td style="padding: 2px;">55MB</td>
            </tr>
            <tr style="border-bottom: 3px solid grey;">
                <td></td>
                <td style="padding: 2px;">30K</td>
                <td style="padding: 2px; font-weight: bold; background-color: yellow; color: #000;">33.6547</td>
                <td style="padding: 2px;">0.9458</td>
                <td style="padding: 2px;">0.1749</td>
                <td style="padding: 2px;">18.5min</td>
                <td style="padding: 2px;">120</td>
                <td style="padding: 2px;">94MB</td>
            </tr>
            <tr>
                <td style="padding: 2px;">gsplat</td>
                <td style="padding: 2px;">7K</td>
                <td style="padding: 2px;">31.8051</td>
                <td style="padding: 2px;">0.9391</td>
                <td style="padding: 2px;">0.1880</td>
                <td style="padding: 2px;">2.86min</td>
                <td style="padding: 2px;">150</td>
                <td style="padding: 2px;">64MB</td>
            </tr>
            <tr style="border-bottom: 3px solid grey;">
                <td></td>
                <td style="padding: 2px;">30K</td>
                <td style="padding: 2px; font-weight: bold; background-color: yellow; color: #000;">34.6451</td>
                <td style="padding: 2px;">0.9511</td>
                <td style="padding: 2px;">0.1658</td>
                <td style="padding: 2px;">16.61min</td>
                <td style="padding: 2px;">120</td>
                <td style="padding: 2px;">119MB</td>
            </tr>
            <tr>
                <td style="padding: 2px;">gsplat + Mip-Splatting</td>
                <td style="padding: 2px;">7K</td>
                <td style="padding: 2px;">31.3528</td>
                <td style="padding: 2px;">0.9362</td>
                <td style="padding: 2px;">0.1922</td>
                <td style="padding: 2px;">2.54min</td>
                <td style="padding: 2px;">150</td>
                <td style="padding: 2px;">66MB</td>
            </tr>
            <tr style="border-bottom: 3px solid grey;">
                <td></td>
                <td style="padding: 2px;">30K</td>
                <td style="padding: 2px; font-weight: bold; background-color: yellow; color: #000;">34.6654</td>
                <td style="padding: 2px;">0.9379</td>
                <td style="padding: 2px;">0.1827</td>
                <td style="padding: 2px;">17.1min</td>
                <td style="padding: 2px;">120</td>
                <td style="padding: 2px;">124MB</td>
            </tr>
        </tbody>
    </table>
    <figcaption style="text-align: left; margin-top: 10px;">
        Table 4: Quantitative evaluation of selected techniques’ results computed over our <em>StructColorPainting</em> scene. (The values for FPS are approximate.)
    </figcaption>
</figure>


### Videos
#### Real Scenes
RGB renders of interactive visualization in SIBR viewer of an optimized real world sences with our techniques:

- *StructColorPainting* scene
{{< video src="/man_16_891_imgs.mp4" controls="yes" >}}

- *StructColorTaylorSwift* scene
{{< video src="/taylor_simulation_2.mp4" controls="yes" >}}


<br>

#### Synthesized Scenes Using Just Primaries
- Simulating Structural Color Object (Pseudo) before Laser Printing:

{{< figure src="/pipeline_gsplat.jpg" caption="Figure 2: Pipeline of Synthesizing Arbitrary Images of Structural Color Object for Arbitrary Viewing Directions." numbered="true">}}

- Comparison between real structural color object views and respective synthesized views using just primaries for respective view directions:
  - *StructColorTaylorSwift* scene
  {{< video src="/taylor_swift_synth_views_gsplat_compare_ 720p.mp4" controls="yes" >}}

  - RGB renders of interactive visualization in SIBR viewer of an optimized synthetic scene, generated using synthesized images created just with primaries:
  {{< video src="/taylor_synth_perspective_simulation.mp4" controls="yes" >}}

<br>

- Synthesizing views using only the earlier tracked primaries for respective view directions, before laser printing the structural color object:
  - Synthesized views using just primaries for respective view directions:
  {{< video src="/cat_synth_views.mp4" controls="yes" >}}

  - RGB renders of interactive visualization in SIBR viewer of an optimized synthetic scene, generated using synthesized images created just with primaries:
  {{< video src="/cat_synth_perspective_simulation.mp4" controls="yes" >}}

### 3D Web Viewer

[**StructColorPaintingViewer**](https://prakashknaikade.github.io/StructColorPaintingViewer/) is a webviwer to visulaize the structural color objects.
The webviewer is implemented with help of [gsplat.js](https://github.com/huggingface/gsplat.js) but it only supports scenes optimized with spherical harmonics (SH) of degree 0. However, scenes optimized with SH0 don't achieve the same quality as those optimized with SH3, which is evident from above videos of renderings of scenes optimized with SH3 in SIBR viewer.

<iframe src="https://prakashknaikade.github.io/StructColorPaintingViewer/"
        width="100%" height="600px"
        style="border: none;">
</iframe>

### BibTeX

### References

<p style="font-size: 1.1rem;">
1. [NeRF] Ben Mildenhall, Pratul P. Srinivasan, Matthew Tancik, Jonathan T. Barron, Ravi Ramamoorthi, and Ren Ng. Nerf: Representing scenes as neural radiance fields for view synthesis. ECCV, 2020.<br>  
2. [InstantNGP] Thomas Muller, Alex Evans, Christoph Schied, and Alexander Keller. Instant neural graphics primitives with a multiresolution hash encoding. ACM Trans.Graph., July 2022.<br> 
3. [Mip-NeRF] Jonathan T. Barron, Ben Mildenhall, Matthew Tancik, Peter Hedman, Ricardo Martin-Brualla, and Pratul P. Srinivasan. Mip-nerf: A multiscale representation for anti-aliasing neural radiance fields. ICCV, 2021.<br>
4. [NeRFacto] Matthew Tancik, Ethan Weber, Evonne Ng, Ruilong Li, Brent Yi, Justin Kerr, Terrance Wang, Alexander Kristoffersen, Jake Austin, Kamyar Salahi, Abhik Ahuja, David McAllister, and Angjoo Kanazawa. Nerfstudio: A modular framework for neural radiance field development. ACM SIGGRAPH 2023.<br>
5. [Ref-NeRF] Dor Verbin, Peter Hedman, Ben Mildenhall, Todd Zickler, Jonathan T. Barron, and Pratul P. Srinivasan. Ref-NeRF: Structured view-dependent appearance for neural radiance fields. CVPR, 2022.<br> 
6. [3D-GS] Bernhard Kerbl, Georgios Kopanas, Thomas Leimkuehler, and George Drettakis. 3d gaussian splatting for real-time radiance field rendering. ACM Transactions on Graphics, July 2023.
</p> 
