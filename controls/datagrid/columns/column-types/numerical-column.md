---
title: Numerical Column
page_title: Numerical Column
position: 1
slug: datagrid-columns-numerical-column
---

# DataGrid NumericalColumn

The **DataGridNumericalColumn** is used to represent only numerical values. It uses an entry control to edit the value in EditMode. The difference between this column and the text one is that it will directly invoke the numeric keyboard on the mobile devices

## Important Properties

* **PropertyName**: Specifies the name of the property of the object type that represents each row within the grid.
* **HeaderText**: Defines the content to be displayed in the Header UI that represents the column.
* **CellContentStyle**: Defines the Style object that defines the appearance of each cell associated with this column. The TargetType of the Style should be TextBlock type.
* **CellContentStyleSelector**: Defines the StyleSelector instance that allows for dynamic appearance on a per cell basis.
* **CellContentFormat**: Defines the custom format for each cell value. The String.Format routine is used and the format passed should be in the form required by this method.

>tip More information about **CellDecorationStyle** and  **CellDecorationStyleSelector** can be found in [Columns Styling]({%slug datagrid-columns-styling%}) topic.

>important **CellContentFormat** uses the format string provided by the framework. For more details check the [Standard Numeric Formatting](https://docs.microsoft.com/en-us/dotnet/standard/base-types/standard-numeric-format-strings) and [Custom Numeric Formatting](https://docs.microsoft.com/en-us/dotnet/standard/base-types/custom-numeric-format-strings) articles.

## Example

```XAML
<telerikGrid:DataGridNumericalColumn PropertyName="StadiumCapacity" 
                                     HeaderText="Stadium Capacity"
                                     CellContentFormat=" Seats - {0:D}">
    <telerikGrid:DataGridNumericalColumn.CellContentStyle>
        <telerikGrid:DataGridTextCellStyle TextColor="Green" 
                                           FontSize="18" 
                                           SelectedTextColor="LightCoral" />
    </telerikGrid:DataGridNumericalColumn.CellContentStyle>
</telerikGrid:DataGridNumericalColumn>
```

![Numerical Column](images/numericalcolumn-overview.png)

## See Also

- [Columns Styling]({%slug datagrid-columns-styling%})
- [Boolean Column]({%slug datagrid-columns-boolean-column%})
- [Date Column]({%slug datagrid-columns-date-column%})