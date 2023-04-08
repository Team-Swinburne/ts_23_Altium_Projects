# About

A Github repository by Team Swinburne for pcb development of the TS_22 vehicle and experimental projects. This will only contain files of the actual pcb design, more information such as design choice, circuit theory, simulation, etc can be located in the shared Pne Drive

# Getting Started

### Prerequisites
- [Altium](https://www.altium.com/solutions/academic-programs/student-licenses) (required): Used to design all of these pcb, fill in the link for a free student license.
- [Git](https://git-scm.com/) (required) : Backbone of Github.
- [Github Destop](https://desktop.github.com/) (recommended) : An UI overlay of git built specifically for Github so you don't have to deal with the terminal interface.

### Installation
Once all prerequisite are install, clone this repository to your desired folder by opening it in Github Desktop
![image](https://user-images.githubusercontent.com/28666595/124406100-b7db7800-dd83-11eb-99b1-a74507a78a47.png)

# Usage
Follow this guide to ensure you meet the standard and is set up probably before diving into create your own pcb

### Naming
**Always** name your project strictly following the naming scheme to avoid confusion in the future. When starting a new board, create a new folder name `ts_22-"Board name"`. Then inside that folder, create a project in Altium called `YYMMDD "Board name" "Revsion number"`
#### For example:
> ts_22-Brake-Module
>
Then:
> 210705 Brake Module R0
> 
`YYMMDD` is the project's createtion date and `Revision number` starts with 0. 
#### Note: Once the pcb is made, **DO NOT** make any changes to that revision, modifying **MUST** be made by starting a new revision, e.g. R1

### Importing libraries
Altium libraries are collections of component intented for speeding up the design and manufacturing process. There are 2 libraries used in PnE: *ts_22-standard-lib* and *ts_22-connectors-lib*, located in the *~ts_22 Library*.

To import them: In Altium with your project opened, right-click on the project name -> Add Existing -> Choose file `"library name".DbLib`, do this for both libraries.

![image](https://user-images.githubusercontent.com/28666595/124409177-2a038b00-dd8b-11eb-9ef3-1194a9db3896.png)

Guide on how to add components into the library will be made available in video from. Please discuss with your section leader before attempting to modify these library.

### Importing design rules
Design rules ensure all pcb meet Team Swinburne standards and more importantly, the competition rule. There are 2 sets of rules: *ts_22-rules.RUL* and *ts_22-HV-rules.RUL*. Choose the corresponding rule dependent on which board you are working on.

To import: In Altium with your project opened, choose Design -> Rules. Then in the pop-up windows, right-click on Design Rules -> Import Rules -> Select all entries -> OK -> Choose file `"rules name".RUL`.

![image](https://user-images.githubusercontent.com/28666595/124417041-a605cf00-dd9b-11eb-9976-f45a026aab0f.png)
