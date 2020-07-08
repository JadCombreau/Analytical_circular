## Copy Init
### Script Language

All the __Copy Init__ box is written in Shell UNIX language.
### What the box does ?

 This aim Shell script box is to copy folders from our Job folder (after modifications by previous boxes) into the Numacous folder.

*__Copy Init__ box is preceded by the __Scenario Analyser__ box (this box makes it possible to test if files or directories do not exist and therefore to determine which configurations or frequencies to restart) and followed by the __Update Monitoring__ box (allows to update the status of the workflow and to pass the finished parts in "completed")*.

![Initialization components](https://user-images.githubusercontent.com/45098441/86895763-3f58c180-c105-11ea-8479-db334e3fee42.JPG)

----------------------------


### Which files to import ?

To execute the script __Copy Init__ correctly, we need to import Python libraries.
The table below lists all the imports to be made :

| Import name | Import location |
| ------ | ------ |
| CopyNumacous_Init.py | `/src_wf/python/workflows/ductnoise/common` |

### What about variables ?

The table below lists all the variables to be created in Isight and their role :

__Inputs variables to be given to Isight or received from previous boxes :__ 

| Variable Name | Variable description | Type | Input | Output |
| ------ | :------------: | :------: | :------: |  :------: |
| nameOfComponent | Name of Results Components folder | STRING | X | - |
| verbosity | Verbosity schema value | STRING | X | - |
| pathOfInputXML | Input XML file path | STRING | X | - |
| pathOfJobFolder| Job Folder path (to copy all workflow results) | STRING | X | - |
| pathOfLogsFolder | Name of Results Logs folder | STRING | X | - |
| pathOfNumacousFolder | Numacous folder wich contain all data to update | STRING | X | - |
| pathOfTools| Tools Folder path | STRING | X | - |
