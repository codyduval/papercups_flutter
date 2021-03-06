![logo](https://raw.githubusercontent.com/papercups-io/papercups_flutter/main/images/logo.svg)

[![pub package](https://img.shields.io/pub/v/papercups_flutter.svg?label=papercups_flutter&color=blue)](https://pub.dev/packages/papercups_flutter) [![style: effective dart](https://img.shields.io/badge/style-effective_dart-40c4ff.svg)](https://pub.dev/packages/effective_dart) ![License](https://img.shields.io/github/license/papercups-io/papercups_flutter?color=black) ![GitHub issues](https://img.shields.io/github/issues/papercups-io/papercups_flutter?color=green&label=Issues)


[![likes](https://badges.bar/papercups_flutter/likes)](https://pub.dev/packages/papercups_flutter/score) [![popularity](https://badges.bar/papercups_flutter/popularity)](https://pub.dev/packages/papercups_flutter) [![pub points](https://badges.bar/papercups_flutter/pub%20points)](https://pub.dev/packages/papercups_flutter/score) 

![Demo Chat](https://raw.githubusercontent.com/papercups-io/papercups_flutter/next/images/chatImages.png)

[![button](https://raw.githubusercontent.com/papercups-io/papercups_flutter/main/images/demoButton.svg)](https://papercups-demo.eduardom.dev/)      [![button](https://raw.githubusercontent.com/papercups-io/papercups_flutter/main/images/getPapercups.svg)](https://papercups.io/)


## Installing
To get started simply add `papercups_flutter:` and the latest version to your pubspec.yaml.
Then run `flutter pub get`

🎉 Done, It's that simple.
## Using the widget
Integration with your app requires just a few lines of code, add the following widget wherever you want your papercups chat window to be:
```Dart
import 'package:papercups_flutter/papercups_flutter.dart';

PaperCupsWidget(
    props: Props(
    accountId: "xxxxxxxx-xxxxxxx-xxxx-xxxxxx", //Your account id goes here.
    ),
),
    
```
That should get you up and running in just a few seconds ⚡️.

## Configuration

### Available PaperCupsWidget arguments
| Parameter | Type | Value | Default |
| :--- | :--- | :----- | :------ |
| **`props`** | `Props` | **Required**, here is where all of the config for the chat is contained.| N/A |
| **`dateLocale`** | `String` |Locale for the date, use the locales from the `intl` package.| `"en-US"` |
| **`timeagoLocale`** | `dynamic` | Check https://github.com/andresaraujo/timeago.dart/tree/master/timeago/lib/src/messages for the available classes.| N/A |
| **`sendingText`** | `String` | Text to show while message is sending.| `Sending...` |
| **`sentText`** | `String` | Text to show when the messgae is sent.| `Sent` |
| **`floatingSendMessage`** | `bool` | Wether to have the message box floating.| `false` |


### Available Props paramaters
| Prop | Type | Value | Default |
| :--- | :--- | :----- | :------ |
| **`accountId`** | `string` | **Required**, your Papercups account token | N/A |
| **`title`** | `string` | The title in the header of your chat widget | Welcome! |
| **`subtitle`** | `string` | The subtitle in the header of your chat widget | How can we help you? |
| **`newMessagePlaceholder`** | `string` | The placeholder text in the new message input | Start typing... |
| **`primaryColor`** | `Color` | The theme color of your chat widget | `Theme.of(context).primaryColor` without alpha |
| **`primaryGradient`** | `Gradient` | Gradient to specify, should be used instead of primaryColor, DO NOT USE BOTH. | N/A |
| **`greeting`** | `string` | An optional initial message to greet your customers with | N/A |
| **`customer`** | `CustomerMetadata` | Identifying information for the customer, including `name`, `email`, `external_id`, and `metadata` (for any custom fields) | N/A |
| **`baseUrl`** | `string` | The base URL of your API if you're self-hosting Papercups. Ensure you do not include the protocol (https) of a trailing dash (/) | app.papercups.io |
| **`requireEmailUpfront`** | `boolean` | If you want to require unidentified customers to provide their email before they can message you | `false` |
| **`companyName`** | `String` | Company name to show on greeting | `"Bot"` |
| **`enterEmailPlaceholer`** | `String` | This is the placeholder text in the email input section | `"Enter your email"` |

### Available CustomerMetaData paramaters
| Parameters | Type | Value | Default |
| :--- | :--- | :----- | :------ |
| **`email`** | `string` | The customer's email| N/A |
| **`externalId`** | `string` | The customer's external ID | N/A |
| **`name`** | `string` | The customer's name | N/A |
| **`otherMetadata`** | `Map<String, String>` | Extra metadata to pass such as OS info. | N/A |

## Developing

You will need flutter beta and flutter web support enabled.

```
flutter channel beta
flutter upgrade
flutter config --enable-web
```

## Supporters
[![Stargazers repo roster for @papercups-io/papercups_flutter](https://reporoster.com/stars/papercups-io/papercups_flutter)](https://github.com/papercups-io/papercups_flutter/stargazers) [![Forkers repo roster for @papercups-io/papercups_flutter](https://reporoster.com/forks/papercups-io/papercups_flutter)](https://github.com/papercups-io/papercups_flutter/network/members)
