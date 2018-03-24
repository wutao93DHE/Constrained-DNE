# Constrained-DNE
High-efficient extraction of drainage networks from digital elevation model data constrained by enhanced flow enforcement from known river maps

This program is used for drainage network extraction from DEM data, based on the least-cost-search algorithm realized using a size-balanced-binary-tree (see the reference below) to speed-up computation, improved with a channel head recognition method using a geomorphologic change point detection algorithm (which is pursuing pulication in the journal of Computers & Geosciences) to provide an alternative for the existing Critical-Sourcing-Area (CSA) method.

### Usage

A compiled Windows exe file can be found in the /Sample folder.
The program runs in the command line mode. 
There are five input parameters in all, including the compulsory DEM_data_file_path and four optional parameters that must be provided togethor.

    DNE.exe DEM_data_file_path [Critical_S_Sqrt_A Critical_A_over_Sq_L Window_Shift_Proportion Confidence_p_Value]
    
    examples:
    DNE.exe Sample.tif
    DNE.exe Sample.tif 25 0.2 0.25 0.05


The program will create a folder named same as the inputed DEM file and save the result file in it. Both of the input DEM and result data are in the uncompressed TIFF format, the samples can be found in the /Sample folder, and is shown as follows.
