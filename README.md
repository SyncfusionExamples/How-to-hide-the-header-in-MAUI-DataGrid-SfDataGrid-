# How-to-hide-the-header-in-MAUI-DataGrid-SfDataGrid-

This short guide shows how to hide (collapse) the header row in the Syncfusion .NET MAUI DataGrid (SfDataGrid) by setting the `HeaderRowHeight` property. The sample project in this repository demonstrates the technique; see the `MainPage.xaml` sample for a minimal implementation.

To learn more about these features, check out the official user guide topics:
- [Getting Started with .NET MAUI DataGrid](https://help.syncfusion.com/maui/datagrid/getting-started)

## XAML 

Set the header row height to 0 in XAML to collapse the header row visually. The snippet below is taken from the sample `MainPage.xaml` in this repo and demonstrates the exact property to change:

```xml
<ContentPage.BindingContext>
    <local:ViewModel x:Name="ViewModel"></local:ViewModel>
</ContentPage.BindingContext>

<syncfusion:SfDataGrid x:Name="dataGrid"
                        HeaderGridLinesVisibility="Both" 
                        GridLinesVisibility="Both"
                        HeaderRowHeight="0" 
                        ItemsSource="{Binding OrderInfoCollection}">
</syncfusion:SfDataGrid>
```
**Reference Image**

![HideHeaderRow](HideHeaderRow.png)

## How it works

- The `SfDataGrid.HeaderRowHeight` property controls the height of the header row. Setting it to `0` instructs the control to collapse the header row so it does not occupy any vertical space in the rendered UI.
- Grid line visibility properties such as `HeaderGridLinesVisibility` and `GridLinesVisibility` are independent and control whether grid lines are drawn for header/body cells.
- Hiding the header can be useful for very compact presentations or when column headers are redundant (for example, when using labeled UI or tooltips elsewhere).



## Conclusion

I hope you enjoyed learning about how to hide the header row in .NET MAUI DataGrid (SfDataGrid).
 
You can refer to our [.NET MAUI DataGrid’s feature tour](https://www.syncfusion.com/maui-controls/maui-datagrid) page to learn about its other groundbreaking feature representations. You can also explore our [.NET MAUI DataGrid Documentation](https://help.syncfusion.com/maui/datagrid/getting-started) to understand how to present and manipulate data. 
For current customers, you can check out our .NET MAUI components on the [License and Downloads](https://www.syncfusion.com/sales/teamlicense) page. If you are new to Syncfusion, you can try our 30-day [free trial](https://www.syncfusion.com/downloads/maui) to explore our .NET MAUI DataGrid and other .NET MAUI components.
 
If you have any queries or require clarifications, please let us know in the comments below. You can also contact us through our [support forums](https://www.syncfusion.com/forums), [Direct-Trac](https://support.syncfusion.com/create) or [feedback portal](https://www.syncfusion.com/feedback/maui?control=sfdatagrid), or the feedback portal. We are always happy to assist you!



