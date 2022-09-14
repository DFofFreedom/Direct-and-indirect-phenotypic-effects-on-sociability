README


These 6 data files (each of the .csv files) are knitted together by the R script (the .R file) to create the analysis file and figures for the paper "Direct and indirect phenotypic effects on sociability indicate potential to evolve"

roach_tags_dryad.csv - csv file with the id number ad tag identifier for eac cockroach. Used for combining the sociability scores with the social networks
id - unique id of each cockroach
colour - two digit code indicating the two colours (left right respectively) that marked the wings of the cockroach to allow vidual identification. R = red, B = blue, W = white, G = green, X  = gold
box - box number for the cockroach, ranges from 1-4
id_box - concatenation of colour and box to generate a unqiue identifier, as colours were re-used between boxes


roach_trials_dryad.csv - csv file describing which roaches were in which box, under which acamera, and with which patners f reac trial. Also includes partner mass and (when it was measured) focal mass)
date - date the trial took place
box - the box the cockroach was trialed in (ranges from 1-24)
id - the unique id of the focal cockroach
partner - the unique id of the partner cockroach
mass_id - the mass (in g, to 2 decimal places) of the focal individual
mass_partner - the mass (in g, to 2 decimal places) of the partner individual
camera - the identifying code of the camera the trial was filmed by (11, 12, 13, or 14)


roach_trial_info_dryad.csv - csv file contaiing basic information about the trials in eac day, including temperature.
date - date the trial took place
start time - start tie of the trial
end time - time when I ended the trial, in some cases this is longer than the alloted time but this extra time was ignored and never analysed.
start temp - starting temperature of the trial
end temp - temperature at the end of the trial

roach_assocs_dryad.csv - csv file contaiing records of the co-use of shelters by the cockroaches, used to build the social networks 
date - the date of the observation
box - the box number of the cockroaches, ranges from 1-4
shelter - the shelter number within a given box, ranges from 1-4
indiv - two digit code indicating the two colours (left right respectively) that marked the wings of the cockroach to allow vidual identification. R = red, B = blue, W = white, G = green, X  = gold
group - unique identifer for the group each cockraoch was foud in for eac observation, made by concatenating date, box, and shelter (concatenated in Excel hence the odd format of the date)


roach_origins_dryad.csv - csv file containing the sex and stock box of origin of each cockroach
id - unique id of each cockroach
sex - sex of the individal, either "f" (female), or "m" (male)
origin - stock box the cockroach was taken from, either Sb1, Sb2, Sb4, or Sb5 for females, or Mb1or Mb2 for males
notes - notes describing which cockroach that died this one replaced

roach_video_dryad.csv - records from the video of the location of the focal cockroach in each trial
date - date the trial took place
camera - the identifying code of the camera the trial was filmed by (11, 12, 13, or 14)
time - the time of the observation
box - the box the cockroach was trialed in (ranges from 1-24)
loc - the location of the cockroach's head for that observation, ranges from 0 (on th edividing mesh) or 8 (the opposite end of the box to the partner individual)
notes - notes indicating whether the mesh divider was breached (crossed) by either the focal ("breached") or partner ("breached by partner") individual. No location recorded for this time point or the rest of the trial


Fisher_Code_for_Roach_Soc_R_and_Psi_for_Dryad.R - R code for the analysis and construction of figures and tables

Loads pacakges, sets working directory (user will need to enter own file directory) and then should be worked through in order.

