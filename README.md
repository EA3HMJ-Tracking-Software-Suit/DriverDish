# DriverDish
Program that is responsible for requesting data from the ephemeris server and communicating with ControllerDish.

[Version and download](#Versions)

## New version 2.0

The new version of DriverDish it is a major change as I have rewritten the whole app.
I've been testing it for a while and it has passed my tests, things can always go wrong and I'm waiting for your reports.
This version needs a new firmware (4.x+) in ControllerDish, which is totally new and with a new security philosophy.
Due to problems with a chip in the controller I have lowered the communication speed to 115200 Bauds instead of 500000 bauds, it doesn't affect the accuracy but it eliminates a problem.

<img src="https://github.com/user-attachments/assets/0d0f3899-75bb-46a2-ae96-c8ad155a590d" width="640">
<img src="https://github.com/user-attachments/assets/2d88f533-caa3-4422-b017-df7e5e0ea6cb" width="640">
<img src="https://github.com/user-attachments/assets/82ef3e7b-f930-44a1-81f6-ecfd2d98ce98" width="640">


## Description version 1.x
This is the main program that is responsible for requesting data from the ephemeris server and communicating with ControllerDish.

<img src="https://github.com/ea3hmj/EME/raw/main/img/dd10.jpg" width="640">
<img src="https://github.com/ea3hmj/EME/raw/main/img/dd2.jpg" width="640">
<img src="https://github.com/ea3hmj/EME/raw/main/img/dd30.jpg" width="640">
<img src="https://github.com/ea3hmj/EME/raw/main/img/dd4.jpg" width="640">
<img src="https://github.com/ea3hmj/EME/raw/main/img/dd5.jpg" width="640">
<img src="https://github.com/ea3hmj/HMJTS/blob/main/img/wx.png" width="640">

New functionality, Computes the offset for the maximum SN signal.

<img src="https://github.com/ea3hmj/HMJTS/assets/2368602/023db93c-6330-43fc-a475-cc25fea36a1c" width="342">

Communications are RS-485 at 500000 bauds.

The ESP32 port is used for debug also at 500000 bauds.

It can handle CAT radios, you need to have [OMNIRIG v2.1](https://www.hb9ryz.ch/omnirig/) installed.

If you have [SpectraVue v3.41](http://www.rfspace.com/RFSPACE/SpectraVue.html) installed, the program can get the RMS value of the signal in continuous mode, and with this data we can get a heatmap or radiomap.
The HeatMap software will be posted in another directory.

<img src="https://github.com/ea3hmj/EME/raw/main/img/heatmap.jpg" width="640">

<a name="Versions"></a>
## Documents
[DriverDish v1 ESP](https://github.com/EA3HMJ-Tracking-Software-Suite/.github/blob/main/DriverDish%20v1%20ESP.pdf)

[DriverDish v1 ENG](https://github.com/EA3HMJ-Tracking-Software-Suite/.github/blob/main/DriverDish%20v1%20ENG.pdf).
## Versions
1.0.0	Initial version.

1.0.817	Display the ControllerDish version in the setup form.

1.0.825	stop tracking whith el<0.

1.0.827 buton stop now stop tracking & motors, Fonts update, Bug in window reposition

1.0.859 read ambient temp from encoder elevation

1.1.954 current sense motors, suport external mini weather station

1.1.960 offset for mini eather station

1.1.981 optimising communications with wx

1.1.1008 Stop tracking when astroserver down.

1.1.1026 Update ASCOM interface, Radio TAB add IF 7400MHz

1.1.1042 Auto position, computes the offset for the maximum SN signal.

2.0 New program with new features

[Versions](https://github.com/EA3HMJ-Tracking-Software-Suite/DriverDish/releases)

## Download
[Latest versions](https://github.com/EA3HMJ-Tracking-Software-Suite/DriverDish/releases/latest)

## Disclaimer
This is an antenna tracking system (software and hardware) designed for amateur use in Earth–Moon–Earth communication (EME), radioastronomy, amateur Deep Sky Network (DSN) and other Space Communication applications where accurate and high precision tracking are required. 
