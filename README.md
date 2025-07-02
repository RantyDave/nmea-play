Plays back an NMEA log file over a TCP socket.

BUT, ALSO: Emulates the fact that NMEA is served over a 4800 bit/sec interface and delivers the lines at a sensible pace.
Where there is a ZDA record it creates an offset to real world time so the ZDA records are delivered at the correct time
ie 

    $IIZDA,081851,30,07,2005,,*59

will be served two seconds before

    $IIZDA,081853,30,07,2005,,*5B

And so on.
