# SMLM
Single Molecule Localization Microscopy Literature

## Segmentation
1. [Wavelet analysis for single molecule localization microscopy (2012)](https://www.osapublishing.org/oe/fulltext.cfm?uri=oe-20-3-2081&id=226621)  
This method is based on using a special wavelet transform called “à trous”. In this approach, each input frame is first decomposed into multiple wavelet planes. The first plane which contains very high frequency content is used for background estimation and the second plane which represents the coarser structure is used for spot detection and the rest of the planes are just discarded. The spot detection is realized by simply filtering the second wavelet plane with a threshold that is 0.5 to 2 times the standard deviation of the background.

2. [ThunderSTORM: a comprehensive ImageJ plug-in for PALM and STORM data analysis and super-resolution imaging](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4207427/)
ThunderSTORM provides three different options for segmenting the potentioal region of interests (ROI): selecting the bright pixels that are larger than a certain threshold in a local neighbourhood, morphological non-maximum suppression and a combination of the first method and the one in [1]. All of these three approaches are based on using a user defined threshold. 

## Localization
[Working principle of other localization algorithms (2014)](https://aip.scitation.org/doi/full/10.1063/1.5005899)
