# Flutter fundamental

## Common Commands

rescan real device

```bash
adb kill-server
```

```bash
adb start-server
```

```bash
adb devices -l
```

---

```bash
cd android/
./gradlew tasks --all | grep externalNativeBuild
```

---

Repair pub cache (usually not needed)
```bash
flutter pub cache repair
```

Delete the cache directly (it will take a while)
```bash
rm -rf ~/.pub-cache
```

If you get some unknown error, it's useful to run this to clear some old stuff.
```bash
flutter clean
```

```bash
flutter pub get
```

---


```bash
keytool -list -v -keystore <KEYSTORE_PATH>
```

---

```
"$FLUTTER_HOME/packages/flutter_tools/gradle/src/main/kotlin/FlutterExtension.kt"
```

---

rebuild multi-language config files.
```bash
flutter gen-l10n
```

---

rebuild some dart gererated files.
```bash
dart run build_runner build
```

```bash
dart run build_runner build --delete-conflicting-outputs
```

```bash
dart run build_runner clean
```

---

Make your Dart code files easier for people to read.
```bash
dart format <PATH>
```
[dart format](https://dart.dev/tools/dart-format)

---

Auto generate documentation files.
```bash
dart doc <PATH>
```
[dart doc](https://dart.dev/tools/dart-doc)

## Basis

[本章目录 | 《Flutter实战·第二版》](https://book.flutterchina.club/chapter1/)

[Effective Dart](https://dart.dev/effective-dart)

## Utils

[equatable | Dart package](https://pub.dev/packages/equatable)

[hive | Dart package](https://pub.dev/packages/hive)

[file\_picker | Flutter package](https://pub.dev/packages/file_picker)

[flutter\_ringtone\_player | Flutter package](https://pub.dev/packages/flutter_ringtone_player)

[fluttertoast | Flutter package](https://pub.dev/packages/fluttertoast)

[flutter\_blue\_plus | Flutter package](https://pub.dev/packages/flutter_blue_plus)

[keyboard\_actions | Flutter package](https://pub.dev/packages/keyboard_actions)

[syncfusion\_flutter\_charts | Flutter package](https://pub.dev/packages/syncfusion_flutter_charts)

[json\_serializable | Dart package](https://pub.dev/packages/json_serializable)

[Day 22 多國語系支援 - iT 邦幫忙::一起幫忙解決難題，拯救 IT 人的一天](https://ithelp.ithome.com.tw/articles/10345741)

State management
- [State management | Flutter](https://docs.flutter.dev/get-started/fundamentals/state-management)
- [provider | Flutter package](https://pub.dev/packages/provider)
- [riverpod | Dart package](https://pub.dev/packages/riverpod)
- [bloc | Dart package](https://pub.dev/packages/bloc)
- [get | Flutter package](https://pub.dev/packages/get)
- [flutter\_redux | Flutter package](https://pub.dev/packages/flutter_redux)
- [mobx | Dart package](https://pub.dev/packages/mobx)

## Awesome Examples

[GitHub - guilherme-v/flutter-clean-architecture-example: A flutter's implementation of a "clean architecture" comparing BLoC, Cubit, GetIt, MobX, Provider, and Riverpod. It includes tests to all libraries and additional features like Material 3 theming, Widget and Unit Tests, Infinite scrolling, Remote API calls, Caching and etc..](https://github.com/guilherme-v/flutter-clean-architecture-example)

[GitHub - Khloud-azeem/Online-Shop-Mobile-App: A shop application, where you can both offer your own products as well as shop for products, add them to a cart and then place an order.](https://github.com/Khloud-azeem/Online-Shop-Mobile-App)

[GitHub - enesakbal/Flutter-Clean-Architecture-Example: Flutter Clean Architecture Example](https://github.com/enesakbal/Flutter-Clean-Architecture-Example)

[GitHub - mitesh77/Best-Flutter-UI-Templates: completely free for everyone. Its build-in Flutter Dart.](https://github.com/mitesh77/Best-Flutter-UI-Templates)

[github action搭建flutter流水线 | Distant Vicinity](https://kzs.moe/blog/015-flutter-github-workflow)
