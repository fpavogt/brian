.. _changelog:

Changelog
=========

TODO:
 - allow for more stellar templates.
 - add the reference to the LOWESS paper in the acknowledgment.
 - add the reference to the stellar templates in the acknowledgments.
 - in the fit inspection tool, know if ppxf or lowess is used for continuum subtraction.

v0.1.1, April 2016, F.P.A. Vogt:
 - replaced '0.1' with '__version__' when saving fits headers
 - separated the continuum fitting from the construction of the continuum data cube, for
   clarity and consistency with the emission lines
 - added local copy of mpfit as brian_mpfit.py for portability
 - refined plot legends and colorbar ticks
 - started catching numpy warnings in known locations, triggered by all-nan's spaxels
 - implemented a dictionary of created filenames (in brian_metadata), to better keep track 
   of what is created, with much less hard-coded filenames
 - added home-made "alligator" colorbar for that special look (and also to show nan's and
   spaxels that land at the edges or outside a colorbar range for a given plot)
 - connected brian to ppxf
 - defined structure of the docstring, to be used through brian, in brian_cof.lowess_fit
 - added interactive plot to inspect the results of the fit - and the ability to save a
   pretty plot from it.
 - bugfixes
 
v0.1.0, April 2016, F.P.A. Vogt:
 - created overall code structure inspired by pywifes
 - implemented continuum fitting using LOWESS approach
 - implemented modular emission line fitting via mpfit
 - added safety measures to catch KeyboardInterrupt during multiprocessing tasks.
 - created preliminary documentation structure 
 - initial upload to Github
 - added license info
 - added semi-automatic detection of structures, and ability to interact to add/remove
   apertures of varying radii
 - added creation of "aperture spectra cube" based on a given aperture list