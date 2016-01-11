# MAME4droid-GeneralGamePadSupport
MAME4droid General GamePad Support - base MAME4droid 1.9.2 (0.139u1)

This is part of the https://code.google.com/p/imame4all/ .
If there is a file needed to build, refer to the original project.

Now base on MAME4droid (0.139u1) 1.9.2 src

Changed files
	android\src\com\seleuco\mame4droid\input\InputHandler.java
	android\src\com\seleuco\mame4droid\input\InputHandlerExt.java
	android\src\com\seleuco\mame4droid\prefs\ListKeys.java
	android\src\com\seleuco\mame4droid\prefs\KeySelect.java
	
Description
	Automatic Detect game pad existing MAME4droid is to operate only in a given specific device, Bluetooth-enabled game pad not listed, it was not support multiple users.
	If it is less than Android 4.4, and is classified by using a DeviceId. Android 4.4 or higher, is classified by using a ControllerNumber.
	DeviceId the id of all input devices. ControllerNumber the judgment shall be granted in the case of a game pad
	We guarantee the good behavior in Adroid 4.4 or more.
	Save DeviceId before 2Byte of existing keyCode 4Byte, Save the original keyCode to the rear 2Byte.
	If the key code has exceeded 2Byte area, it is determined that would error occurs.
	DeviceId and ControllerNumber are granted when device connect.
	Therefore, it may be necessary to re-create the settings each time it connects. :)
	And, D-PAD setting(Up, Down, Left, Right) does not work to the individual.
	It follows all the correct D-PAD Up setting.
