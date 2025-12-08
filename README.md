# organizeDV
This script can be used to organize Deltavision Images. This is a pre-processing step for WormLib

# INSTALLATION 

To obtain the code, use git clone to sync a copy of organizeDV to your local directory:

```bash
$ git clone https://github.com/erinosb/organizeDV.git
```

Navigate into the obtained directory:

```bash
$ cd organizeDV
```

Use **chmod** to make the script organizeDV executable:

```bash
# Check that you are located within the organizeDV directory:
$ pwd
~/your/file/structure/organizeDV

# Check that you can see the organizeDV script listed in your working directory:
$ls -alh
organizeDV
README.md

# Change your permissions to allow execusion by the user:
$ chmod +x organizeDV

# Check that permissions are changed:
$ ls -alh organizeDV

```

Now, the script can be executed using the syntax: `./organizeDV` from within the directory where it is located. It should be denoted with an x in the permission code. 

To make the organizeDV script executable from anywhere in your file structure, you will need to add its working directory to your $PATH. Please understand this process before you change your $PATH.




<tbd>

# USAGE

**USAGE: organize_DV.sh [-h] [-d \<directory\>]**

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

```bash

USAGE:
     organizeDV [ -h ] [ -d <directory> ]

OPTIONS:
     -h              Print usage statement\\
     -d <directory>  Default is working directory (.). Alternatively, specify the desired directory
```

# KNOWN BUGS

  * Please be aware that if your files do not increment perfectly, the Image_## folder number and the actual image number can move out of sync. If you would like to use the image file name to designate the folder name, please contact Erin Nishimura. This can be added.

# FUTURE EXPANSION

Ideas for future expanstion will go here.



