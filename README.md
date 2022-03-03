import panel as pn
from bokeh.resources import INLINE

SimpleTable = pn.panel("""
<style>
table, th, td {
  border: 1px solid black;
}
</style>

# Branch Master (main code)

## Requirements 
(check the CMakeLists.txt and src/CMakeLists.txt)
<ol>
<li>CGAL (>= 4.11.2)</li>
<li>  g++ </li>
<li> maxhs  </li>  *check the installation instruction and detailed information: http://www.maxhs.org/
</ol>

## Installation
Compile the source with the build/build_auto.sh

## JEA_RCR Test
Run test.sh (the results will be stored in folder OUTPUT as json files.)

# Branch dynamis_jea_plots (plots generator)
## Requirements
check the requirements.txt file
## JEA_RCR Test
Run plotting.sh
## Evaluation
For each set of experiements, we set up a folder as follows. Each of the folders 
contains one subfolder "plots", which contains the generated plots of its corresponding experiment set.
To compare the generated plots with plots presented in the papar, please refer to the following table.



|     Time    | Number of Trial with Results | Unique Units |
|:-----------:|:----------------------------:|:------------:|
| 20 Apr 2018 |            30,763            |    21,094    |
|  7 Feb 2019 |            34,751            |    23,733    |
| 12 Apr 2019 |            35,926            |    24,548    |
|             |                              |              |

""")
E1:
E1-Rect
E23
E23-Rect
E4
E4-Rect
E5
E5-Rect



**NOTE**


The benchmark data files (in the folder INPUT) were generated with the https://github.com/dyna-mis/labeling-instance-generator. 
However, since the two rectangle files are lost, we generate two new files with seed 0. 
The computed results are slightly different, however the generated plots have semiliar pattern as the one in our paper. 

 
