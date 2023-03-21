# How-to-hide-the-header-in-MAUI-DataGrid-SfDataGrid-

The .NET [MAUI DataGrid](https://www.syncfusion.com/maui-controls/maui-datagrid)(SfDataGrid) allows to customize the height of the header row by setting the SfDataGrid.HeaderRowHeight property.

## XAML

When Setting [HeaderRowHeight](https://help.syncfusion.com/cr/maui/Syncfusion.Maui.DataGrid.SfDataGrid.html#Syncfusion_Maui_DataGrid_SfDataGrid_HeaderRowHeight) to 0 will collapse the header row in the view.

```XML
<syncfusion:SfDataGrid x:Name="dataGrid"
                           HeaderGridLinesVisibility="Both" 
                           GridLinesVisibility="Both"
                           HeaderRowHeight="0" 
                           ItemsSource="{Binding OrderInfoCollection}" >
    </syncfusion:SfDataGrid>
```

![HideHeaderRow](HideHeaderRow.png)

