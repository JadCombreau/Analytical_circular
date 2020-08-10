## Link Data From Numacous
### Script Language

All the __Link Data From Numacous__ box is written in __Shell UNIX__ language.
### What the box does ?

This script allows data copy from the Numacous directory to our Job folder.
For this, the scripts will process all the following files, created previously :

- ACOUSMESH
- INTERPOLMESH
- MICROPHONES
- INPUTS
- INFO
- FLOW
- FLOWMESH
- SCOUT

The input XML file previously nammed *"input.xml"* will be copied and renamed *"previous.xml"* in our Job folder.

*__Link Data from Numacous__ box is followed by the __Build Paths__ box which consist in the creation of different file paths (necessary for all the Workflow)*.

![Initialization components](https://user-images.githubusercontent.com/45098441/86895761-3e279480-c105-11ea-9a34-5aedfb4b2582.JPG)


----------------------------

### What about variables ?

The table below lists all the variables to be created in Isight and their role :

__Inputs variables to be given to Isight or received from previous boxes :__ 

| Variable Name | Variable description | Type | Input | Output |
| ------ | :------------: | :------: | :------: |  :------: |
| pathOfJobFolder | Job folder path (to copy all workflow results) | STRING | X | - |
| pathOfNumacousFolder | Numacous folder path | STRING | X | - |

