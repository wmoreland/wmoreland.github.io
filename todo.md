# qgis plugins with vs code and conda
  * conda and conda-build
  * make environment and activate
  * install qgis=3.34 (https://aneto.pt/posts/tutorials/2019-05-29-using-qgis-from-conda/)
    
  `conda install -c conda-forge/label/qgis_ltr -c conda-forge qgis`

  * run qgis from within environment (note that an error stating "Couldn't load SIP module" might appear when starting QGIS. I don't know how to fix this but deleting the environment and starting again can work!)
  * in qgis python console use sys.path and copy output
  * deactivate conda env and use conda-develop -n ENVNAME COPIED_PATH
  * voila qgis.core etc can be loaded

## tips
  * add variable QGIS_PLUGINPATH (append) to QGIS enivornment e.g. C:\Users\williammo\ONEDRI~1\Documents\GitHub\qgis-skjalftalisa
  * use shortnames to get around non-latin characters in path names... e.g. ONEDRI~1 
