This is the changelog file for the OPC DA/AE Server SDK .NET.

## OPC DA/AE Server SDK .NET - 9.0.0 (Release Date 13-JUL-2019)

### New License Model & Pricing
The OPC DA/AE Server SDK .NET follows now a dual-license: 

#### Binaries
The OPC DA/AE Server SDK .NET is licensed under the MIT License. A very liberal license that encourages both commercial and non-commercial use. There are no separate runtime fees or royalties.

#### Source Code
The OPC DA/AE Server SDK .NET source code is available under a commercial source code license. There are no separate runtime fees or royalties.

Our Source Code License Agreement (https://technosoftware.com/documents/Source_License_Agreement.pdf) allows the use of the OPC DA/AE Server SDK .NET source code to develop software on and for all supported operating system and hardware platforms.

### Commercial Support
Purchase commercial suppourt via https://technosoftware.com/product/standard-support/ for a single Standard Support request (two hours support time budget, five business days maximum initial response time, although we usually answer within one to two business days) for EUR 390,00 from Technosoftware GmbH.

After completing the purchase, please use our HelpDesk at https://technosoftware.com/my-account/support/ to submit your request.

By purchasing support, you agree to our Support Service Agreement at https://technosoftware.com/documents/Support_Services_Agreement.pdf

## OPC DA/AE Server SDK .NET - 8.6.0 (Release Date 06-JUL-2019)

### Changed Behavior
- Generic Server updated to Visual Studio 2019

## OPC DA/AE Server SDK .NET - 8.5.0 (Release Date 06-MAY-2019)

### Changed Behavior
- Executables and assemblies no longer use a digital signature

### Fixed Issues
- Fixed memory leak caused by Logging

### Important
- The OPC DA/AE Server SDK .NET is no longer maintained.
  Please be aware that this product will no longer receive further features and updates. Only critical fixes will be provided for this product. 

## OPC DA/AE Server SDK .NET - 8.4.1 (Release Date 01-MAR-2019)

### Fixed Issues
- Fixed memory leak caused by ProcessConditionStateChanges
- Fixed memory leak caused by ProcessSimpleEvent
- Fixed memory leak caused by ProcessTrackingEvent

## OPC DA/AE Server SDK .NET - 8.4.0 (Release Date 02-FEB-2019)

### Changed Behavior
- If a client used GetGroupByName() while still having OnDataChange handler active on that group it could lead to a deadlock.
  The group list containing all groups must be searched by the GetGroupByName() function and the OnDataChange handling mechanism but also by 
  adding groups functionality. This was done by a simple lock mechanism and is now change to a read/write lock mechanism to avoid a deadlock.
  
## OPC DA/AE Server SDK .NET - 8.3.0 (Release Date 26-DEC-2018)

### New Features
- Updated to .NET 4.7.2

### Fixed Issues
- Updated evaluation license file

## OPC DA/AE Server SDK .NET - 8.2.0 (Release Date 10-NOV-2018)

### Changed Behavior
- For the acknowledgement of an AE Condition the generic server always used the current time for the state change 
  regardless if the acknowledgement came from a client or the server itself. 
  Now the time specified by the call to the ProcessConditionStateChanges() is used in case the acknowledgement is done by the custom specific part. 

## OPC DA/AE Server SDK DLL - 8.1.2 (Release Date 13-JUL-2018)

### Fixed Issues
- Fixed server crash when the character '-' is included in the directory path of the generic executable server file.
- Fixed server crash on server shutdown after last OPC client connected is disconnecting.

## OPC DA/AE Server SDK .NET - 8.1.1 (Release Date 13-APR-2018)

### New Features
- Updated to OPC Core Components 3.00.107

### Fixed Issues
- OnGetLogPath() wasn't called

## OPC DA/AE Server SDK .NET - 8.1.0 (Release Date 19-MAR-2018)

### New Features
- Source Code Option is now available

## OPC DA/AE Server SDK .NET - 8.0.0 (Release Date 01-JAN-2018)

### New Features
- OnGetLogLevel() added
- OnGetLogPath() added

### Removed Features
- OnGetLicenseInformation() no longer used

## OPC DA/AE Server SDK .NET - 7.5.1 (Release Date 31-JUL-2017)
- .NET 3.5, .NET 4.0 and .NET 4.5 no longer supported.

