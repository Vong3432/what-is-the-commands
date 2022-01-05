# Flutter

Just a repo that stores frequently used commands from flutter

## 🚧 Development

#### Check flutter health

This command will check the status of installed Flutter.

```
flutter doctor
```

#### Check flutter health (w/ detail info)

This command will check the status of installed Flutter with extra detail message.

```
flutter doctor -v
```

#### Start flutter project

This command will run Flutter app.

```
flutter run
```

#### Start flutter project (w/ detail info)

This command will run Flutter app with extra detail message. By using this command, most of the time you can view more detailed error message during the development process.

```
flutter run -v
```

#### Release app to production build

This command will compile your Flutter app into release mode. Usually you will run this when you want to know how your apps work without development mode before deploying it to App Store or Google Playstore.

```
flutter run --release
```

#### Clean build

This command will clean your Flutter project cache. Usually you are gonna run this when your Flutter app is not working correctly. Once you run this command, your IDE should have bunch of errors, because everything is deleted. But this can be fixed once you [start](#start-flutter-project) your project again.

```
flutter clean
```

#### Run build runner

This command will generate files using Dart code.
```
flutter pub run build_runner build              
```

#### Clear build runner conflicts 

This command will remove all conflicts from previous build data.
```
flutter packages pub run build_runner build --delete-conflicting-outputs          
```

## 📦 Packages & Dependencies

#### Install package

```
flutter pub add <<package_name>>
```

#### Uninstall package

```
flutter pub remove <<package_name>>
```
