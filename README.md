# otp_count_down

Easily implement the count down timer in Flutter Application.

# Usage

Import `package:otp_count_down/otp_count_down.dart`

Example:

```dart
import 'package:otp_count_down/otp_count_down.dart';

OTPCountDown _otpCountDown; // create instance
final int _otpTimeInMS = 1000 * 5 * 60;  // time in milliseconds for count down

_otpCountDown = OTPCountDown.startOTPTimer(
    timeInMS: _otpTimeInMS, // time in milliseconds
    currentCountDown: (String countDown) {
        print("Count down : $countDown"); // shows current count down time
    },
    onFinish: () {
        print("Count down finished!"); // called when the count down finishes.
    },
);
```

You will find links to the API docs on the [pub page](https://pub.dev/packages/otp_count_down).

## Getting Started

For help getting started with Flutter, view our online
[documentation](http://flutter.io/).

For help on editing plugin code, view the [documentation](https://flutter.io/platform-plugins/#edit-code).
