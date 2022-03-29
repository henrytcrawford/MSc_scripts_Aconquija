# aconquija_scripts
 Python scripts for Sierrra de Aconquija age calibration model. Includes BCET code, Raster Statistics, SPOT sampling, and Spectral analysis. All code is a work in progress.  
- Data outputs are saved locally one directory level up, outside of Git repository in 'outputs'. 
- Spot Sampling requires input multiband raster file (use BCET code for pre-processing), and a polygon vector file. Pixel statistics are extracted and calculated for each polygon, and appended to a table. Resulting spectral profles for each polygon are plotted.  
- The Pixel Mean Statistics code uses spot sampling and first derivative calculations to identify the minimum number of pixels needed to achieve a stbalized spectral refelctance mean, for each band. 
- PCA codes run Principle Component Analysis on the output of the Spot Sampling statististics. This code identifies patterns of varibility in the spectral dataset (i.e. spot sampling output) as it realtes to surface age. 
- Subsequent code regresses Principle Components with cosmogenic-nuclide absolute ages, and paleoclimate records. 
- This code is made publc as an open-science effort. Please do not submit pull requests as code is disorganized and a work in progress. 
