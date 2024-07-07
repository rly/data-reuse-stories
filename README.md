# data-reuse-stories
Examples of reuse of publicly accessible neurophysiology datasets and analysis code

## Data reuse examples from the Allen Brain Observatory
de Vries, S. E. J., Siegle, J. H., & Koch, C. (2023). **Sharing neurophysiology data from the Allen Brain Observatory.** eLife, 12, e85550. [https://doi.org/10.7554/eLife.85550](https://doi.org/10.7554/eLife.85550)

See the above paper for a comprehensive review of over 100 publications and preprints that reuse Allen Brain Observatory data prior to its publication (July 2023) for:
1. scientific discovery
2. validation of models and algorithms
3. comparison with other datasets
4. education

I may summarize those examples here in the future.

## NWB data reuse

See [Ryan's Notion Database of NWB Data Reuse Publications](https://www.notion.so/rly1/8b1d1f08841e41b89fdd9ab21d486d31?v=99f8e0f855a5486b8fc521066b34d4b3) for the latest, filterable table of papers that reused publicly available NWB data, from DANDI and other sources.

NWB Overview listing of data analysis and reuse examples
- https://nwb-overview.readthedocs.io/en/latest/community_gallery/community_gallery.html#data-analysis-and-reuse

DANDI Notebooks collection (Python)
- https://github.com/dandi/example-notebooks

Example MATLAB Live Scripts collection (MATLAB)
- https://github.com/MATLAB-Community-Toolboxes-at-INCF/example-live-scripts

MATLAB Live Script associated with:
Najafi, F., Elsayed, G. F., Cao, R., Pnevmatikakis, E., Latham, P. E., Cunningham, J. P., & Churchland, A. K. (2020). **Excitatory and inhibitory subnetworks are equally selective during decision-making and emerge simultaneously during learning.** Neuron, 105(1), 165-179.
- https://github.com/datajoint-company/najafi-2018-matlab

[OpenScope Databook](https://alleninstitute.github.io/openscope_databook/intro.html)

## Other examples

Uses of the **AJILE12 dataset** prior(?) to publication as an NWB dataset on DANDI:
- Steven M Peterson, Zoe Steine-Hanson, Nathan Davis, Rajesh PN Rao, and Bingni W Brunton. **Generalized neural decoders for transfer learning across participants and recording modalities.** Journal of Neural Engineering, 18(2):026014, 2021.
- Nancy Wang, Ali Farhadi, Rajesh Rao, and Bingni Brunton. **Ajile movement prediction: Multimodal deep learning for natural human neural recordings and video.** In Proceedings of the AAAI Conference on Artificial Intelligence, volume 32, 2018.
- Steven Michael Peterson, Rajesh PN Rao, and Bingni Wen Brunton. **Learning neural decoders without labels using multiple data streams.** bioRxiv, 2021.
- Steven M Peterson, Satpreet H Singh, Nancy XR Wang, Rajesh PN Rao, and Bingni W Brunton. **Behavioral and neural variability of naturalistic arm movements.** Eneuro, 8(3), 2021.
- Neuromatch Academy project
    - Notebook: https://colab.research.google.com/github/NeuromatchAcademy/course-content/blob/main/projects/ECoG/exploreAJILE12.ipynb
    - Notebook: https://github.com/neurovium/Neuromatch-AJILE12/blob/master/Notebook/exploreAJILE12.ipynb
    - Code: https://github.com/neurovium/Neuromatch-AJILE12

**SpikeForest**
- https://elifesciences.org/articles/55167
- https://github.com/flatironinstitute/spikeforest
- Data is also available on DANDI: https://dandiarchive.org/dandiset/000618

A non-scientist friend of Ryan's used Neuropixels spiking data from [dandiset 000053](https://dandiarchive.org/dandiset/000053) to make music.

**Inferring brain-wide interactions using data-constrained recurrent neural network models**
Matthew G. Perich, Charlotte Arlt, Sofia Soares, Megan E. Young, Clayton P. Mosher, Juri Minxha, Eugene Carter, Ueli Rutishauser, Peter H. Rudebeck, Christopher D. Harvey, Kanaka Rajan
- https://www.biorxiv.org/content/10.1101/2020.12.18.423348v2
- Used multi-region datasets from mice during running, macaques during Pavlovian conditioning, and humans during memory retrieval.
- Data do not appear to be publicly available.

**Orthogonal representations for robust context-dependent task performance in brains and neural networks**
Timo Flesch, Keno Juechems, Tsvetomira Dumbalska, Andrew Saxe, and Christopher Summerfield
- https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8992799/
- Reused "a freely available dataset describing single-neuron activity in frontal eye fields (FEF) while macaques performed an equivalent context-dependent decision task on stimuli with varying color and motion coherence (Mante et al., 2013; Aoi et al., 2019)"
- With a follow-up note from both these data reuse authors and the original data authors: https://arxiv.org/abs/2306.16733
- Data is available at https://www.ini.uzh.ch/en/research/groups/mante/data.html

**Preserved neural dynamics across animals performing similar behaviour**
Mostafa Safaie, Joanna C. Chang, Junchol Park, Lee E. Miller, Joshua T. Dudman, Matthew G. Perich & Juan A. Gallego
- https://www.nature.com/articles/s41586-023-06714-0
- Used data of "recordings of neural populations from monkey and mouse motor cortex to demonstrate that neural dynamics in individuals from the same species are surprisingly preserved when they perform similar behaviour"
- "Most of the monkey datasets are publicly available on Dryad (https://datadryad.org/stash/dataset/doi:10.5061/dryad.xd2547dkt) and CRCNS (https://doi.org/10.6080/K0FT8J72). The remaining monkey datasets and the mouse datasets will be made available on reasonable request."
- NOTE: The authors seem to be heavily involved with the original data collection experiments, so this may be more of a "we reused our own data" instead of a "we reused others' data" story.

**Diversity amongst human cortical pyramidal neurons revealed via their sag currents and frequency preferences**
Homeira Moradi Chameh, Scott Rich, Lihua Wang, Fu-Der Chen, Liang Zhang, Peter L. Carlen, Shreejoy J. Tripathy & Taufik A. Valiante
- https://doi.org/10.1038/s41467-021-22741-9
- "We also made use of a publicly accessible dataset of 272 pyramidal cells sampled from L2, L3, and L5 from an additional cohort of 39 human surgical patients characterized by the Allen Institute for Brain Sciences (http://celltypes.brain-map.org/)"

Uses of the [**O'Doherty et al., 2020 NHP Reaching dataset**](https://zenodo.org/records/3854034)
- 30+ instances of documented reuses of this dataset under section "Publications making use of this dataset."
- including some mentioned above

**A doubly stochastic renewal framework for partitioning spiking variability**
https://www.biorxiv.org/content/10.1101/2024.02.21.581457v1
need to check whether data is public

**Unifying community-wide whole-brain imaging datasets enables robust automated neuron identification and reveals determinants of neuron positioning in C. elegans**
Sprague, D. Y., Rusch, K., Dunn, R. L., Borchardt, J., Bubnis, G., Chiu, G., ... & Kato, S. (2024). Unifying community-wide whole-brain imaging datasets enables robust automated neuron identification and reveals determinants of neuron positioning in C. elegans. bioRxiv, 2024-04.
- https://www.biorxiv.org/content/10.1101/2024.04.28.591397v1
- Data were originally stored in non-NWB formats and were later converted to NWB and uploaded to DANDI.
- Datasets used:
    - Original neuroPAL: https://doi.org/10.48324/dandi.000715/0.240424.1847
    - EY: TBD
    - HL: https://doi.org/10.48324/dandi.000714/0.240402.2115
    - KK: https://doi.org/10.48324/dandi.000692/0.240402.2118
    - SK1: TBD
    - SK2: https://doi.org/10.48324/dandi.000472/0.240402.2117
    - SF: TBD

**A machine learning toolbox for the analysis of sharp-wave ripples reveals common waveform features across species.**
Navas-Olive, A., Rubio, A., Abbaspoor, S., Hoffman, K. L., & de la Prida, L. M. (2024). A machine learning toolbox for the analysis of sharp-wave ripples reveals common waveform features across species. Communications Biology, 7(1), 1-15.

**Learning identifiable and interpretable latent models of high-dimensional neural activity using pi-VAE. **
Zhou, D., & Wei, X. Adv. Neural Inf. Process. Syst. 
- https://proceedings.neurips.cc//paper/2020/file/510f2318f324cf07fce24c3a4b89c771-Paper.pdf
- "You can find code to generate the simulated data in our paper ./examples/simulate_data.ipynb."
    - https://github.com/zhd96/pi-vae
- Used data from <https://portal.nersc.gov/project/crcns/download/hc-11/data/>](https://portal.nersc.gov/project/crcns/download/hc-11/data/), session Achilles_10252013

**Compression strategies for large-scale electrophysiology data.**
Buccino et al. Journal of Neural Engineering.
- https://iopscience.iop.org/article/10.1088/1741-2552/acf5a4/meta#jneacf5a4t1
- Used raw ephys data from IBL Brain Wide Map and pilot sessions from AIND.

## Miscellaneous

Replications of experimental research can be published in [Rescience X](http://rescience.org/x). Replications of computational research can be published in [Rescience C](https://rescience.github.io/).

Benefits of sharing neurophysiology data from the BRAIN Initiative Research Opportunities in Humans Consortium
Vasiliki Rahimzadeh et al. (2023). Neuron. DOI:https://doi.org/10.1016/j.neuron.2023.09.029
https://www.cell.com/neuron/pdf/S0896-6273(23)00717-1.pdf
- "The standardized datasets also have doubled as an educational resource for unique users. For example, children ages 8 to 15 years reviewed the data using NWB-based graphical user interfaces and helped translate the original publication of the dataset into a version for Frontiers for Young Minds. [https://doi.org/10.3389/frym.2023.968856] The interactive, web-based viewing, made possible by DANDI, enabled readers with limited programming experience to visualize the structured data and understand key findings from the parent study."
- and other stories and comments about data sharing and reuse

TODO: it looks like DANDI tracks citations "dCite:IsReferencedBy" on individual dandiset pages. How is this done?

Every research result paper from the Allen Institute is basically reuse of their publicly shared data, often by different groups. Does that count?
