Alias Short by Thet Zaw Latt

Alias Short is a command-line tool that simplifies commonly used Flutter commands by allowing you to create short aliases for longer Flutter commands. Instead of typing lengthy commands like flutter build apk --release, you can simply type apk in the terminal to achieve the same result.

Features
•	Shorten long Flutter commands to quick and easy aliases.
•	Supports common Flutter build commands, such as building APKs, iOS builds, and more.
•	Easy to customize and extend by adding more aliases.

Installation
1.	Activate the package globally using the Dart command:

```bash
dart pub global activate alias
```

Add path:
2.	Ensure that the Dart SDK's bin directory is added to your system's PATH environment variable. This directory is typically located at C:\src\flutter\bin\cache\dart-sdk\bin on Windows or /usr/local/bin on macOS and Linux.
If not, add the output of this command to your PATH:
You will see the following output:

```bash
Building package executables...
Built alias:alias.
Installed executables alias, apk and ios.
Warning: Pub installs executables into $HOME/.pub-cache/bin, which is not on your path.
You can fix that by adding this to your shell's config file (.bashrc, .bash_profile, etc.)
export PATH="$PATH":"$HOME/.pub-cache/bin"
Activated alias 1.0.2.
```    
```bash
dart pub global list
```
Verify the installation:
3.	Verify that the installation was successful by running the following command:

```bash
alias --version
```

Usage

After installing the package, you can use the following aliases in your terminal:

•	Generate APK:
```bash
alias apk
```
•	Generate ios build:
```bash
alias ios
```

This is a shortcut for running flutter build ios.

You can add more commands by editing the commandsMap in the package.

Example

To generate a release APK for Android, simply open your terminal in your Flutter project and type:

```bash
apk
```
Instead of typing the full command:

```bash
flutter build apk --release
```

Customization

You can easily customize or extend the package by adding your own aliases.
1.	Clone this repository.
2.	Open the bin/alias.dart file.
3.	Add more aliases to the commandsMap:

```dart
final commandsMap = {
  'apk': 'flutter build apk --release',
  'ios': 'flutter build ios',
  'web': 'flutter build web',
  'clean': 'flutter clean',
  // Add more aliases here
};
```
//
4.	Rebuild the package or use it locally.

Contributing

Contributions are welcome! If you’d like to add more functionality or improve the package, feel free to open a pull request or submit an issue.

License

This project is licensed under the MIT License. See the LICENSE file for details.

Additional Notes:
1.	You can modify the Customization section to better fit your own development workflow.
2.	Be sure to replace the links in the License and Contributing sections with the correct URLs if needed.

Let me know if you need any further adjustments!



