#Workspace renamer for BD Influx running Sortware v1.2.0.142

Copyright (c) 2017 Genome Research Ltd.

Author : Christopher Hall, Wellcome Trust Sanger Institute, christopher.hall@sanger.ac.uk

http://www.sanger.ac.uk/science/groups/cytometry-core-facility


BD Sortware for the Influx names all its files with non-descriptive names, however it can read any name a file has.  When backing up and cleaning our PC we run this script to rename the workspace.xml files to the descriptive name as seen in Sortware itself.

This script renames all XML files in its folder and subfolders to the 'name' tag of the file.  
####DO NOT do this on your working workspace directory.  Make a copy of it and do it there.

##INSTRUCTIONS
This script uses Python V3.
Place the .py file into the top folder of your saved workspaces, which can be found in the BD folder.
Run the script.
The script will then rename all the files form workspace1.xml to whatever is in the 'Name' tag in the xml file.  
If you have 2 files with the same 'name' tag then the script willa dd a random number to prent overwriting.
Windows filenames cannot contain any of the following charactors [\\/*?:"<>|] If yours does then it will be replaced with a -
 