### Android Studio Configuration

#### Platform Tools Include adb

- The SDK will be downloaded the first time you install it.

#### Check SDK Path

- Settings -> Languages & Frameworks -> Android SDK

The adb path is within Platform Tools.

#### Install ADB Keyboard

1. Download the [ADB Keyboard](https://github.com/senzhk/ADBKeyBoard/blob/master/ADBKeyboard.apk)

2. Install it on the virtual device:

- View -> Tool Windows -> Device Explorer
- `/storage/emulated/0/Download`

- Upload the `ADBkeyboard.apk`
- Find and install the file on the phone screen.
*In case adb keyboard doesn't work, you can enable it with the following commands:*

```bash
adb shell ime enable com.android.adbkeyboard/.AdbIME
adb shell settings put secure default_input_method com.android.adbkeyboard/.AdbIME
adb shell settings get secure default_input_method

```

### MobileAgent
Modify config.py to set up adb and API.
Modify the instruction in it.

For first time use pls run "RAG/create_localRAG_adb.py" to find app

Use "RAG/FAISS_create.py" to create localRAG database and MemRAG database 