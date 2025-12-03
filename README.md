# PassiveGPSense
Use android gnss logger coupled with CNN to detect the cardinal direction of a human target near receiver

record data with the android app GNSS Logger. download the files in the .24o filetype. 

For this analysis, you have to utilze the RINEX 3.0 version. since these logs are recorded with the 4.0 version, you have to convert the logs usinf the gfrnx converter tool (gfzrnx_linux_64).

then you can run the script and getthe validation results.

i did these experiments at ~ 3-4 PM on top of an empty 6 story parking garage with minimal interference (except for multipath from the garage floor)
