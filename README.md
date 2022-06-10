# flutter_devenv
Development environment for flutter & firebase.

## NOTES
The docker file is provided for the arm64 architecture.So if you want to build a container for the x86_64 architecture, you need to make changes.
Do not use the qemu x86_64 emulator on the M1 architecture Host. It causes a segmentation fault.

As below:
```
FROM --platform=arm64 ubuntu:20.04 => FROM --platform=amd64 ubuntu:20.04
dartsdk-linux-arm64-release.zip => dartsdk-linux-x64-release.zip
```

