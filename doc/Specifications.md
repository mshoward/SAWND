#SAWND: Sound Above Windows NT Drivers

###Contents:
1. Description
2. Specifications
3. Features
4. Software Used

##Description:

SAWND is intended to be a lightweight application allowing users to decide on an application basis which audio device to output sound.
Currently, Windows classifies audio and applications into two categories: communication and not-communication.
This lack of control results in users unable to maximize their audio experience.
In addition, from this centralized point, users can also customize their audio experience by
varying aspects of the sound output and optimizing playback for the best listening experience possible.


##Specifications:

In order to improve the development process,
components of the software will be split into modules.


###Virtual Sound Device:

This will be the component that captures sound.
This is what will be selected as the default sound device in Windows.
Based on the application accessing the Virtual Sound Device, output will be
selectively output to one or more actual sound devices or files. This will have
minimal interaction with the user, but will be accessed and controlled by other
software components.



###Control Board:

This will be the component that manages other
omponents interacting with the Virtual Sound Device (VSD). From it, features
like an equalizer, amplifier and application settings will be accessed.



###Control Board Components:

These will be self contained components that pass their
information off to the VSD. Information passing can be through signals,
configuration changes, transformation function passing, etc. How this will
exactly be handled is yet to be determined.

##Features

###Starting Features:
*Virtual Sound Device
*Control Board
*Control Board Component: Application Sound Device Selector
*Control Board Component: SAWD Settings

###Possible Features:
*Equalizer
*Amplifier
*Audio Transformer
*Audio Stream Capture
