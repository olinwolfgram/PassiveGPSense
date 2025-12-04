# PassiveGPSense
Use android gnss logger coupled with CNN to detect the cardinal direction of a human target near receiver

record data with the android app GNSS Logger. download the files in the .24o filetype. ive attached the logs from my experiment.

For this analysis, you have to utilze the RINEX 3.0 version. since these logs are recorded with the 4.0 version, you have to convert the logs using the gfrnx converter tool (gfzrnx_linux_64) which ive included in this repo.

then you can run the script and getthe validation results.

i did these experiments at ~ 3-4 PM on top of an empty 6 story parking garage with minimal interference (except for multipath from the garage floor)
I was standing 0.5 meters away form the phone for each N, E, S, W cardinal direction, stood at each cardinal direction for 20 seconds. recorded four 10-minute logs where i would stand at each and move in the order N>E>S>W. 

my results proved the detector works (with 83% accuracy while using C/N0 metric). the pseudorange was slightly worse (~64%) but still well above the 25% random chance for guessing direction. All in all, gnss navigation data, speciifcally interference fluctuation metrics derived from it, can be used to detect the orientation of a user to an unmoving phone reciever. pretty cool.
