# Tester-DLL
### Software J2534 Device Emulation

Emulate a J2534 Device in a that creates a perfect emulation, so you can test J2534 software with full emulation of the PassThru API and ISO14229 controller commmunication traffic as if you were sitting in car with device plugged into the OBD port.
A complete UDS stack is available for testing various diagnostic routines and procedures, created against ISO14229 - UDS.  

Added SAE 1979 compatibility(that's OBD2 for you n00bers) and some K-Line functionaslity, uploaded code as vs solution and new version uploaded to releases. 30/03/2026.

#### This tooling was developed by Tester Present Specialist Automotive Solutions for the wider open source automotive community. https://testerpresent.com.au/   


To build and run:
```
cd StubDLL && build_stub.cmd

cd EmuCore && dotnet build -c Release

cd Installer && install_registry.cmd C:\path\to\EmuJ2534.dll

EmuCore.exe --can-id 0x7E0 --resp-id 0x7E8  
```
