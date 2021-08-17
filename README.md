# Cobrowse.io - Windows SDK

Cobrowse.io is 100% free and easy to try out in your own apps. Please see full documentation at [https://docs.cobrowse.io](https://docs.cobrowse.io).

Try our **online demo** at the bottom of our homepage at <https://cobrowse.io/#tryit>.

## Installation

We recommend installing the Cobrowse.io SDK using NuGet. Add the following package to your projects:

[![CobrowseIO.Windows NuGet](https://img.shields.io/nuget/v/CobrowseIO.Windows.svg?label=CobrowseIO.Windows)](https://www.nuget.org/packages/CobrowseIO.Windows/)

### Usage

To use Cobrowse.io in your project, use the `Cobrowse.IO` namespace:

```csharp
using Cobrowse.IO;
```

To start Cobrowse.io:

```csharp
CobrowseIO.Instance.License = "put your license key here";
await CobrowseIO.Instance.Start();
```

### Add your License Key

Please register an account and generate your free License Key at [https://cobrowse.io/dashboard/settings](https://cobrowse.io/dashboard/settings).

This will associate sessions from your Windows app with your Cobrowse account.

### HiDPI Support

For Windows 10 HiDPI mode \(when display scale is not 100%\) client application should be "DPI aware". To enable this please add `app.manifest` \("New item" -&gt; "Application Manifest File" in Visual Studio\) and add/uncomment the following XML tag:

```markup
<application xmlns="urn:schemas-microsoft-com:asm.v3">
  <windowsSettings>
    <dpiAware xmlns="http://schemas.microsoft.com/SMI/2005/WindowsSettings">true</dpiAware>
  </windowsSettings>
</application>
```

## Try it out

Once you have your app running on a Windows computer, navigate to [https://cobrowse.io/dashboard](https://cobrowse.io/dashboard) to see your device listed. You can click the "Connect" button to initiate a Cobrowse session!

## Optional features

[Identify your devices](https://docs.cobrowse.io/sdk-features/identify-your-devices)

[Use 6-digit codes](https://docs.cobrowse.io/sdk-features/6-digit-codes)

[Redact sensitive data](https://docs.cobrowse.io/sdk-features/redact-sensitive-data)

[Customize the interface](https://docs.cobrowse.io/sdk-features/customize-the-interface)

[Initiate sessions with push](https://docs.cobrowse.io/sdk-features/initiate-sessions-with-push)

[Full device capabilities](https://docs.cobrowse.io/sdk-features/full-device-capabilities)

[Advanced features](https://docs.cobrowse.io/sdk-features/advanced-features)

## Questions?
Any questions at all? Please email us directly at [hello@cobrowse.io](mailto:hello@cobrowse.io).

## Requirements

* .NET Framework 4.6.1
* Minimal supported OS is Windows 7
* _x86_ and _x64_ architectures only are supported
