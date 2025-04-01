This is a demo project that has a diagnostic in the main.dart file, which can be
used to see if cursor has the ability to read info, warning, and error-level
diagnostics in Dart.

In main.dart you should see 1 error and 1 info-level diagnostic.

These diagnostics use newer Dart language features and newer lint rules that the
Agent would have been trained to know. This is important, since the Agent seems
to GUESS what diagnostics are seen when it doesn't have access to read the
diagnostics themselves - so we avoid this type of false positive by using newer
types of diagnostics.
