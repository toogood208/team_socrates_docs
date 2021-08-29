# Utilities
*This directory contains subdirectories for utility classes, functions, mixins and even extension classes.*

## constants
This contains the constant variable that will be used through out the app, they do not change
### constants.dart
This contains the app constants used
```dart
//* Credentials
const apiBaseUrl = '';

//* Client data
const appName = 'ZuriChat App';

//* Messages
const serverErrorMessage = 'An error occured. Please try again.';

const networkErrorMessage = 'Please check your internet'
    ' connection and try again';

//* Defaults
const defaultAvatarAsset = 'assets/images/fire_cracker.png';
const defaultNetworkImage = 'https://placeimg.com/300/550/nature';
```
**Usage**
```dart
import 'lib/utilities/constants/constants.dart';
```

### styles.dart
This file contains the constants used for styling the app like color, textstyles, sizes, etc.

```dart
const logoAsset = AssetImage('assets/logo/hng_logo.png');
const dummyNetworkImage =
    'https://loremflickr.com/320/240/paris,news,work?random=';

const dummyNetworkVideo =
    'https://commondatastorage.googleapis.com/gtv-videos-bucket/sample/VolkswagenGTIReview.mp4';

//* COLORS

//* TEXTSTYLES

//* DECORATION

//* MARKDOWN STYLE DATA
```
**Usage**
```dart
import 'lib/utilities/constants/styles.dart';
```

## extensions
Contains dart extension methods
### string_extensions.dart
This contains some extension methods that extends the String

**validateEmail**
Used for validating if a string is an email
```dart
bool validateEmail()
```

**Usage**
```dart
import 'lib/utilities/extensions/string_extension.dart';

"user@mail.com".validateEmail()
```
### strip
checks if the string is empty
```dart
bool strip()
```

**Usage**
```dart
import 'lib/utilities/extensions/string_extension.dart';

"  ".strip()
```

### turnStringToDate
checks if the string is empty
```dart
 String turnStringToDate(String format)
 //see string definition for more
```

**Usage**
```dart
import 'lib/utilities/extensions/string_extension.dart';

"2012-02-27".turnStringToDate('EEE, M/d/y')
//Returns 'Mon, 2/27/2012'

//Example of Accepted String Formats
//"2012-02-27"
//"2012-02-27 13:27:00"
//"2012-02-27 13:27:00.123456789z"
//"2012-02-27 13:27:00,123456789z"
//"20120227 13:27:00"
//"20120227T132700"
//"20120227"
//"+20120227"
//"2012-02-27T14Z"
//"2012-02-27T14+00:00"
//"-123450101 00:00:00 Z": in the year -12345.
//"2002-02-27T14:00:00-0500": Same as "2002-02-27T19:00:00Z"
```

### validateLink
Used for checking if a string is a valid url link
```dart
bool validateLink()
```

**Usage**
```dart
import 'lib/utilities/extensions/string_extension.dart';

"https://www.google.com".validateLink()
```
## mixin
Mixin classes [Read More here](https://medium.com/flutter-community/https-medium-com-shubhamhackzz-dart-for-flutter-mixins-in-dart-f8bb10a3d341)

### close_on_second_back_mixin.dart
*Code samples coming soon*
## enums.dart
*nothing here yet*

## utilities.dart

### makeNetworkImage

This helps to show images from the internet and keep them in the cache directory
```dart
ImageProvider makeNetworkImage(String? link)
```


**Usage**
```dart
import 'lib/utilities/utilities.dart';

makeNetworkImage("https://google.com")
```

### openUrl

The openUrl function will be used for opening URL links
```dart
Future<void> openUrl(String? url)
```
**Usage**
```dart
import 'lib/utilities/utilities.dart';

openUrl("https://google.com")
```



## validators.dart

### notEmptyField
Checks if a field is empty
```dart
 String? notEmptyField(String input, [String? label])
```

**Usage**
```dart
import 'lib/utilities/validators.dart';
Validator validate = Validator.validate;

 validate.notEmptyField("", "name")
```

### emailField
checks if an email address is valid
```dart
  String? emailField(String input)
```

**Usage**
```dart
import 'lib/utilities/validators.dart';
Validator validate = Validator.validate;

 validate.emailField('user@nmail.com')
```

### passwordField
checks if a password has been inputted
```dart
   String? passwordField(input) 
```

**Usage**
```dart
import 'lib/utilities/validators.dart';
Validator validate = Validator.validate;

 validate.passwordField('my Aw3s0me p4SSw04d@1')
```

### confirmPasswordField
checks if a passwords match
```dart
  String? confirmPasswordField(String input, String password)
```

**Usage**
```dart
import 'lib/utilities/validators.dart';
Validator validate = Validator.validate;

 validate.confirmPasswordField('my Aw3s0me p4SSw04d@1','my awesome password@1')
```
