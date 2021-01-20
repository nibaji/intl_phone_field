# International Phone Field Package

A customised Flutter TextFormField to input international phone number along with country code.

This widget can be used to make customised text field to take phone number input for any country along with an option to choose country code from a dropdown.

## Screenshots

<img src="https://github.com/nibaji/intl_phone_field/blob/master/1.png?raw=true" height="500px"> <img src="https://github.com/nibaji/intl_phone_field/blob/master/2.png?raw=true" height="500px"> <img src="https://github.com/vanshg395/nibaji/blob/master/3.png?raw=true" height="500px">

## Installing

To use this package:

Add the following to your `pubspec.yaml` file:

```yaml
dependencies:
  intl_phone_field:
    git: https://github.com/nibaji/intl_phone_field.git
```

## How to Use

Simply create a `IntlPhoneField` widget, and pass the required params:z

```dart
IntlPhoneField(
    decoration: InputDecoration(
        labelText: 'Phone Number',
        border: OutlineInputBorder(
            borderSide: BorderSide(),
        ),
    ),
    initialCountryCode: 'IN',
    onChanged: (phone) {
        print(phone.completeNumber);
    },
)
```

Use `initialCountryCode` to set an initial Country Code.

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## CONTRIBUTORS

- [Vansh Goel](https://github.com/vanshg395/)
- [Nidhun Balaji T R](https://github.com/nibaji/)

## LICENSE

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
