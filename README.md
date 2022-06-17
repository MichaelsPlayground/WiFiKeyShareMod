# WiFiKeyShare

Source: https://github.com/bparmentier/WiFiKeyShare

Libraries:

```plaintext
implementation 'org.wordpress:passcodelock:1.4.0' // TODO: update (1.5.1 fixed a PIN input screen bypass, but doesn't work currently)
entweder:
// https://mvnrepository.com/artifact/org.wordpress/passcodelock
implementation group: 'org.wordpress', name: 'passcodelock', version: '2.0.2'
oder version 1.2.0 verfügbar

```


[![Build Status](https://travis-ci.org/bparmentier/WiFiKeyShare.svg?branch=master)](https://travis-ci.org/bparmentier/WiFiKeyShare)

WiFiKeyShare lets you easily share your Wi-Fi password by generating a QR code or by writing it to
an NFC tag.

The format of the string encoded in the QR code is commonly used and should be recognized by most
barcode scanner applications.

The NFC tag is formatted in the same way as Android does since it introduced its "Write to NFC tag"
option in Lollipop. That means people running Android 5.0+ won't have to download any specific app
to connect to the network after scanning the tag.

## Note

Android does not let apps read the saved Wi-Fi passwords, so the user will need the enter them
manually for each network. However, the passwords will automatically be retrieved if WiFiKeyShare is
given root access.