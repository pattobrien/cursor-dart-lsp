This is a demo project that has diagnostics in the main.dart file, which can be
used to show that the Cursor IDE does not have the ability to read info,
warning, and error-level diagnostics for the Dart language.

## Requirements

Install Dart VSCode extension and Dart SDK, according to
https://dart.dev/get-dart

## Bug Description

In main.dart you should see 1 error and 1 info-level diagnostic.

These diagnostics use newer Dart language features and newer lint rules that the
Agent would have been trained to know. This is important, since the Agent seems
to GUESS what diagnostics are seen when it doesn't have access to read the
diagnostics themselves - so we avoid this type of false positive by using newer
types of diagnostics.
