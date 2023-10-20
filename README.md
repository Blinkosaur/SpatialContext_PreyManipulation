# SpatialContext_PreyManipulation

Our aim was to assess the impact of spatial context on prey manipulation in the California moray eel (*Gymnothorax mordax*), a crevice forager with a diverse prey handling repertoire. We first compared the duration engaged in specific manipulation behaviors between spatially “enclosed” and “open” foraging environments (Experiment 1), followed by a comparison of tightly enclosed spaces that were scaled to individual moray diameter (Experiment 2). 

Project Folders:

data - contains all data files for this project
  Phase1-SpatialContext.csv --> data from Experiment 1; Enclosed vs Open spatial treatments
  Phase2-SpatialContext2.csv --> data from Experiment 2; Diameter-based enclosed treatments
  Phase2-SpatialContext+Open.csv --> data combining aspectso of Experiment 1 (open treatment) with Experiment 2 treatments 
  Rotation_Complete.csv --> rotation speed data 
      *see notes below about column names*
  
docs - contains: index.html --> rendered quarto doc containing code and descriptive text as html 

images - contains images of experimental apparati as well as illustrations of prey handling behaviors, which are overlaid onto graphics within the code

reports - contains:
  index.qmd --> quarto document containing all code and descriptions 
  All graphics in manuscript made by the code 

---------------------------------------
Column Names & Content Descriptions:
---------------------------------------
  - Phase1-SpatialContext.csv
      Trial info --> order of treatment presentation
      Treatment --> Spatial Treatments; Open, 10cm, 5cm 
      Eel --> name of individual 
      Trial_Duration --> total time feeding in seconds
      Handling_Dur --> total time manipulating prey in seconds
      Bites --> number of bites
      Ptransport_Dur --> total time spent swallowing in seconds
      Ptransport_Prop --> proportion of the total trial time spent swallowing
      Knotting_Binomial --> yes/no if knotting was observed in the trial

All manipulation behaviors (shaking, ramming, rotating, knotting) have three columns; total duration of behavior in seconds, proportion of the behaviour out of the total feeding time, and proportion of time in the behavior out of the total handling duration. For example, shaking has three columns: Shaking_Dur (total time), Shaking_Prop (out of feeding time), and Shaking_Prop_Handling (out of handling time). 

- Phase2-SpatialContext2.csv *many columns are the same as previous, or contain the same type of information; only new columns are listed here*
    Treatment_Round --> contains information about the number of exposures to the treatment
    [behavior]_freq --> the _freq suffix denotes frequency data; # of instances a behavior was observed during a trial

    Two new behaviors are included:
        crinkle_ -->  referred to as body anchoring in the text
        anchor_ --> referred to as tail anchoring in the text
        tug_ --> not included in analysis as this behavior could not be seperated fully from other behaviors 

- Phase2-SpatialContext+Open.csv
    Contains columns from previous data files

- Rotation_Complete.csv
   Rotation_Bout --> within a trial there could be multiple bouts of rotating; these were numbered 1 - n 
   Rotation_Duration --> total length of time in a rotation bout in seconds
   Opercular_Passes --> number of instances the opercular opening passes by the field of view
   Opercular_Passes.2 --> Opercular_Passes divided by 2
   Rotation_Second --> rotations per second
   Log_Rotation_Second --> log transformed Rotations/Second



