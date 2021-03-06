# SMLM
Single Molecule Localization Microscopy Literature

## Segmentation
1. [Wavelet analysis for single molecule localization microscopy (2012)](https://www.osapublishing.org/oe/fulltext.cfm?uri=oe-20-3-2081&id=226621)  
This method is based on using a special wavelet transform called “à trous”. In this approach, each input frame is first decomposed into multiple wavelet planes. The first plane which contains very high frequency content is used for background estimation and the second plane which represents the coarser structure is used for spot detection and the rest of the planes are just discarded. The spot detection is realized by simply filtering the second wavelet plane with a threshold that is 0.5 to 2 times the standard deviation of the background.

2. [ThunderSTORM: a comprehensive ImageJ plug-in for PALM and STORM data analysis and super-resolution imaging (2014)](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4207427/)  
ThunderSTORM provides three different options for segmenting the potentioal region of interests (ROI): selecting the bright pixels that are larger than a certain threshold in a local neighbourhood, morphological non-maximum suppression and a combination of the first method and the one in [1]. All of these three approaches are based on using a user defined threshold. 

3. [Imaging Intracellular Fluorescent Proteins at Nanometer Resolution (2006)](https://science.sciencemag.org/content/313/5793/1642)  
In PALM, first all frames are subtracted from a dark state frame to convert EMCCD detector counts to photons. Then, subsequent frames are subtracted from each other to yield bright spots as fluorescent molecule candidates. Finally, spots that their photon count in a neighbourhood of 2.5\*PSF is larger than five times the mean of the shot noise from the background are kept for the next steps.

4. [Sub-diffraction-limit imaging by stochastic optical reconstruction microscopy (STORM) (2006)](https://www.nature.com/articles/nmeth929)  
The segmentation step in STORM imaging is based on spatio-temporal filtering of each recorded frame. Candidate regions of size 13x13 pixels are kept based on 3 criteria: They should be on for at least 3 frames, the elipticity of the 2D fitted Gaussian should be smaller than a certain threshold and the total number of photoelectrons in the ROI should be larger than 2000.  

5. [Probability-based particle detection that enables threshold-free and robust in vivo single-molecule tracking (2015)](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4710236/)  
They incorporate the prior knowledge of camera noise model, PSF and experiment conditions into a statistical framework. In this framework, the probabiliy of a true positive pixel (pixel with intensity from the fluorescent molecules) is computed by comparing the foreground and background likelihood model. The main features of this approach is that it is thereshold-free and it provides the minimum number of false-negative at a fixed number of false positives. 

## Localization
[Working principle of other localization algorithms (2014)](https://aip.scitation.org/doi/full/10.1063/1.5005899)

1. [Center of mass]()  

2. [Radial symmetry](https://www.nature.com/articles/nmeth.2071)

3. [Gaussian fitting]()

4. [Computational correction of spatially variant optical aberrations in 3D single-molecule localization microscopy (2019)](https://www.osapublishing.org/oe/abstract.cfm?uri=oe-27-9-12582)  
This approach is based on fitting full vectorial PSF model to the segmented spots (ROI)
