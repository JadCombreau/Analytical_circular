# ANANAX ANALYTICAL CIRCULAR
## Markdown documentation file
## Ananax2d_Analytical_Circular Workflow over Isight

| | CANONICAL | ANALYTICAL |
|-----------|:-----------:|:-----------:|
|INTAKE | -- | X |
|BYPASS | -- | X |

### Workflow type & role

This Workflow (__Analytical Circular__) has the final goal (*like the other Workflows*) the acoustic attenuation matrix calculus.
This Workflow is for canonical geometries, that is to say we do not have to generate any mesh. 

In numerical cases, ACTRAN automatically generates mesh supposed to be uniformed. In analytical cases, we don't have to create any mesh and we don't use ACTRAN solver but MADIWHAX solver. Sounds simple right ?

The air inlet duct is therefore assumed to be more or less uniform. We do not calculate any flow. There is no weighted average to be used for computation in various nodes of mesh.

__This Workflow therefore presents four boxes :__

![Canonical Workflow](https://user-images.githubusercontent.com/45098441/72733825-eddd6a00-3b98-11ea-9b77-2d24f6790d91.jpeg)
----------------------------


- __Initialization :__ *allows among other things the creation of initialization variables, environment variables or even structure test and the input XML file reading.*
- __Acoustic Models :__ *input file, thermodynamic file conditions (etc.)*
- __Acoustic Computations :__ *MADIWHAX solver for the noise acoustic calculation in the air intake/bypass (to obtain frequencies)*
- __Postprocessing :__ *allows the generation of the attenuation matrix (PIFF & PID calculus)*

### Initialization details :

#### The left side :

![Workflowleft](https://user-images.githubusercontent.com/45098441/72735505-3c403800-3b9c-11ea-9b80-446dedf0615e.jpeg)

#### And the right side :

![Workflowright](https://user-images.githubusercontent.com/45098441/72735511-3f3b2880-3b9c-11ea-9771-076188e4fe7a.jpeg)
