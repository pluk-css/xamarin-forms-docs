---
title: Required Telerik Assemblies
page_title: Required Telerik Assemblies
position: 1
slug: gauge-getting-started-required-assemblies
---

# Required Telerik Assemblies

This article contains a list with the assemblies required by the **RadGauge** controls.

> The path of the assemblies is relative to the `Binaries` folder that is located in the installation folder of the controls. The default location is:  
> `C:\Program Files (x86)\Telerik\UI for Xamarin RX XXX\Binaries`.

| Platform | Location | Assemblies |
| -------- | -------- | ---------- |
| Portable | XamarinForms\Portable\ | Telerik.XamarinForms.Common.dll <br/> Telerik.XamarinForms.DataVisualization.dll <br/> Telerik.XamarinForms.Controls.SkiaSharp |
| Android  | XamarinForms\Android\ | Telerik.XamarinForms.Common.dll <br/> Telerik.XamarinForms.DataVisualization.dll <br/> Telerik.XamarinForms.Controls.SkiaSharp |
| iOS      | XamarinForms\iOS\ | Telerik.XamarinForms.Common.dll <br/> Telerik.XamarinForms.DataVisualization.dll <br/> Telerik.XamarinForms.Controls.SkiaSharp |
| UWP      | XamarinForms\UWP\ | Telerik.XamarinForms.Common.dll <br/> Telerik.XamarinForms.DataVisualization.dll <br/> Telerik.XamarinForms.Controls.SkiaSharp |

The gauge controls are rendered via the SkiaSharp graphics library so you need to install also [SkiaSharp.Views.Forms](https://www.nuget.org/packages/SkiaSharp.Views.Forms/1.55.0) in all projects of the xamarin solution (common, android, ios, etc). 

### See Also

- [Required Android Support Libraries]({%slug required-android-support-libraries%})
- [Getting Started]({%slug gauge-getting-started%})