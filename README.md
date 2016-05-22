# NativeScript BootReceiver

Starts the main activity of a NativeScript application on BOOT_RECEIVED

## Installation

Open a shell, go to your app's root folder and run

```
tns plugin add nativescript-bootreceiver
```

## Usage

### Android

Add the boot receiver to the application node of your Android manifest

```
<receiver
    android:name="com.dashorando.bootreceiver.BootReceiver"
    android:enabled="true"
    android:exported="false"
    android:permission="android.permission.RECEIVE_BOOT_COMPLETED" >
    <intent-filter>
        <action android:name="android.intent.action.BOOT_COMPLETED" />
        <category android:name="android.intent.category.DEFAULT" />
    </intent-filter>
</receiver>
```

### iOS

To be done

## Feature requests

Let us know what you need by opening a Github issue

Planned features:

- Add iOS support
