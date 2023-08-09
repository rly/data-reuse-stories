# data-reuse-stories
Examples of reuse of publicly accessible neurophysiology datasets 

## A survey
de Vries, S. E. J., Siegle, J. H., & Koch, C. (2023). **Sharing neurophysiology data from the Allen Brain Observatory.** eLife, 12, e85550. https://doi.org/10.7554/eLife.85550

See the above paper for a comprehensive review of examples of reuse of Allen Brain Observatory data prior to publication (July 2023) for:
1. scientific discovery
2. validation of models and algorithms
3. comparison with other datasets
4. education

I may summarize those examples here in the future.

## Papers
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

Nguyen, D. T., Nguyen, M. D. T., Hy, T. S., & Kondor, R. (2023). **Fast Temporal Wavelet Graph Neural Networks.** arXiv preprint arXiv:2302.08643. https://arxiv.org/abs/2302.08643
1. Used AJILE12 dataset (DANDI:000055) - specifically, one hour of recording from subject id 5.
    1. Data descriptor paper: https://www.nature.com/articles/s41597-022-01280-y
    2. Data on DANDI: https://dandiarchive.org/dandiset/000055
3. Data was used to evaluate the authors' proposed model, FTWGNN, against other models. The authors found that:
    1. FTWGNN outperforms other models by most metrics
    2. FTWGNN performs well at 1-second prediction, but produces unstable and erroneous forecasts for steps of 5 or 15 seconds
    3. FTWGNN is faster than DCRNN by at least 2X
