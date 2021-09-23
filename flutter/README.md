# Flutter

Just a repo that stores frequently used commands from flutter

## 🚧 Development

##### Check flutter health

This command will check the status of installed Flutter.

```
flutter doctor
```

##### Check flutter health (w/ detail info)

This command will check the status of installed Flutter with extra detail message.

```
flutter doctor -v
```

##### Start flutter project

This command will run Flutter app.

```
flutter run
```

##### Start flutter project (w/ detail info)

This command will run Flutter app with extra detail message. By using this command, most of the time you can view more detailed error message during in development.

```
flutter run -v
```

##### Clean build

This command will clean your Flutter project cache. Usually you are gonna run this when your Flutter app is not working correctly. Once you run this command, your IDE should have bunch of errors, because everything is deleted. But this can be fixed once you [start](#start-flutter-project) your project again.

```
flutter clean
```

## 📦 Packages & Dependencies

##### Install package

```
flutter pub add <<package_name>>
```

##### Uninstall package

```
flutter pub remove <<package_name>>
```
