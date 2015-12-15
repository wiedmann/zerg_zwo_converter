# Zerg zwo Converter
ERG/MRC to Zwift Workout File, based on code posted to this blog https://fukawitribe.wordpress.com/2015/12/15/zerg-ergmrc-to-zwift-workout-file/

# ZWO Tag Syntax Documentation
In an effort to better understand the format that is needed for Zwift to correctly accept the files this script creates, here is some reverse engineered documentation.

## SteadyState
An interval that stays at the same level for the entire time.
  - Duration: Time of Interval, in seconds
  - PowerLow: % of FTP for interval divided by 100
  - PowerHigh: % of FTP for interval divided by 100 (appears to be redundant to PowerHigh)
  

## Warmup
An interval that slowly increases the power required throughout the duration of the interval.
  - Duration: Time of Interval, in seconds
  - PowerLow: % of FTP for the start of the warmup divided by 100
  - PowerHigh: % of FTP for the end of the warmup divided by 100

## Cooldown
An interval that slowly decreases the power required throughout the duration of the interval.
  - Duration: Time of Interval, in seconds
  - PowerLow: % of FTP for the start of the cooldown divided by 100
  - PowerHigh: % of FTP for the end of the cooldown divided by 100
