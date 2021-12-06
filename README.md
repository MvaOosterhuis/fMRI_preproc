# fMRI_preproc

fMRI EPI preprocessing pipeline which computes and applies a set of transformation using AFNI such that the EPI dataset ends up living in the space of a high-resolution anatomical dataset, imports that transformed dataset into a mrVistaSession which is ready to use with the vistalab vistasoft software. This package also contains novel existing code that was (slightly) modified to fit the current pipeline.

**Existing codebase used in this project include:**

r2aGUI (https://github.com/jeddobson/par_convert/blob/master/r2agui.m).

vistasoft (https://github.com/vistalab/vistasoft)

**These functions were built to use AFNI version AFNI_19.0.21, and cannot be guaranteed to work with newer versions of AFNI.**

Open EmptyStartfile.m, fill in the relevant fields and press play.

**N.B. make sure that all data to be preprocessed contains AT LEAST the following components and follows the directory-tree structure specified below:**

EPI-data, t1-matched data (t1 scanned in the same resolution/FOV/orientation as the EPI), and a high-resolution anatomical dataset that can be in any orientation.

ProjectDirectory/Participant/Session/datafiles_as_Stated_Above

Allows for participant and session batch processing if structured appropriately
