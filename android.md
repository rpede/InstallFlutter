# Android

## Install Windows

`winget install --id Google.AndroidStudio`

## Install Mac

*Requires MacOS 10.14 (Mojave) or higher*

[Download](https://developer.android.com/studio)

Open and drag Android Studio icon into Applications folder.

Follow the instructions.

## Configure SDK

Verify that flutter is able to locate the SDK by running `flutter doctor`.

Open **Android Studio**

### Virtual Android device

Open **Virtual Device Manager**

![](./screenshots/android1.png)

Create a new virtual Android device by clicking **Create Device**

![](./screenshots/android2.png)

You should pick something with Play Store enabled. I chose Pixel 2.

![](./screenshots/android3.png)

Click the small download icon on item with API Level 33.
Wait for it to complete then next.

![](./screenshots/android4.png)

Finish

![](./screenshots/android5.png)

Open **SDK Manager**

![](./screenshots/android6.png)

Check **Android SDK Command-line Tools** and click **OK**.

![](./screenshots/android7.png)