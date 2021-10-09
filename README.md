# AltiumManufacturingAndDRC
Altium OutJob file for generating gerbers, PNPs, etc. Also includes Rules file for JLC, Oshpark

How to use Altium Outjob file for generating manufacturing documents:
1. Download Outjob file + drag and drop into project folder. Then right-click on the project >> add existing files to project (Make sure Outjob file appears under)
2. Project Releaser. Right-click on project >> Project Releaser. Click details on Source data to ensure the Outjob file has been recognized.
    i. Make sure to disable PLM. right-click project >> PLM >> uncheck enabled
    ii. Choose target folder for output files. In project releaser >> Options >> Output Path
    iii. If Outjob file not immediately recognized, go to Options (in project releaser) >> Release Options >> ensure RPLExports is checked for Source data
3. Hit Prepare. Then review and export all files. They should appear where specified in the output path.

Configuring a DRC using JLC/Oshpark Rules file
