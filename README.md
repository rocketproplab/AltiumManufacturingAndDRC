# AltiumManufacturingAndDRC
Altium OutJob file for generating gerbers, PNPs, etc. Also includes Rules file for JLC, Oshpark

How to use Altium Outjob file for generating manufacturing documents:
1. Download Outjob file + drag and drop into project folder. Then right-click on the project >> add existing files to project (Make sure Outjob file appears under)
2. Project Releaser. Right-click on project >> Project Releaser. Click details on Source data to ensure the Outjob file has been recognized.
    i. Make sure to disable PLM. right-click project >> PLM >> uncheck enabled
    ii. Choose target folder for output files. In project releaser >> Options >> Output Path
    iii. If Outjob file not immediately recognized, go to Options (in project releaser) >> Release Options >> ensure RPLExports is checked for Source data
3. Hit Prepare. Then review and export all files. They should appear where specified in the output path.
4. For Uploading to JLC:
    i. In the NC Drill Files folder that was created, rename the .txt file to .xln
    ii. Take all generated gerber files (GTL, GTS, etc.) and the .xln drill file and upload those to JLC in a zipped folder
More info:
https://www.altium.com/documentation/altium-designer/working-with-the-project-releaser-ad

Configuring a DRC using JLC/Oshpark Rules file:
0. Download Rules file to project folder
1. Design >> Rules
2. Right-click on Design Rules folder on the left side >> Import Rules
3. Ctrl A to select all rules. Hit Next
4. Select Rules file
5. Hit Yes to clear all existing rules. The DRC should now be configured for JLC/Oshpark
More info:
https://www.altium.com/documentation/knowledge-base/altium-designer/import-or-export-design-rules
