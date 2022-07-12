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
date-meta: '2022-07-12'
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
  <meta name="dc.date" content="2022-07-12" />
  <meta name="citation_publication_date" content="2022-07-12" />
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
  <link rel="alternate" type="text/html" href="https://elatella.github.io/deep-prepyto-paper/v/bb3d0ac988aab0ce06b7a095630bf125459e9bf7/" />
  <meta name="manubot_html_url_versioned" content="https://elatella.github.io/deep-prepyto-paper/v/bb3d0ac988aab0ce06b7a095630bf125459e9bf7/" />
  <meta name="manubot_pdf_url_versioned" content="https://elatella.github.io/deep-prepyto-paper/v/bb3d0ac988aab0ce06b7a095630bf125459e9bf7/manuscript.pdf" />
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
([permalink](https://elatella.github.io/deep-prepyto-paper/v/bb3d0ac988aab0ce06b7a095630bf125459e9bf7/))
was automatically generated
from [elatella/deep-prepyto-paper@bb3d0ac](https://github.com/elatella/deep-prepyto-paper/tree/bb3d0ac988aab0ce06b7a095630bf125459e9bf7)
on July 12, 2022.
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

The fine architecture of cells can be investigated by cryo-electron tomography (cryo-ET) [@doi:10.1016/j.jmb.2021.167187].
Cellular structures are preserved down to the atomic scale through vitrification and observation of the samples in a fully hydrated state.
When a macromolecule is present in a sufficient number of copies in the cells imaged by cryo-ET, it is possible to obtain its atomic structure in situ using subtomogram averaging [@doi:10.1101/2022.01.10.475481; @doi:10.1038/s41596-021-00648-5].
Cellular cryo-ET datasets are usually extremely complex, making them difficult to analyze. 
This is aggravated by the sensitivity of biological samples to electron radiation, which limits the signal-to-noise ratio in cryo-ET datasets [@doi:10.1146/annurev.biochem.73.011303.074112].
Tomographic reconstructions are generated from a series of images of the sample acquired at different viewing angles.
The geometry of the samples prevents acquisition at certain angles, resulting in anisotropic spatial coverage.
The resolution in the directions close to the axis of the electron beam incident on the untilted sample is strongly reduced. 
This effect, commonly referred to as the missing-wedge artifact, further complicates data analysis. 
In particular, organelles fully bounded by a membrane appear to have holes at their top and bottom (relative to the electron beam axis) [@doi:10.1146/annurev.biochem.73.011303.074112].

The synapse is the functional cellular contact at which information is transmitted from a neuron to another. 
The former neuron is called presynaptic and the latter is postsynaptic. 
In most cases, the signal is transmitted by the release of neurotransmitters into the intercellular space.
Neurotransmitters are stored in SVs and are released following the fusion of a vesicle with the presynaptic plasma membrane.
A synapse contains hundreds of SVs and their mobility and recruitability for neurotransmitter release depends on inter-vesicle interactions through so-called connector structures [@doi:10.1083/jcb.200908082 ]. 
The characterization of these interactions can be performed automatically with the pyto software, which implements a hierarchical connectivity approach to detect and annotate connectors [@doi:10.1016/j.jsb.2016.10.004]. For accurate connector segmentation, an exceptionally precise segmentation of SVs is prerequisite.
To date, this SV segmentation has been achieved manually, but given the massive number of SVs per dataset, it is an extremely time-consuming process. 
Typically, one person spends 3 to 8 working days to segment a single dataset.
Attempts to perform this task automatically based on classical computer vision algorithms have not yielded sufficiently accurate performance [@doi:10.1016/j.jsb.2014.02.015].  
To alleviate this situation, we considered applying deep learning methods.

Convolutional neural networks (CNN) have been successfully employed to segment cryo-ET data [@doi:10.1038/nmeth.4405]. 
Although entirely satisfying for visualization purposes, this approach has not met the requirements of pyto.
A recent publication described accurate SV segmentation of transmission electron microscopy images using CNN, but it is limited to 2-dimensional images of resin-embedded synapses [@doi:10.1523/ENEURO.0400-20.2021]. 
For our use-case, a common issue is that the input data consists of 2-dimensional images.
In the first study, cryo-ET data are decomposed in individual 2-dimensional slices, which are handed as seperate input to the CNN. 
The independent output prediction images are re-assembled in a 3-dimensional stack.[@doi:10.1038/nmeth.4405]
As discussed above, membranes oriented approximately parallel to the plane of the 2-dimensional tomographic images are not resolved.
In the absence of contextual knowledge of the other 2-dimensional images, the CNN fails to segment these regions of the vesicles.
Hence, spherical vesicles appear open, whereas we expect closed spherical objects.
To overcome this limitation, we used a U-Net CNN that takes 3-dimensional images as input.
U-Net architecture has been introduced in 2015 by Ronenberger et al. [@arxiv:1505.04597].
It consists of a contracting path, typical of CNN, and a symmetric expanding path. 
At each expansion step, the correspondingly cropped feature map of the contracting path is concatenated. 
The contracting path captures context, while the expanding path coupled with concatenation enables precise localization.
The U-Net architecture was developed to achieve a fast and accurate segmentation of biomedical two-dimensional images, with the requirement of only a small fraction of training data in comparison to previous CNNs.
It was then extended to segment 3-dimensional biomedical images (3D U-Net) [@arxiv:1606.06650].
Weigert et al. [@doi:10.1038/s41592-018-0216-7] implemented a U-Net for content-aware restoration (CARE) of 3-dimensional fluorescence microscopy datasets. They showed that it can restore information from anisotropic and very noisy datasets.

We implemented a 3D U-Net based on CARE building blocks and trained it with manually segmented datasets. 
This method provided good accuracy and was only slightly affected by the missing wedge artifact. 
Nevertheless, it was not quite sufficient for our downstream pyto analysis.
Hence, we developed a post-processing method, which transforms the segmented objects into spheres and refines their radius and center location.
This leads to a substantial accuracy improvement, which are reflected in better pyto performance.
Additionally, we designed a multivariate ranking procedure, highlighting possibly wrongly segmented SVs. 
We also introduce a semi-automatic method to very quickly fix wrongly segmented and missed SVs.

Although our set of procedures was developed with the use case of SV segmentation in mind, it can be used to segment any other types of biological spherical vesicles, such as transport vesicles, secretory vesicles, endocytic vesicles, and extracellular vesicles.


## Results

To automize the tracing of cellular features in tomograms, also called segmentation, we developed a deep-learning pipeline, which segments 3D objects.
-> similar approaches in 2D
The manual segmentation of synaptic vesicles is one of the most time-intensive steps, when segmenting tomograms of presynaptic terminals.
Synaptic vesicles also constitute a large, homogeneous group, which would create a large training set for deep learning applications.
Therefore, we decided to develop the automatic segmentation for synaptic vesicles in an initial step.
The used tomograms were previously manually segmented with IMOD [@doi:10.1006/jsbi.1996.0013].
In a next step, filaments connecting the synaptic vesicles with each other (connectors) and to the active zone (AZ) were automatically segmented with the algorithm application Pyto [@doi:10.1016/j.jsb.2016.10.004].

![**Pipeline of automatic segmentation.** a) tomograms b) patchify the tomograms into 3D patches c) Segmentation Network d) probability masks  e) stitching patches back f) thresholding g) adaptive localized thresholding h) outlier removal i) radial profile](images/pipeline.svg){#fig:pipeline width="15cm"}

![**Segmentation Network: UNET.** Input Size is 32^3, in each resolution we have two convolution layer followed by batch normalization layer and relu activation function. Intermediate sizes are written on top of arrows, number of convolution filters is written bottom of boxes. Skip connections shows concatenation of the features from contracting path (left side of the network) and expansive path (right side of the network).](images/unet.png){#fig:unet width="10cm"}

![**2D Slices** A) a section from z axis of a tomogram’s presynaptic terminal of a neuron B) instance mask of the vesicles after post processing C) predicted probability mask by the segmentation network](images/tomo.svg){#fig:tom width="15cm"}

Fig 4- Dice improvements after post processing of initial predicted mask (different colors correspond to different tomograms ): a) training datasets b) synaptosome test datasets c) Neuron test datasets

![**Vesicle radius and position through radial profile and cross-correlation**
Radial Profile Refinement A) couple of vesicles are not centered B) Radial Profile. Blue range is from membrane center to outer white halo center, this is the search range for the optimal radius. (smoothed by gaussian filtering) C) second derivative of radial profile
E, F, H, G) Same as above columns after refinement.] (images/radial_avg_115-099.svg){#fig:radial_profile width="15cm"}

Fig 6- Splitting adjacent vesicles. A) Examples of tomogram, no labels; B) raw label with connected vesicle-labels; C) modified label with seperated vesicles ---> for software: IMOD

### Comparison of manual segmentation with automatic deep-learning based segmentation

![**3D model of manual segmented and automatically segmented synaptosome.**](images/3d.png)

Evaluation metric DICE for pixel/pixel analysis

Table 1- Evaluation of the segmentation- MDICE: Mask Dice coefficient for the predicted mask PDICE: Dice coefficient after post-processing SIGMA-d: diameter error on correctly detected vesicle, DELTA-c: average error center (nm) #Vesicles: number of expected vesicles TP: True Positive FN: False Negative FP: False Positive

Global analysis

![**Dice coefficient and loss value for training and validation set.** ](images/blinddice.png){#fig:dice width="10cm"}

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
1. Create a training set
	Since the scientific question of our manually segmented data was for the specific region of interest and consequently prepared segmentation was accomplished on the specific region of interest in the tomograms therefore they did not contain all vesicles in the tomogram (in the synaptosome the first 250 nm away from the active zone was interested). Moreover, because our cryo-EM images are high resolution (pixel size around 1 nm) and the data size is relativity huge we can not also feed the whole image into our model. Hence due to limited memory, we prepare our training set by splitting each volume into 32x32x32 sub volumes and keeping only volumes occupied by a sufficient amount of binarized label (at least 1000 voxels from vesicles).
To train the network we divided the data into 10 folds and randomly chose between the created sub-volumes generated in the previous step. For validation of our training, we determine the last fold of data almost entirely from aside tomogram to avoid overfitting.

#### Deep Model Training
2. Training the 3D U-NET
	This Experiment was conducted on AMD Ryzen Threadripper 3970X, 32x 3.7GHz workstation empowered NVIDIA GeForce RTX 2080 Ti, 11GB. All the framework has been implemented in Python using the Keras library (2.4.3) and Tensorflow (2.4.1). Moreover, we developed the GUI based on Napari (0.4.15) multi-dimensional image viewer for adding and removing vesicles by users.
  Kernel size determined 3x3x3, we double the number of channels every time and down sample the voxel. For 200 epochs, the batch size was 50, and to stabilize our training we used batch normalization. Furthermore, on configuration, we resolved binary cross-entropy as a loss function and Adam optimizer for the training of the network.

In the encoding path, we have two layers of the resolution followed by two convolutional layers, Kernel size determined 3x3x3, we double the number of channels every time and down sample the voxel with Max poling of 2x2x2. In the decoder path, the setup is arranged similarly to the contraction path but with up convolution operation. Each convolutional layer in the network goes along with the RELU activation function. Come after the convolutional layers to achieve 3D probability mask a Softmax layer applies to bring channel size to one.

3. Mask prediction
	We split large tomograms into 32x32x32 patches with step size of 24 (stride) and then stitch together the predictions to get the final probability mask.


Unet
Training Datasets and Batch Generation

### Transfer Learning


#### Optimization / Postprocessing
-Global Threshold
-Mask Tuning
-Compute Radial Profile
-Remove Outlier Labels
-Radius Estimation (Cross Correlation through Radial Profile)

1. Estimating global threshold
	In order to binarize the obtained probability mask, we search through some thresholds (from 0.8 to 1.0) and select the one that minimizes something.

2. Adaptive localized threshold
although the global threshold reveals almost all desired synaptic vesicles due to variation in the intensity of vesicles surrounding some binarized labels that are far away from the spherical shape of vesicles. First, by looking at the extent value(Ratio of pixels in the region to pixels in the total bounding box. Computed as area / (rows * cols)) and the size of each particle’s binary label we can capture those vesicles that are get connected and those vesicles that captured partially.
Then by searching more into the probability mask, we try to expand the partially detected vesicles and separate those close connected vesicles by searching between the initial threshold and one to find a better finner threshold that can separate these vesicles.


3. Radial Profile

4.Outlier removal

We define feature space on predicted vesicles’ label containing thickness, membrane density, and estimated radius of a vesicle. (Benoit: after radial profile, we can add the definition of thinness and membrane as well)
While we face different metrics for detecting outliers we apply Mahalanobis Distance MD on this multivariate space MD to calculate L2 norm distance on normalized variable using the covariance matrix of observation. Afterward, we calculate the p-value of MD and bring this evaluation setup in iterative form while giving the second chance to detect outlier vesicles while recalculating radial profile in a specific margin range (0-10) and removing them if they could not pass a margin on the p-value.


### Analysis of Results


## References {.page_break_before}

<!-- Explicitly insert bibliography here -->
<div id="refs"></div>
