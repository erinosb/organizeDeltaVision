# organizeDV
This script can be used to organize Deltavision Images. This is a pre-processing step for WormLib

# INSTALLATION 

<tbd>

# USAGE

**USAGE: bash organize_DV.sh [-h] [-d \<directory\>]**

| Option      | Value | Description    |
| :---        | :---      | :---   |
| -h      |        | Help. Print usage statement   |
| -d   | \<directory\>        | Default is working directory (.). Alternatively, specify the desired directory   |

This script takes as default input the current working directory.

Deltavision image files (_R3D.dv) and reference image files (_R3D_REF.dv) must be located within the current working directory or specified directory. File names must be specified like so:

  * N2_mRNA-1_01_R3D.dv
  * N2_mRNA-1_01_R3D_REF.dv
  * N2_mRNA-1_02_R3D.dv
  * N2_mRNA-1_02_R3D_REF.dv

 This script identifies all the R3D.dv and R3D_REF.dv files and organizes them into directories labeled Image_01, Image_02, etc.

OPTIONS:\\
 -h              Print usage statement\\
 -d <directory>  Default is working directory (.). Alternatively, specify the desired directory
