# SMLM
Single Molecule Localization Microscopy Literature

## Segmentation
1. [Wavelet analysis for single molecule localization microscopy (2012)](https://www.osapublishing.org/oe/fulltext.cfm?uri=oe-20-3-2081&id=226621)  
This method is based on using a special wavelet transform called “à trous”. In this approach, each input frame is first decomposed into multiple wavelet planes. The first plane which contains very high frequency content is used for background estimation and the second plane which represents the coarser structure is used for spot detection and the rest of the planes are just discarded. The spot detection is realized by simply filtering the second wavelet plane with a threshold that is 0.5 to 2 times the standard deviation of the background.


## Localization
(Working principle of other localization algorithms)[ftp://ftp.aip.org/epaps/journ_chem_phys/E-JCPSA6-148-013898]
