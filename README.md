# get_ooi_csv
Matlab script to retrieve and concatenate data files from OOI.

The starting point for this script is the download link sent from noreply@oceanobservatories.org in response to a csv data request. The link should be pasted into the appropriate spot near the top of the script, and the 'choice' variable set to 1 for text or 2 for numeric output. The text option is faster but results in much more RAM usage.

Currently, the code pre-allocates space for 3.5 million rows of data (with number of columns determined by the type of data). This can be increased, by setting numRows to the desired number.

Note that this script has undergone only minimal testing with data from TRHPH, so it is not known whether it will work with data from other OOI instruments.