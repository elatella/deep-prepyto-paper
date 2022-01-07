---
title: Morphofunctional changes at the active zone during synaptic vesicle exocytosis
keywords:
- synapse
- cryo-electron tomography
- synaptic vesicles
- deep learning
- segmentation
- post-processing
lang: en-US
date-meta: '2022-01-07'
author-meta:
- Amin Khosrozadeh
- Raphaela Seeger
- Julika Radecke
- Guillaume Witz
- Vladan Lučić
- Jakob B. Sørensen
- Benoît Zuber
header-includes: |-
  <!--
  Manubot generated metadata rendered from header-includes-template.html.
  Suggest improvements at https://github.com/manubot/manubot/blob/main/manubot/process/header-includes-template.html
  -->
  <meta name="dc.format" content="text/html" />
  <meta name="dc.title" content="Morphofunctional changes at the active zone during synaptic vesicle exocytosis" />
  <meta name="citation_title" content="Morphofunctional changes at the active zone during synaptic vesicle exocytosis" />
  <meta property="og:title" content="Morphofunctional changes at the active zone during synaptic vesicle exocytosis" />
  <meta property="twitter:title" content="Morphofunctional changes at the active zone during synaptic vesicle exocytosis" />
  <meta name="dc.date" content="2022-01-07" />
  <meta name="citation_publication_date" content="2022-01-07" />
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
  <meta name="citation_author_orcid" content="0000-0003-1562-4265" />
  <meta name="citation_author" content="Vladan Lučić" />
  <meta name="citation_author_institution" content="Max-Planck-Institute of Biochemistry, Am Klopferspitz 18, 82152 Martinsried, Germany" />
  <meta name="citation_author_orcid" content="0000-0003-3698-7436" />
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
  <link rel="alternate" type="text/html" href="https://elatella.github.io/deep-prepyto-paper/v/69b721acec69104302323287baac8151ed026c3a/" />
  <meta name="manubot_html_url_versioned" content="https://elatella.github.io/deep-prepyto-paper/v/69b721acec69104302323287baac8151ed026c3a/" />
  <meta name="manubot_pdf_url_versioned" content="https://elatella.github.io/deep-prepyto-paper/v/69b721acec69104302323287baac8151ed026c3a/manuscript.pdf" />
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
([permalink](https://elatella.github.io/deep-prepyto-paper/v/69b721acec69104302323287baac8151ed026c3a/))
was automatically generated
from [elatella/deep-prepyto-paper@69b721a](https://github.com/elatella/deep-prepyto-paper/tree/69b721acec69104302323287baac8151ed026c3a)
on January 7, 2022.
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
     Science IT Service, University of Bern, Bern, Switzerland
  </small>

+ **Vladan Lučić**<br>
    ![ORCID icon](images/orcid.svg){.inline_icon}
    [0000-0003-3698-7436](https://orcid.org/0000-0003-3698-7436)
    · ![GitHub icon](images/github.svg){.inline_icon}
    [vladanl](https://github.com/vladanl)<br>
  <small>
     Max-Planck-Institute of Biochemistry, Am Klopferspitz 18, 82152 Martinsried, Germany
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
✉ Address correspondence to <benoit.zuber@ana.unibe.ch> and <jakobbs@sund.ku.dk>.
:::
::: {#equal_contribution}
\* These authors contributed equally.
:::


## Abstract {.page_break_before}

The communication between neurons is based on the exocytosis of neurotransmitter filled vesicles. Even small disbalances in this delicate system can result in different disorders. Numerous questions are still unanswered about synaptic vesicle exocytosis regulation as well as about which proteins affect this fundamental process. Hundreds to thousands of vesicles are present at the synapse and most of them are interconnected. There is a number of evidence suggesting that the connectivity between the vesicles influences synaptic vesicle exocytotic activity and that connectivity can be regulated. To address these issues, cryo-electron tomography is a method of choice. Yet inevitable quantitative studies require accurate segmentation of both synaptic vesicles and the interconnecting filaments.

This segmentation process has been widely recognized as a bottleneck by the community. When working with synapses, an incredibly tedious cellular feature to segment are synaptic vesicles. Even though they have a very homogeneous shape and size, which makes it easy to distinguish them from other cellular features, their high occurrence makes their segmentation challenging (one average-sized synapse or synaptosomes can easily contain between 300-500 synaptic vesicles).

Several attempts at utilizing machine learning algorithms  to automize the segmentation of synaptic vesicles yielded in unfavorable results. We analyzed these approaches and realized that most algorithms solely worked with the 2D image planes within the tomogram, but didn’t tap into their 3D information and therefore increased the weight of the missing wedge.

We designed a framework that consists of two parts: 1) U-Net convolutional network to obtain mask for SVs following by 2) post-processing step which fine-tunes the mask and provides entire 3D-vesicles. A deep-learning model has been trained with manually segmented synaptic vesicles, which have been entirely annotated as 3D objects. By post-processing, we achieved to transfer the vesicle recognition through this pipeline. The evaluation metrics like the DICE value suggest a very high success rate.


## Introduction

The rise of machine learning is sweeping the technological landscape.
Its use cases are highly diverse and are just starting to reach the scientific community.
Especially the graphical deep-learning approaches have been quite popular [@doi:10.1056/NEJMra1814259].
The graphical deep-learning approach is based around learning the description of the common attributes of a group or subset of a universe of objects [@doi:10.1017/S026988899700101X].
Describe the typical make up of a deeplearning approach
But also the field of cryo electron microscopy has recently recognized the benefits of machine/deep-learning approaches [@doi:10.1093/jmicro/dfz036].

The method of cryo-electron tomography (ET) utilises a series of tilted two-dimensional (2D) images to reconstruct a three-dimensional (3D) image of the imaged sample [@doi:10.1042/BCJ20200715].
It brings many advantages compared to other cryo-electron microscopy (EM) methods, as it yields images at in situ conditions.
Therefore cryo ET can help to reveal the natural cellular environment of protein(-complexes), their function as well as their structure.
In order to analyze the cellular context within a tomogram, cellular features are being segmented. 
Popular programs for manual segementation are IMOD and Amira [@doi:10.1006/jsbi.1996.0013; @doi:10.1016/B978-012387582-2/50040-X].
Currently manual segmentation is being considered the bottleneck in the worklow of cellular cryo-ET.

Problem 2D and 3D 

3D machine learning
We decided to teach our network with a real world dataset rather than using synthetic datasets, as it is often custom, as the synthetic datasets lack noise and ould represent a complete 360° 3D object, which our datasets cannot due to the missing wedge problem in cryo-ET.


## Results


### Comparison of manual segmentation with automatic deep-learning based segmentation



## Discussion






## Materials and methods

### Cryo-electron Tomography Datasets

Two datasets of different origin were used as input and test subjects for the automatic segmentation pipeline, rat synaptosomes as well as astrocytic and neural cell cultures derived from mice.

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

### Description of Machine Learning: Training Stage

### Training Datasets and Batch Generation

### Optimization / Postprocessing

### Analysis of Results


## References {.page_break_before}

<!-- Explicitly insert bibliography here -->
<div id="refs"></div>
