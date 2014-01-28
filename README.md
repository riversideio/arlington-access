# arlington-access

Arlington Access is forked from [Open Access Control](https://code.google.com/p/open-access-control/) 
to control RFID access to the Riverside.io space. 

## Instructions

1. Place the .ino and .h files in a directory under your Arduino sketeches folder
2. Place the remaining directories in your Arduino libraries area (usually C:\Program Files (x86)\Arduino\libraries for Windows)
3. Restart the Arduino software if libraries were just added.
4. Connect up the Open Access v4. Allow the system to detect the USB/Serial port. Select "Arduino Duemillanove" from the
list of boards.
5. Change the privilege password.
6. Compile and upload the program.

_Changes since v1.35_

-10/23/2013 (Version 1.36)
-Updated the lockall() function to fix bug when relocking all doors (I/O pins high instead of low)
-Updated reader code to allow user to define whether or not a reader has a keypad from user.h file
-Updated superuser code to disable superusers by default.

## Usage

To login to the rasberry pi at the space do the following swapping
`port`, `username`, and `ipaddress` for the proper credentials. Request
those credentials from an active member.

```
ssh username@ipaddress -p port
```

## Notes

```
minicom screen msmtp arduino
```
