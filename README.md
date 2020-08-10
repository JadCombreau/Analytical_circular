# ANANAX ANALYTICAL CIRCULAR
## Initialization details :
### The aim of this box :
*Allows among other things the creation of initialization variables, environment variables or even structure test but also the input XML file reading.*

### The Composition :

- __Set ANANAX Environment and Resources PATH :__ *allows to source the variable environment necessary for the execution of the various workflows scripts (cdng_ananax_home.tmp)*
- __Reference to init_v2019r1 :__ *allows the initialization of the different paths and the construction of the paths for each execution (for each frequency of each configuration through the JobID)*
- __Create Folders :__ *allows initializing an array containing the various Isight variables (containing repository names) then the creation of these different folders*
- __Check & Read XML :__ *input XML verifiying and reading (we get here all the parameters we will need for the rest)*
- __Link Data From Numacous :__ *allows data copy from the Numacous directory to our Job folder*
- __Build Paths :__ *allows the creation of different file paths necessary for all the Workflow (particularly in the Scenario Analyser)*
- __Scenario Analyser :__ *allows you to test if there are missing folders/files after the first execution of the Workflow*
- __Copy Init :__ *this aim Shell script box is to copy folders from our Job folder (after modifications by previous boxes) into the Numacous folder*
- __Update Monitoring :__ *allows to update the status of the Workflow and to pass the finished parts at "completed". It allows to modify the XML file directly (using of the Python language DOM API - Document Object Model)*

### The left side :

![Workflowleft](https://user-images.githubusercontent.com/45098441/86895578-f99bf900-c104-11ea-886b-6301fba9bf44.JPG)

### And the right side :

![Workflowright](https://user-images.githubusercontent.com/45098441/86895580-fa348f80-c104-11ea-932e-a843720f7c14.JPG)
