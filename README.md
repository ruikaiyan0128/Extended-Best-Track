# Extended-Best-Track
Extended Best Track Data, source: http://rammb.cira.colostate.edu/research/tropical_cyclones/tc_extended_best_track_dataset/


Description of the Extended Best Track File
             (ebtrk_atlc.txt)
             (ebtrk_epac.txt)
       Version 2.03   Aug 06, 2015

Based on NHC Atlantic HURDAT Downloaded Aug, 15 2012
East Pac HURDAT Downloaded Aug, 15 2012

2012 cases from ATCF b-decks
2013 cases from ATCF b-decks
2014 AL cases from ATCF b-decks

Currently Supported by NESDIS/RAMMB and CIRA


         Previous project contributors

               Mark DeMaria
NESDIS/StAR/Regional and Mesoscale Meteorology Branch
       CIRA/Colorado State University
            West Laporte Avenue
           Fort Collins, CO 80523

 with contributions from
Jeremy Pennington and Krislyn Williams
formerly of the
Tropical Prediction Center/National Hurricane Center
11691 SW 17th Street
  Miami, FL 33165

The National Hurricane Center (NHC) maintains a climatology of all
Atlantic tropical cyclones since 1851. For each storm, the data file contains
estimates of the latitude, longitude, 1-minute maximum sustained surface
winds, minimum sea-level pressure, and an indicator of whether the system
was purely tropical, subtropical or extra-tropical at 6-hour intervals.
This data set is sometimes referred to as HURDAT.  One limitation of the
HURDAT file is that it does not contain any information about the storm
size. As part of the operational forecasting procedure, NHC routinely
estimates the radii of 34, 50 and 64 kt winds, the radius and pressure of
the outermost closed isobar, the radius of maximum wind, and the diameter
of the storm eye, if one exists. Under original support from the Risk
Prediction Initiative, this operational data for the period 1988-1997 was
digitized and combined with the information from the HURDAT file.
Although the RPI project was completed in 1999, the file is updated by NESDIS/ORA
for development of satellite algorithms, using data supplied by NHC personnel.

Version 1.0 - Feb 1998 - All variables for 1990-1997
Version 1.1 - Apr 1998 - All variables for 1988-1997
       except max wind radii for 88-89
Version 1.2 - Feb 1999 - All variables for 1988-1997
Version 1.3 - Apr 2000 - All variables for 1988-1999
Version 1.4 - Mar 2001 - All variables for 1988-2000
Version 1.5 - Apr 2003 - All variables for 1988-2002,
       updated NHC best track file 1988-2002 used,
which includes category 5 upgrade of Andrew 1992
Version 1.6 - Feb 2004 - All variables for 1988-2003
Version 1.7 - Mar 2007 - All variables for 1988-2006
       All changes to HURDAT as of March 2007 included.
       34, 50 and 64 kt wind radii since 2004 are from NHC best track.
       NHC began creating best track wind radii in 2004;
       radii from 1988-2003 are still the operational radii.
       An east Pacific extended best track was added in
          version 1.7 called ebtrk17_epac.txt. It includes
          the years 2001-2006.
version 1.8 - Feb 2008   Cases from 2007 season added.
version 1.9 - May 2009   Cases from 2008 season added.
       Some missing data from tropical storm Zeta (2005-06) added
       Storm numbers from 1997 modified for consistency with
          NHC numbering convention
       Minor changes to HURDAT since 2008 incorporated
version 1.10 - Nov 2010  Cases from 2009 season added.
version 1.11 - Jun 2011  Cases from 2010 season added.
version 2.00 - Aug 2012  Cases from 2011 season added.
       New field added to end of record showing distance to
       nearest major landmass (km).
version 2.01 - Feb 2013  Cases from 2012 season added.
version 2.02 - Feb 2014  Cases from 2013 season added.
version 2.03 - Aug 2015  AL Cases from 2014 season added


Note:  If you need to refer to the extended best track file in a publication,
a very brief description can be found in the following paper:

Demuth, J., M. DeMaria, and J.A. Knaff, 2006: Improvement of advanced
microwave sounder unit tropical cyclone intensity and size estimation
algorithms. J. Appl. Meteor., 45, 1573-1581.

The radius and pressure of the outer closed isobar and the radius
of maximum wind were not routinely estimated as part of the NHC
operational forecast procedure prior to 1990. The outer closed isobars
and pressures from 1988-89 that were added in version 1.1 were estimated
from the tropical surface analyses which were prepared operationally
by NHC. These surface analyses were extracted from the NHC microfilm
archive and the radius and pressure were estimated manually by J.
Pennington. The radius of maximum winds for 1988-89 that were added in
version 1.2 were obtained from the vortex messages of aircraft
reconnaissance missions. These values were smoothed in time (the
nearest three observations were averaged) to give the estimates included
in the extended best track data file. The wind radii for this period
(1988-89) are only included for cases where aircraft data was available.

All of the parameters not available in the HURDAT file were estimated
from operational data sources, including ship and other surface reports,
aircraft reconnaissance data and satellite imagery. At present, there are
no error estimates for these variables. Generally speaking, these
parameters are more reliable west of 55 longitude, where aircraft
reconnaissance data is usually available. Also, because the data is
operational, there is no guarantee that all of the parameters are
consistent. For example, the radius of 50 kt winds might be smaller
than the radius of 64 kt winds, even though this arrangement is not
physically possible. Note that in version 1.7 and higher the wind radii  
are from the NHC best track.

The extended best track file uses a simple ASCII format. There is
one line of data for each date and time period (00, 06, 12 or 18 UTC)
of each storm (see sample line listed below). The information is given
in the following order: Storm identification number, storm name, month,
day, time, year, latitude (deg N), longitude (deg W), maximum wind
speed (kt), minimum central pressure (hPa), radius of maximum wind
speed (nm), eye diameter (nm), pressure of the outer closed isobar (hPa),
radius of the outer closed isobar (nm), radii (nm) of 34 kt wind to the
NE, SE, SW and NW of the storm center, radii (nm) of 50 kt wind to the
NE, SE, SW and NW, radii (nm) of 64 kt wind to the NE, SE, SW, NW, and
a storm type code.  This code is either * for a tropical system
(tropical depression, tropical storm, or hurricane), W for tropical
wave, D for a tropical disturbance, S for a subtropical storm, E
for an extra-tropical storm, or L for remnant low. The last record
is the distance to the nearest major landmass (km), where the island of
Trinidad is the smallest area considered to be land. Negative values
indicate the storm center is over land.

Each item above is separated by a space in the file except the
following: The month, day, and time are listed as one 6-digit number
following the storm name.  For example, 06 UTC on July 10 would be
listed as 071006. Also the 34, 50, and 64-knot wind radii are separated
from one another, but the radii for the four directions (NE, SE, SW, NW)
are grouped together (12 characters). If any of these radii are less
than 100 nm, a space will occur within the grouping. Thus, a wind radii
group 125 25100100 indicates that winds at the given speed occur 125 nm
to the NE, 25 nm to the SE, 100 nm to the SW, and 100 nm to the NW of
the storm center. The following is a complete line of text from the
extended best track file:

AL0290 ARTHUR    072518 1990 13.1  63.7  60  995  30 -99 1012 180  60 60 60 60  30  0  0 30   0  0  0  0 *   267.

A -99 in any parameter is a default value that means no estimate was available.
