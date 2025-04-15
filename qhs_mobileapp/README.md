# QHS Mobile App

## Overview
The QHS Mobile App is a Flutter-based application that integrates Firebase for authentication and provides a feature to generate QR codes containing user-specific information. The app demonstrates the use of Firebase Authentication, GPS location services, and QR code generation.

## Features
- **Firebase Authentication**: Users can sign up and log in using Firebase Authentication.
- **QR Code Generation**: Generate QR codes containing the user's email, GPS location, and the current timestamp.
- **Cross-Platform Support**: The app is designed to run on Android, iOS, and other platforms supported by Flutter.

## Prerequisites
- Flutter SDK installed ([Installation Guide](https://flutter.dev/docs/get-started/install))
- Firebase project set up with `google-services.json` (Android) and `GoogleService-Info.plist` (iOS)
- Android Studio or Xcode for platform-specific builds

## Installation
1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd QHS_MobileApp/qhs_mobileapp
   ```

2. Install dependencies:
   ```bash
   flutter pub get
   ```

3. Run the app:
   ```bash
   flutter run
   ```

## Project Structure
- `lib/main.dart`: Main entry point of the application.
- `android/`: Android-specific files and configurations.
- `ios/`: iOS-specific files and configurations.
- `pubspec.yaml`: Project dependencies and metadata.

## Firebase Setup
1. Add your `google-services.json` file to `android/app/`.
2. Add your `GoogleService-Info.plist` file to `ios/Runner/`.
3. Ensure Firebase is initialized in `main.dart`.

## QR Code Data Format
The generated QR code contains the following JSON structure:
```json
{
  "user": "useremail@example.com",
  "location": {
    "latitude": 12.345678,
    "longitude": 98.765432
  },
  "time": "2025-04-15T12:34:56.789Z"
}
```

## Contributing
Contributions are welcome! Please fork the repository and submit a pull request.

## License
This project is licensed under the MIT License. See the LICENSE file for details.
