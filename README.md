# libxzxcba (v0.4.0)

Native builds of the crash reporter library, one folder per
operating system. Binaries only — no source code in this
repository. Source code lives in the
`imnotdeveloper0102/libcrashreporter` repository.

## Folders

- `android/` — native `.so` files (4 ABIs)
- `linux/` — native `.so` files (8 chips)
- `windows/` — native `.dll` files (3 chips, each with a `.lib`
  import library)

Apple (iOS/macOS/watchOS) and HarmonyOS builds are NOT included:
they need Xcode / DevEco Studio.

## Verification status (honest)

Only the Linux x86_64 build has been run (crash-tested, 18/18
checks). All other binaries are verified by file type and
exported symbols only and have never run on real hardware.

The binaries are hardened against casual reverse engineering
(stripped symbols, encrypted string literals). This raises the
bar; it does not make reverse engineering impossible.

## License

Triple-licensed: MIT, Apache-2.0, or GPL-3.0 — pick any one.
Full license texts are in the source repository.
