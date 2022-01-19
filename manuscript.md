---
title: Deep-learning based automatic segmentation of vesicles in cryo-electron tomograms
keywords:
- synapse
- cryo-electron tomography
- synaptic vesicles
- deep learning
- segmentation
- post-processing
- automation
lang: en-US
date-meta: '2022-01-19'
author-meta:
- Amin Khosrozadeh
- Raphaela Seeger
- Julika Radecke
- Guillaume Witz
- Jakob B. Sørensen
- Benoît Zuber
header-includes: |-
  <!--
  Manubot generated metadata rendered from header-includes-template.html.
  Suggest improvements at https://github.com/manubot/manubot/blob/main/manubot/process/header-includes-template.html
  -->
  <meta name="dc.format" content="text/html" />
  <meta name="dc.title" content="Deep-learning based automatic segmentation of vesicles in cryo-electron tomograms" />
  <meta name="citation_title" content="Deep-learning based automatic segmentation of vesicles in cryo-electron tomograms" />
  <meta property="og:title" content="Deep-learning based automatic segmentation of vesicles in cryo-electron tomograms" />
  <meta property="twitter:title" content="Deep-learning based automatic segmentation of vesicles in cryo-electron tomograms" />
  <meta name="dc.date" content="2022-01-19" />
  <meta name="citation_publication_date" content="2022-01-19" />
  <meta name="dc.language" content="en-US" />
  <meta name="citation_language" content="en-US" />
  <meta name="dc.relation.ispartof" content="Manubot" />
  <meta name="dc.publisher" content="Manubot" />
  <meta name="citation_journal_title" content="Manubot" />
  <meta name="citation_technical_report_institution" content="Manubot" />
  <meta name="citation_author" content="Amin Khosrozadeh" />
  <meta name="citation_author_institution" content="Institute of Anatomy, University of Bern, Bern, Switzerland" />
  <meta name="citation_author_institution" content="Graduate School for Cellular and Biomedical Sciences, University of Bern" />
  <meta name="citation_author_orcid" content="XXXX-XXXX-XXXX-XXXX" />
  <meta name="citation_author" content="Raphaela Seeger" />
  <meta name="citation_author_institution" content="Institute of Anatomy, University of Bern, Bern, Switzerland" />
  <meta name="citation_author_institution" content="Graduate School for Cellular and Biomedical Sciences, University of Bern" />
  <meta name="citation_author_orcid" content="XXXX-XXXX-XXXX-XXXX" />
  <meta name="citation_author" content="Julika Radecke" />
  <meta name="citation_author_institution" content="Institute of Anatomy, University of Bern, Bern, Switzerland" />
  <meta name="citation_author_institution" content="Department of Neuroscience, Faculty of Health and Medical Science , 2200 Copenhagen N, University of Copenhagen, Copenhagen, Denmark" />
  <meta name="citation_author_institution" content="Diamond Light Source Ltd, Didcot, Oxfordshire, United Kingdom" />
  <meta name="citation_author_orcid" content="0000-0002-5815-5537" />
  <meta name="citation_author" content="Guillaume Witz" />
  <meta name="citation_author_institution" content="Science IT Service, University of Bern, Bern, Switzerland" />
  <meta name="citation_author_institution" content="Microscopy Imaging Center, University of Bern, Bern, Switzerland" />
  <meta name="citation_author_orcid" content="0000-0003-1562-4265" />
  <meta name="citation_author" content="Jakob B. Sørensen" />
  <meta name="citation_author_institution" content="Department of Neuroscience, University of Copenhagen, Blegdamsvej 3B, 2200 Copenhagen N, Denmark" />
  <meta name="citation_author_orcid" content="0000-0001-5465-3769" />
  <meta name="citation_author" content="Benoît Zuber" />
  <meta name="citation_author_institution" content="Institute of Anatomy, University of Bern, Bern, Switzerland" />
  <meta name="citation_author_orcid" content="0000-0001-7725-5579" />
  <link rel="canonical" href="https://elatella.github.io/deep-prepyto-paper/" />
  <meta property="og:url" content="https://elatella.github.io/deep-prepyto-paper/" />
  <meta property="twitter:url" content="https://elatella.github.io/deep-prepyto-paper/" />
  <meta name="citation_fulltext_html_url" content="https://elatella.github.io/deep-prepyto-paper/" />
  <meta name="citation_pdf_url" content="https://elatella.github.io/deep-prepyto-paper/manuscript.pdf" />
  <link rel="alternate" type="application/pdf" href="https://elatella.github.io/deep-prepyto-paper/manuscript.pdf" />
  <link rel="alternate" type="text/html" href="https://elatella.github.io/deep-prepyto-paper/v/6d26ebf8fbeb7d1d2b309cd8921bc2880c3a600c/" />
  <meta name="manubot_html_url_versioned" content="https://elatella.github.io/deep-prepyto-paper/v/6d26ebf8fbeb7d1d2b309cd8921bc2880c3a600c/" />
  <meta name="manubot_pdf_url_versioned" content="https://elatella.github.io/deep-prepyto-paper/v/6d26ebf8fbeb7d1d2b309cd8921bc2880c3a600c/manuscript.pdf" />
  <meta property="og:type" content="article" />
  <meta property="twitter:card" content="summary_large_image" />
  <link rel="icon" type="image/png" sizes="192x192" href="https://manubot.org/favicon-192x192.png" />
  <link rel="mask-icon" href="https://manubot.org/safari-pinned-tab.svg" color="#ad1457" />
  <meta name="theme-color" content="#ad1457" />
  <!-- end Manubot generated metadata -->
bibliography:
- content/manual-references.json
manubot-output-bibliography: output/references.json
manubot-output-citekeys: output/citations.tsv
manubot-requests-cache-path: ci/cache/requests-cache
manubot-clear-requests-cache: false
...






<small><em>
This manuscript
([permalink](https://elatella.github.io/deep-prepyto-paper/v/6d26ebf8fbeb7d1d2b309cd8921bc2880c3a600c/))
was automatically generated
from [elatella/deep-prepyto-paper@6d26ebf](https://github.com/elatella/deep-prepyto-paper/tree/6d26ebf8fbeb7d1d2b309cd8921bc2880c3a600c)
on January 19, 2022.
</em></small>

## Authors



+ **Amin Khosrozadeh**^[\*](#equal_contribution)^<br>
    ![ORCID icon](images/orcid.svg){.inline_icon}
    [XXXX-XXXX-XXXX-XXXX](https://orcid.org/XXXX-XXXX-XXXX-XXXX)
    · ![GitHub icon](images/github.svg){.inline_icon}
    [ameen-khosrowzadeh](https://github.com/ameen-khosrowzadeh)<br>
  <small>
     Institute of Anatomy, University of Bern, Bern, Switzerland; Graduate School for Cellular and Biomedical Sciences, University of Bern
     · Funded by Grant XXXXXXXX
  </small>

+ **Raphaela Seeger**^[\*](#equal_contribution)^<br>
    ![ORCID icon](images/orcid.svg){.inline_icon}
    [XXXX-XXXX-XXXX-XXXX](https://orcid.org/XXXX-XXXX-XXXX-XXXX)
    · ![GitHub icon](images/github.svg){.inline_icon}
    [elatella](https://github.com/elatella)<br>
  <small>
     Institute of Anatomy, University of Bern, Bern, Switzerland; Graduate School for Cellular and Biomedical Sciences, University of Bern
  </small>

+ **Julika Radecke**<br>
    ![ORCID icon](images/orcid.svg){.inline_icon}
    [0000-0002-5815-5537](https://orcid.org/0000-0002-5815-5537)
    · ![GitHub icon](images/github.svg){.inline_icon}
    [julikaradecke](https://github.com/julikaradecke)<br>
  <small>
     Institute of Anatomy, University of Bern, Bern, Switzerland; Department of Neuroscience, Faculty of Health and Medical Science , 2200 Copenhagen N, University of Copenhagen, Copenhagen, Denmark; Diamond Light Source Ltd, Didcot, Oxfordshire, United Kingdom
  </small>

+ **Guillaume Witz**<br>
    ![ORCID icon](images/orcid.svg){.inline_icon}
    [0000-0003-1562-4265](https://orcid.org/0000-0003-1562-4265)
    · ![GitHub icon](images/github.svg){.inline_icon}
    [guiwitz](https://github.com/guiwitz)<br>
  <small>
     Science IT Service, University of Bern, Bern, Switzerland; Microscopy Imaging Center, University of Bern, Bern, Switzerland
  </small>

+ **Jakob B. Sørensen**<br>
    ![ORCID icon](images/orcid.svg){.inline_icon}
    [0000-0001-5465-3769](https://orcid.org/0000-0001-5465-3769)
    · ![GitHub icon](images/github.svg){.inline_icon}
    [JBSorensen](https://github.com/JBSorensen)<br>
  <small>
     Department of Neuroscience, University of Copenhagen, Blegdamsvej 3B, 2200 Copenhagen N, Denmark
     · Funded by Novo Nordisk Fonden, NNF17OC0028516.; Carlsbergfondet, CF17-0875; Independent Research Fond Denmark, 8020-00228A; Lundbeckfonden, R277-2018-802
  </small>

+ **Benoît Zuber**^[✉](#correspondence)^<br>
    ![ORCID icon](images/orcid.svg){.inline_icon}
    [0000-0001-7725-5579](https://orcid.org/0000-0001-7725-5579)
    · ![GitHub icon](images/github.svg){.inline_icon}
    [aseedb](https://github.com/aseedb)<br>
  <small>
     Institute of Anatomy, University of Bern, Bern, Switzerland
     · Funded by Swiss National Science Foundation, 179520; ERA-NET NEURON, NEURON-119
  </small>


::: {#correspondence}
✉ Address correspondence to <benoit.zuber@ana.unibe.ch>.
:::
::: {#equal_contribution}
\* These authors contributed equally.
:::


## Abstract {.page_break_before}

Cryo-electron Tomography (Cryo-ET) has the potential to reveal cell structure down to atomic resolution.
Nevertheless, cellular cryo-ET data is often highly complex and visualization, as well as quantification, of subcellular structures require image segmentation.
Due to a relatively high level of noise and to anisotropic resolution in cryo-ET data, automatic segmentation based on classical computer vision approaches usually does not perform satisfyingly.
For this reason, cryo-ET researchers have mostly performed manual segmentation.

Communication between neurons rely on neurotransmitter-filled synaptic vesicle (SV) exocytosis.
Recruitment of SVs to the plasma membrane is an important means of regulating exocytosis and is influenced by interactions between SVs.
Cryo-ET study of the spatial organization of SVs and of their interconnections allows a better understanding of the mechanisms of exocytosis regulation.
To obtain a faithful representation of SV connectivity state, an absolutely vital prerequisite is an extremely accurate SV segmentation.
Hundreds to thousands of SVs are present in a typical synapse, and their manual segmentation is a burden.
Typically accurately segmenting all SVs in one synapse takes between 3 to 8 days.
This segmentation process has been widely recognized as a bottleneck by the community.

Several attempts to automate vesicle segmentation by classical computer vision or machine learning algorithms have not yielded very robust results.
We addressed this problem by designing a workflow consisting of a U-Net convolutional network followed by post-processing steps.
This combination yields highly accurate results.
Furthermore, we provide an interactive tool for accurately segmenting spherical vesicles in a fraction of the time required by available manual segmentation methods.
This tool can be used to segment vesicles that were missed by the fully automatic procedure or to quickly segment a handful of vesicles, while bypassing the fully automatic procedure.
Our pipeline can in principle be used to segment any spherical vesicle in any cell type as well as extracellular vesicles.


## Introduction

The rise of machine learning is sweeping the technological landscape.

While machine learning has been around for several decades prior to its boom, and it theoratically would be able to learn anything using a shallow neural network of 1 hidden layer (universal approximation theorem by Cybenko), more complex problems required several hidden layers. 
However, with an increased number of hidden layers, the chance of finding the correct weights, which are initialized as random numbers, through backpropagation is low, as they are being multiplied over the layers and eventually approach 0. 
The initilizing booster for this hype in 2006 was moving from back propagation in multiple layer neural networks and eventually vanish (they are fractions) to deep learning [@doi:10.1126/science.1127647]. 
Deep learning uses a new initalization strategy: series of single layer networks. (check the prior 2 sentences, especially if the citation fits)
In the following years many new publications revolutinized the field further with new concepts of how to train deep neural networks [@doi:10.5555/3042817.3043064] 

Since then the use cases of deep learning have become highly diverse and are just starting to reach the scientific community.
Especially the graphical deep-learning approaches have been quite popular [@doi:10.1056/NEJMra1814259].
Its approach is based around learning the description of the common attributes of a group or subset of a universe of objects [@doi:10.1017/S026988899700101X].
The segmentation of an input image is a typical area of application. 
Here the computer seperates the image into different partitions, each of them representing a different feature and traces the detected feature in the original image.
Adapting this image segmentation into the medical and biological research has resulted in the design of UNet [@doi:10.1007/978-3-319-24574-4_28].
UNet is able to localise, distinguish and trace borders, by treating the segmentation as a multiclass classification problem for each pixel.
Its architecture consists of two parts: the contracting part which captures context, and the symmetric expanding path that enables precise localization [@doi:10.1109/TPAMI.2021.3059968].
`*_What UNet type are we using: Extended 3D U-Net, Joint 2D-3D CNN, CNN with optimization module or Hierarchical networks_*`{.blue}

But also the field of cryo electron microscopy has recently recognized the benefits of machine/deep-learning approaches [@doi:10.1093/jmicro/dfz036].

The method of cryo-electron tomography (ET) utilises a series of tilted two-dimensional (2D) images to reconstruct a three-dimensional (3D) volume of the imaged sample [@doi:10.1042/BCJ20200715].

-> Describe more about cryo EM and cryo ET, also mention missing wedge problem

It brings many advantages compared to other cryo-electron microscopy (EM) methods, as it yields images at in situ conditions.
Therefore cryo ET can help to reveal the natural cellular environment of protein(-complexes), their function as well as their structure.
In order to analyze the cellular context within a tomogram, cellular features are being segmented. 
Popular programs for manual segementation are IMOD and Amira [@doi:10.1006/jsbi.1996.0013; @doi:10.1016/B978-012387582-2/50040-X].
Currently manual segmentation is being considered the bottleneck in the worklow timewise of cellular cryo-ET.

Our lab researches, with the help of cryo-ET, the synaptic architecture and its changes upon neurotransmitter vesicle release.
A special focus in that research holds the SNARE complex, which connects the synaptic vesicles and the presynaptic cell membrane, mediating vesicle fusion.
Their function and regulation still pose big questions.
In addition, mutations of involved proteins have been linked to numerous neurological diseases.
To address these issues, cryo-ET is the methode of choice. 
To perform quantitative studies on the resulting tomograms, accurate segmentation of both synaptic vesicles and the interconnecting filaments are required.
Among the different cell features, synaptic vesicles are the most time consuming to segment.
Despite their very homogeneous size and shape, their sheer number and finding their true center (due to the missing wedge problem) complicates their segmentation.

Problem 2D and 3D 

Our aim is the creation of a deep-learning pipeline, which is taught to segment cellular features, starting with synaptic vesicles.
We decided to teach our network with a real world dataset rather than using synthetic datasets, as it is often custom, as the synthetic datasets lack noise and would represent a complete 360° 3D object, which our datasets cannot due to the missing wedge problem in cryo-ET.
Our proposed method provides the initial step for downstream segmentation of subcellular compartments such as synaptic connectors and tethers for which an extremely accurate vesicle segmentation is required.


## Results


### Comparison of manual segmentation with automatic deep-learning based segmentation
Evaluation metric DICE for pixel/pixel analysis
Global analysis

![Dice coefficient and loss value for training and validation set.](images/blinddice.png){#fig:dice width="10cm"}


3d unet good for 3D processing
recent Nature methods paper by Ben Engel, DeepFinder -> Relion for STA creates mask to find more using dl
	-what are they doing, maybe compare that in the text, different aims; we might compare results we achieve (keep as bonus, revision)

3 different types of dl: classification, localization and segmentation
We specialize in accuratly segmenting 3D svs -> results
through the network, output is a mask, smooth DICE/ binary DICE = which one for our mask? one function for both? -> Amin will check
when we encounter error until now we remove sv(?), bug inside function -> fix bug for better performance, how many fail and why?
evaluation: objectwise evaluation for I/O, radius, center (according to nature paper) -> compare with manual seg
	other common evaluation tool other than DICE (Amin wants to check)
  
  

## Discussion

DICE

### Outlook
implement automatic cell-outline and active zone segmentation as deep learning workflow using UNet
implement automatic connector and tether segmentation as a deep leaning workflow using UNet





## Materials and methods

Benoît doing some tests.

### Cryo-electron Tomography Datasets

Two datasets of different origin were used as input and test subjects for the automatic segmentation pipeline, rat synaptosomes as well as astrocytic and neural cell cultures derived from mice.
`\_cite Vladan, segmentation write a bit more*`{.green}

#### Rat synaptosomes

The preparation of the rat synaptosomes were previously described [@doi:10.1038/nprot.2008.171].
After the purification, the synaptosomes were incubated for 30min at room temperature.
1.3mM CaCl2 and 10 nm gold fiducials were added (gold fiducials, #s10110/8. AURION Immuno Gold Reagents & Accessories. Wageningen, The Neatherlands).
The synaptosome solution was applied to a 200-mesh lacey finder carbon film grid (#AGS166-H2. Agar Scientific. Elektron Technology UK Ltd. Stansted, UK).
Manual blotting was used to remove exess liquid with the aid of a filter paper.
Thereafter the grid was immediately plunge frozen in liquid ethane using a homebuilt plunge freezer controlled with a LabView script (National Onstruments Corporation. Mopac Expwy Austin, TX, USA).
The grids coated with rat synaptosomes were mounted in a cryo-holder (Gatan, Pleasonton, CA, USA) and transferred to a Tecnai F20 (FEI, Eindhoven, The Netherlands) which was set to low dose conditions, operated at 200 kV, and equipped with a field emission gun.
Images were recorded with a 2k x 2k CCD camera (Gatan) mounted after a GIF Tridiem post-column filter (Gatan) operated in zero-loss mode.
The sample was kept at about -180°C.
Tilt series were acquired using SerialEM [@doi:10.1016/j.jsb.2005.07.007] for automated acquisition recorded typically from -50° to 50° with a 2° angular increment and an unbinned pixel size of 0.75 or 1.2 nm.
Due to sample thickness (400-700 nm), tomograms were usually not recorded with higher tilt angles.
Defocus was set between -8 to -12 µm and the total electron dose used was about 80-100 e^-^/Å^2^.
Some tomograms were acquired at a Titan Krios equipped with a K2 direct electron detector (Gatan) without energy filter.
The K2 camera was operated in superresolution counting mode and between 8-40 frames per tilt angle were taken.
Tilt series were acquired using the Latitude software (Gatan) for automated acquisition recorded typically from -60° to 60° with a 2° angular increment and an unbinned pixel size of 0.6 nm.
Defocus was set between -8 to -12 µm and the total electron dose used was about 80-100 e^-^/Å^2^.
Prior to image processing the frames at each tilt angle, frames were aligned and averaged in 2dx MC_Automator [@doi:10.1016/j.jsb.2014.03.016] with motioncor [@doi:10.1038/nmeth.2472].
3D reconstruction was done in IMOD [@doi:10.1006/jsbi.1996.0013].
The alignments were done using the automated fiducial tracking function and the 3D reconstructions were done using the weighted back projection followed by a nonlinear anisotropic diffusion (NAD) filtering.

#### Astrocytic and neuronal mouse culture

The preparation of astrocytic and neuronal culture has been published before [@doi:10.3791/50783].
After 12 to 14 days of incubation grids with mouse neurons were plunge frozen with a Vitrobot (Thermofisher Scientific, Mark IV) with a blot time of 3 s and a blot force of -10. Wait time and drain time were not used. Humidity was set to 100% at 4°C. 4 undiluteted 10 nm BSA gold tracer (Aurion) was added directly onto the grid prior to plunge freezing.
Cultured mouse neurons tilt series were acquired at a Titan Krios, equipped with a Falcon 3 direct electron detector (Thermofisher Scientific) without energy filter.
The Falcon camera was operated in linear mode.
Tilt series were acquired using the TEM Tomography software (TFS) for automated acquisition recorded typically from -60° to 60° with a 2° angular increment and an unbinned pixel size of 0.37 nm.
Defocus was set between -6 to -10 µm and the total electron dose used was about 80-100 e^-^/Å^2^.
Tomogram reconstruction was done in the same way as for the synaptosome datasets.

### Manual segmentation procedures

Manual segmentation of SVs, mitochondria, and the active zone PM was done in IMOD (Figure S4A&B).
The boundary marked the region to be analyzed by Pyto [@doi:10.1016/j.jsb.2016.10.004].
The analysis by Pyto was essentially the same as described previously [@doi:10.1083/jcb.200908082] [@doi:10.1016/j.jsb.2016.10.004].

In short, the segmented area is divided in 1 voxel thick layers parallel to the active zone for distance calculations.
A hierarchical connectivity segmentation detects densities interconnecting vesicles (so called connectors) and densities connecting vesicles to the active zone PM (so called tethers) (Figure S4C).
Distance calculations are done with the center of the vesicle.
Mainly default settings were used.
The segmentation procedure is conservative and tends to miss some tethers and connectors because of noise.
Consequently, the numbers of tethers and connectors should not be considered as absolute values but rather to compare experimental groups.
As it was done before, an upper limit was set between 2100 and 3200 nm3 on segment volume.
The tomograms that were used for this analysis were binned by a factor of 2 to 3, resulting in voxel sizes between 2.1 and 2.4 nm.

### Pre-processing of manual segmentation outputs from IMOD for further use (jupyter notebook pre-pyto)



### Description of Machine Learning: Training Stage


#### Deep Model Training  
Unet
Training Datasets and Batch Generation

### Transfer Learning


#### Optimization / Postprocessing
-Global Threshold

-Mask Tuning

-Compute Radial Profile

-Radius Estimation (Cross Correlation through Radial Profile)
-Remove Outlier Labels

### Analysis of Results


## References {.page_break_before}

<!-- Explicitly insert bibliography here -->
<div id="refs"></div>
