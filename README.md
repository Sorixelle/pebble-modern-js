# pebble-modern-js
A boilerplate for developing Pebble apps with ESNext+ support in PebbleKit JS.

## Usage
Just use it like you would any other Pebble project created with `pebble
new-project`. Any JS-side packages can be added with `npm install` like you
normally would in a JS project.

## Caveats
Some libraries (notably Firebase) might not work on the emulator. This is
because the emulator's JS runtime is very old and minimal, and doesn't support
all features that a browser environment would normally have, such as IndexedDB.
These apps will likely work when used on an Android phone, but may not work on
an iOS device. For this reason, it's not recommended to use libraries that
don't work on the emulator in a deployed app.
