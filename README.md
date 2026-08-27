# Getting Started with Syncfusion Xamarin MaskedEdit (SfMaskedEdit)

This repository contains a getting-started sample that demonstrates how to use the Syncfusion **SfMaskedEdit** control in a Xamarin.Forms application. The project is configured as a multi-target solution covering **Xamarin.Forms (netstandard2.0)**, **Xamarin.Android**, **Xamarin.iOS**, and **UWP**, so the same masked input behavior can be evaluated across all the supported platforms from a single shared code base.

## About the SfMaskedEdit control

`SfMaskedEdit` is a flexible input control that restricts user input to a defined pattern. It is commonly used to collect structured data such as phone numbers, credit card numbers, dates, IP addresses, currency, and product codes, while preventing the user from typing invalid characters. The control supports both `Simple` and `RegEx` mask types, allows culture-aware formatting, provides prompt and placeholder characters, and exposes value, validation, and culture-related APIs that you can bind to in MVVM scenarios.

In this sample, the `SfMaskedEdit` is configured with `MaskType="RegEx"` and `Mask="\w+"`, accepting one or more word characters, and its initial value is set to **"Syncfusion"** through the `Value` property. The control is declared in `MainPage.xaml` using the `Syncfusion.XForms.MaskedEdit` namespace and rendered inside a `StackLayout` with a top margin so the input area is clearly visible on the device.

## Prerequisites

To build and run this sample locally, install the following:

- Visual Studio 2022 with the **Mobile development with .NET** and/or **Universal Windows Platform** workloads.
- Xamarin.Forms **4.8.0.1687** (referenced from the shared project) and **Xamarin.Essentials 1.2.0**.
- The Syncfusion **SfMaskedEdit** NuGet package (`Syncfusion.Xamarin.SfMaskedEdit`), restored through NuGet.
- Android SDK and emulator images for the Android target, Xcode for the iOS target, and the Windows 10 SDK for the UWP target.
- A valid Syncfusion license if you plan to deploy a release build; the control works in trial mode for development and evaluation.

## Running the sample

1. Clone or download this repository to a local folder.
2. Open the solution file `MaskedEdit_Sample.sln` in Visual Studio.
3. Restore the NuGet packages for the solution so the Syncfusion and Xamarin dependencies are downloaded.
4. Set the desired startup project — `MaskedEdit_Sample.Android`, `MaskedEdit_Sample.iOS`, or `MaskedEdit_Sample.UWP` — as the launch target.
5. Select an appropriate device or emulator and press **F5** to build and deploy the app.
6. The main page will display the masked edit control pre-filled with the value **Syncfusion**; edit the text to see the regular-expression mask accept only word characters.

## Project structure

- `MaskedEdit_Sample/` – shared Xamarin.Forms project containing `App.xaml`, `App.xaml.cs`, `MainPage.xaml`, and `MainPage.xaml.cs`.
- `MaskedEdit_Sample.Android/` – Android host project with `MainActivity.cs`, manifest, and platform resources.
- `MaskedEdit_Sample.iOS/` – iOS host project with `AppDelegate.cs`, `Info.plist`, and launch storyboard.
- `MaskedEdit_Sample.UWP/` – UWP host project with `App.xaml`, `MainPage.xaml`, and `Package.appxmanifest`.

## Further learning

For more details about the SfMaskedEdit control, its properties, available mask characters, and customization options, refer to the official Syncfusion Xamarin documentation and the API reference included with the NuGet package.
