---
title: Styling
page_title: Styling
description: Check our &quot;Styling&quot; documentation article for Telerik DateTimePicker for Xamarin control.
position: 8
slug: datetime-picker-styling
---

# Styling

Date and Time Picker control for Xamrin provides the following Style properties for customizing its look:

* **SpinnerStyle**(of type *Style* with target type **telerikDataControls:RadSpinner**): Defines the style applied to the spinner item and selected item.
* **SpinnerHeadersStyle**(of type *Style* with target type **Label**): Specifies the style applied to the spinner header labels.
* **SelectionHighlightStyle**(of type *Style* with target type **telerikPrimitives:RadBorder**): Specifies the style applied to the selection inside the popup. 
* **PlaceholderLabelStyle**(of type *Style* with target type **Label**): Defines the style applied to the placeholder label. 
* **DisplayLabelStyle**(of type *Style* with target type **Label**): Defines the style applied to the label which is visualized when date/time is selected.
* **TabStripStyle**(of type *Style* with target type **telerikPrimitives:TabViewHeader**)
* **TabStripItemStyle**(of type *Style* with target type **telerikInput:DateTimeSelectorTabStripItem**)
* **SelectorSettings**(*Telerik.XamarinForms.Input.PickerPopupSelectorSettings*):

Using the SelectorSettings property of the RadPickerBase class, you could style the dialog(popup) through the following properties:

* **PopupViewStyle**(of type *Style* with target type **telerikInput:PickerPopupContentView**): Defines the popup view style.
* **HeaderStyle**(of type *Style* with target type **telerikInput:PickerPopupHeaderView**): Defines the popup header style.
* **HeaderLabelStyle**(of type *Style* with target type **Label**): Defines the popup header label style.
* **FooterStyle**(of type *Style* with target type **telerikInput:PickerPopupFooterView**): Defines the popup footer style.
* **AcceptButtonStyle**(of type *Style* with target type **Button**): Defines the Accept button style.
* **CancelButtonStyle**(of type *Style* with target type **Button**): Defines the Cancel button style.

The SelectorSetting also provides the following properties for popup customization:

* **PopupOutsideBackgroundColor**(*Xamarin.Forms.Color*): Defines the color outside of the popup.
* **IsPopupModal**(*bool*): Defines a boolean value indicating if the popup should be closed when tapped outside of the popup. 
	When *IsPopupModal="True"*  the UI behind the popup gets inactive and cannot be used until the popup is closed. 
	When *IsPopupModal="False"* the popup could be closed when clicking outside the popup. 
	By default the value of the **IsPopupModal** is **false**.
* **HeaderLabelText**(*string*): Specifies the text visualized in the popup header.
* **AcceptButtonText**(*string*): Defines the text visualized for the accept button. By default the text is *OK*.
* **CancelButtonText**(*string*): Defines the text visualized for the cancel button. By default the text is *Cancel*. 

## Namespaces

Using **TabStripItemStyle**, **PopupViewStyle**, **HeaderStyle**, **FooterStyle** you will need to add the following namespace:

```XAML
xmlns:telerikInput="clr-namespace:Telerik.XamarinForms.Input;assembly=Telerik.XamarinForms.Input"
```

Using **SelectionHighlightStyle**, **TabStripStyle** you need to add the following namespace:

```XAML
xmlns:telerikPrimitives="clr-namespace:Telerik.XamarinForms.Primitives;assembly=Telerik.XamarinForms.Primitives"
```

Using **SpinnerStyle** you need to add the following namespace:

```XAML
xmlns:telerikInput="clr-namespace:Telerik.XamarinForms.Input;assembly=Telerik.XamarinForms.Input"
```

## Example

Here is a sample example that shows how the styling properties are applied.

A sample **List Picker** definition:

<snippet id='datetimepicker-style' />

and here are how the styles are defined in the page resources

## Spinner Style

<snippet id='datetimepicker-style-spinner-style' />

## SpinnerHeaders Style

<snippet id='datetimepicker-style-spinner-header-style' />

## SelectionHighlight Style

<snippet id='datetimepicker-style-selection-highlight-style' />

## PlaceholderLabel Style

<snippet id='datetimepicker-style-placeholder-label-style' />

## DisplayLabel Style

<snippet id='datetimepicker-style-display-label-style' />

## PopupView Style

<snippet id='datetimepicker-style-popupview-style' />

## Header Style

<snippet id='datetimepicker-style-header-style' />

## HeaderLabel Style

<snippet id='datetimepicker-style-header-label-style' />

## Footer Style

<snippet id='datetimepicker-style-footer-style' />

## AcceptButton Style

<snippet id='datetimepicker-style-accept-button-style' />

## CancelButton Style

<snippet id='datetimepicker-style-cancel-button-style' />

## Namespaces

In addition, add the following namespaces:

```XAML
xmlns:telerikInput="clr-namespace:Telerik.XamarinForms.Input;assembly=Telerik.XamarinForms.Input"
xmlns:telerikDataControls="clr-namespace:Telerik.XamarinForms.DataControls;assembly=Telerik.XamarinForms.DataControls"
xmlns:telerikPrimitives="clr-namespace:Telerik.XamarinForms.Primitives;assembly=Telerik.XamarinForms.Primitives"
```

This is how the Date and Time Picker control looks when the styles described above are applied:

![Date and Time Picker](images/datetimepicker_style.png)

>important A sample Styling example can be found in the DateTimePicker/Features folder of the [SDK Samples Browser application]({%slug developer-focused-examples%}).

## See Also

- [Key Features]({%slug datetime-picker-key-features%})
- [Custom Templates]({%slug datetime-picker-templates%})
- [Commands]({%slug datetime-picker-commands%})
- [Visual Structure]({%slug datetime-picker-visual-structure%})