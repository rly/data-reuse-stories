# data-reuse-stories
Examples of reuse of publicly accessible neurophysiology datasets and analysis code

## A survey
de Vries, S. E. J., Siegle, J. H., & Koch, C. (2023). **Sharing neurophysiology data from the Allen Brain Observatory.** eLife, 12, e85550. https://doi.org/10.7554/eLife.85550

See the above paper for a comprehensive review of examples of reuse of Allen Brain Observatory data prior to publication (July 2023) for:
1. scientific discovery
2. validation of models and algorithms
3. comparison with other datasets
4. education

I may summarize those examples here in the future.

## Papers

### Allen Institute Visual Coding - Neuropixels (DANDI:000021)

Lowet, E., Sheehan, D. J., Chialva, U., De Oliveira Pena, R., Mount, R. A., Xiao, S., Zhou, S. L., Tseng, H. A., Gritton, H., Shroff, S., Kondabolu, K., Cheung, C., Wang, Y., Piatkevich, K. D., Boyden, E. S., Mertz, J., Hasselmo, M. E., Rotstein, H. G., & Han, X. (2023). **Theta and gamma rhythmic coding through two spike output modes in the hippocampus during spatial navigation.** Cell reports, 42(8), 112906. Advance online publication. https://doi.org/10.1016/j.celrep.2023.112906
1. Used Allen Brain Observatory Neuropixels data -- specifically, spiking of all CA1 neurons from wild-type mice viewing the "Brain Observatory 1.1" stimulus set
    1. Data description: https://portal.brain-map.org/explore/circuits/visual-coding-neuropixels
    1. Data via Brain Observatory Toolbox: https://www.mathworks.com/matlabcentral/fileexchange/90900-brain-observatory-toolbox
    1. Data via allensdk: https://allensdk.readthedocs.io/en/latest/visual_coding_neuropixels.html
    1. Data on DANDI: https://dandiarchive.org/dandiset/000021
1. Data was used to corroborate the authors' main findings of
    1. The percentage of spikes from CA1 neurons that were spike bursts
    1. The average spike rate of CA1 neurons (partial support)
    1. Differential coupling of spike bursts and single spikes to LFP rhythms: coupling of spike bursts to theta (5-12 Hz) was stronger than coupling of single spikes to theta, coupling of spike bursts to gamma (30-90 Hz) was weaker than coupling of single spikes to gamma

### AJILE12 dataset (DANDI:000055)

Nguyen, D. T., Nguyen, M. D. T., Hy, T. S., & Kondor, R. (2023). **Fast Temporal Wavelet Graph Neural Networks.** arXiv preprint arXiv:2302.08643. https://arxiv.org/abs/2302.08643
1. Used AJILE12 dataset (DANDI:000055) - specifically, one hour of recording from subject id 5.
    1. Data descriptor paper: https://www.nature.com/articles/s41597-022-01280-y
    2. Data on DANDI: https://dandiarchive.org/dandiset/000055
1. Code appears to use a transformed version of the neural data (.npy file)
    1. Code: https://github.com/HySonLab/TWGNN/
1. Data was used to evaluate the authors' proposed model, FTWGNN, against other models. The authors found that:
    1. FTWGNN outperforms other models by most metrics
    2. FTWGNN performs well at 1-second prediction, but produces unstable and erroneous forecasts for steps of 5 or 15 seconds
    3. FTWGNN is faster than DCRNN by at least 2X

Talukder, S., Sun, J. J., Leonard, M., Brunton, B. W., & Yue, Y. (2022). **Deep Neural Imputation: A Framework for Recovering Incomplete Brain Recordings.** arXiv preprint arXiv:2206.08094. https://arxiv.org/abs/2206.08094
1. Used AJILE12 dataset (DANDI:000055)
2. Data generator (Bing Brunton) is a coauthor on the paper

Other uses of this dataset:
- Steven M Peterson, Zoe Steine-Hanson, Nathan Davis, Rajesh PN Rao, and Bingni W Brunton. **Generalized neural decoders for transfer learning across participants and recording modalities.** Journal of Neural Engineering, 18(2):026014, 2021.
- Nancy Wang, Ali Farhadi, Rajesh Rao, and Bingni Brunton. **Ajile movement prediction: Multimodal deep learning for natural human neural recordings and video.** In Proceedings of the AAAI Conference on Artificial Intelligence, volume 32, 2018.
- Steven Michael Peterson, Rajesh PN Rao, and Bingni Wen Brunton. **Learning neural decoders without labels using multiple data streams.** bioRxiv, 2021.
- Steven M Peterson, Satpreet H Singh, Nancy XR Wang, Rajesh PN Rao, and Bingni W Brunton. **Behavioral and neural variability of naturalistic arm movements.** Eneuro, 8(3), 2021.

### Other datasets (to organize...)
Schneider, S., Lee, J. H., & Mathis, M. W. (2023). **Learnable latent embeddings for joint behavioural and neural analysis.** Nature, 1-9. https://doi.org/10.1038/s41586-023-06031-6
- Used synthetic spiking data from: Zhou, D., & Wei, X. Learning identifiable and interpretable latent models of high-dimensional neural activity using pi-VAE. Adv. Neural Inf. Process. Syst. https://proceedings.neurips.cc//paper/2020/file/510f2318f324cf07fce24c3a4b89c771-Paper.pdf (2020).
- Used spiking data from silicon probes in CA1 of rats: Grosmark, A. D. & Buzsáki, G. Diversity in neural firing dynamics supports both rigid and learned hippocampal sequences. Science 351, 1440–1443 (2016).
    - Data: https://crcns.org/data-sets/hc/hc-11/about-hc-11
    - Preprocessing script: https://github.com/zhd96/pi-vae/blob/main/code/rat_preprocess_data.py
- Used spiking data from Area 2 of S1 in rhesus macaque during a centre-out reaching task with a manipulandum: Chowdhury, R. H., Glaser, J. I. & Miller, L. E. Area 2 of primary somatosensory cortex encodes kinematics of the whole arm. eLife 9, e48198 (2019).
    - Data: https://gui.dandiarchive.org/#/dandiset/000127
- Used Allen Institute two-photon calcium imaging and Neuropixels data
    - Processed 2p data from: de Vries, S. E. et al. A large-scale standardized physiological survey reveals functional organization of the mouse visual cortex. Nat. Neurosci. 23, 138–151 (2019).
        - Data: https://github.com/zivlab/visual_drift/tree/main/data
    - Neuropixels data from the ‘Brain Observatory 1.1’ dataset: Siegle, J. H. et al. Survey of spiking in the mouse visual system reveals functional hierarchy. Nature 592, 86–92 (2021).
        - Data accessed via allensdk: https://allensdk.readthedocs.io/en/latest/visual_coding_neuropixels.html
- Code: https://github.com/AdaptiveMotorControlLab/CEBRA

Easthope, E., Shamei, A., Liu, Y., Gick, B., & Fels, S. (2023). Cortical control of posture in fine motor skills: evidence from inter-utterance rest position. Frontiers in Human Neuroscience. https://doi.org/10.3389/fnhum.2023.1139569
- Used ECoG data in NWB format from Figshare
    - Data: https://figshare.com/collections/Human_ECoG_speaking_consonant-vowel_syllables/4617263/4
    - Data also available at: https://dandiarchive.org/dandiset/000019
    - Data descriptor paper: Bouchard, K. E., and Chang, E. F. (2019). Human ECoG Speaking Consonant-Vowel Syllables. doi: 10.6084/m9.figshare.c.4617263.v4
    - Original scientific paper that used this data: https://www.nature.com/articles/nature11911
- Code: https://github.com/ericeasthope/as-in-ecog

## Education

### AJILE12 dataset (DANDI:000055)

Neuromatch Academy project
- Notebook: https://colab.research.google.com/github/NeuromatchAcademy/course-content/blob/main/projects/ECoG/exploreAJILE12.ipynb
- Notebook: https://github.com/neurovium/Neuromatch-AJILE12/blob/master/Notebook/exploreAJILE12.ipynb
- Code: https://github.com/neurovium/Neuromatch-AJILE12

## Unsorted

DANDI Notebooks collection
- https://github.com/dandi/example-notebooks

Example MATLAB Live Scripts collection
- https://github.com/INCF/example-live-scripts

MATLAB Live Script associated with:
Najafi, F., Elsayed, G. F., Cao, R., Pnevmatikakis, E., Latham, P. E., Cunningham, J. P., & Churchland, A. K. (2020). **Excitatory and inhibitory subnetworks are equally selective during decision-making and emerge simultaneously during learning.** Neuron, 105(1), 165-179.
- https://github.com/datajoint-company/najafi-2018-matlab

NWB Overview listing of data analysis and reuse examples
- https://nwb-overview.readthedocs.io/en/latest/community_gallery/community_gallery.html#data-analysis-and-reuse

SpikeForest
- https://elifesciences.org/articles/55167
- https://github.com/flatironinstitute/spikeforest
- Data also on DANDI: https://dandiarchive.org/dandiset/000618?search=spikeforest&pos=1

Processing and analysis tool benchmarking efforts

OpenScope Databook
https://alleninstitute.github.io/openscope_databook/intro.html

A non-scientist friend of Ryan's used Neuropixels spiking data from [dandiset 000053](https://dandiarchive.org/dandiset/000053) to make music.
