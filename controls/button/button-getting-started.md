---
title: Getting Started
page_title: Getting Started
position: 1
slug: button-getting-started
---

# Getting Started

This article will guide you through the steps needed to add a basic **RadButton** control in your application.

* [Setting up the app](#1-setting-up-the-app)
* [Adding the required Telerik references](#2-adding-the-required-telerik-references)
* [Adding RadButton control](#3-adding-radbutton-control)


## 1. Setting up the app

Take a look at these articles and follow the instructions to setup your app:

- [Setup app with Telerik UI for Xamarin on Windows]({%slug getting-started-windows%})
- [Setup app with Telerik UI for Xamarin on Mac]({%slug getting-started-mac%})

## 2. Adding the required Telerik references

You have two options:

* Add the Telerik UI for Xamarin Nuget packages following the instructions in [Telerik NuGet package server]({%slug telerik-nuget-server%}) topic.

* Add the references to Telerik assemblies manually, check the list below with the required assemblies for **RadButton** component:

| Platform | Assemblies |
| -------- | ---------- |
| Portable | Telerik.XamarinForms.Common.dll<br/>Telerik.XamarinForms.Input.dll<br/>Telerik.XamarinForms.DataControls.dll |
| Android  | Telerik.Xamarin.Android.Common.dll<br/>Telerik.Xamarin.Android.Data.dll<br /> Telerik.Xamarin.Android.Input.dll<br/>Telerik.Xamarin.Android.List.dll<br/>Telerik.Xamarin.Android.Primitives.dll<br/>Telerik.XamarinForms.Common.dll<br/> Telerik.XamarinForms.Input.dll<br/> Telerik.XamarinForms.DataControls.dll |
| iOS      | Telerik.Xamarin.iOS.dll <br/>Telerik.XamarinForms.Common.dll<br/>Telerik.XamarinForms.Input.dll<br/>Telerik.XamarinForms.DataControls.dll |
| UWP      | Telerik.Core.dll<br/>Telerik.Data.dll<br />  Telerik.UI.Xaml.Controls.Data.UWP.dll<br /> Telerik.UI.Xaml.Input.UWP.dll<br/>Telerik.UI.Xaml.Primitives.UWP.dll<br/>Telerik.XamarinForms.Common.dll<br/>Telerik.XamarinForms.Input.dll<br/>Telerik.XamarinForms.DataControls.dll |

## 3. Adding RadButton control

You could use one of the following approaches:

#### Drag the control from the Toolbox. 

Take a look at the following topics on how to use the toolbox:

* [Telerik UI for Xamarin Toolbox on Windows]({%slug telerik-xamarin-toolbox%})
* [Telerik UI for Xamarin Toolbox on Mac]({%slug telerik-xamarin-toolbox-mac%})
	
#### Create the control definition in XAML or C#.

The snippet below shows a simple RadButton definition:

<snippet id='button-getting-started-xaml'/>

In addition to this, you need to add the following namespace:

<snippet id='xmlns-telerikinput'/>
<snippet id='ns-telerikinput'/>

Then define the Click event handler:

<snippet id='button-getting-started-click-event'/>

Here is the result:

![Button Getting Started Example](images/button-getting-started.png)

>important [SDK Browser](https://github.com/telerik/xamarin-forms-sdk) and [QSF](https://github.com/telerik/telerik-xamarin-forms-samples/tree/master/_Samples%20Application) applications contain different examples that show RadButton's main features.

## See Also

- [Key Features]({% slug button-key-features%})
- [Circular Button]({% slug button-howto-create-circle-button%})
- [Button with disabled text color]({% slug button-howto-textcolor-disabled-button%})