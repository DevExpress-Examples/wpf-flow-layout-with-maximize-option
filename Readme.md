<!-- default badges list -->
![](https://img.shields.io/endpoint?url=https://codecentral.devexpress.com/api/v1/VersionRange/128654202/22.2.2%2B)
[![](https://img.shields.io/badge/Open_in_DevExpress_Support_Center-FF7200?style=flat-square&logo=DevExpress&logoColor=white)](https://supportcenter.devexpress.com/ticket/details/E2260)
[![](https://img.shields.io/badge/📖_How_to_use_DevExpress_Examples-e9f6fc?style=flat-square)](https://docs.devexpress.com/GeneralInformation/403183)
<!-- default badges end -->

# WPF Flow Layout Control - Arrange Items Vertically and Enable Maximize Option 

This example creates a [WPF Flow Layout Control](https://docs.devexpress.com/WPF/8148/controls-and-libraries/layout-management/tile-and-layout/flow-layout-control). The form layout has four [groups](https://docs.devexpress.com/WPF/DevExpress.Xpf.LayoutControl.GroupBox). Each group contains a `TextBlock` control.

![WPF Flow Layout Control - Arrange Items Vertically and Enable Maximize Option ](https://raw.githubusercontent.com/DevExpress-Examples/how-to-display-items-in-flowlayoutcontrol-and-enable-maximization-feature-e2260/22.2.2%2B/i/wpf-flow-layout-control-devexpress.png)

## Enable Maximize Option

Use the [FlowLayoutControl.MaximizedElement](https://docs.devexpress.com/WPF/DevExpress.Xpf.LayoutControl.FlowLayoutControl.MaximizedElement) property to maximize the specified group (in this example this is the first group):

```xaml
<lc:FlowLayoutControl Orientation="Vertical" Background="#FFFAFAFA" BreakFlowToFit="True" 
			MaximizedElementPosition="Right" MaximizedElement="{Binding ElementName=groupBox1}">
    <lc:GroupBox x:Name="groupBox1" Header="Group 1" Style="{StaticResource  myGroupBoxStyle}">
        <TextBlock  TextWrapping="Wrap" Text="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed molestie porttitor congue..."/>
    </lc:GroupBox>
  ...
</lc:FlowLayoutControl>
```


## Files to Review

* [MainWindow.xaml](./CS/FlowLayoutControl_GroupBox/MainWindow.xaml) (VB: [MainWindow.xaml](./VB/FlowLayoutControl_GroupBox/MainWindow.xaml))


## Documentation

* [Flow Layout Control](https://docs.devexpress.com/WPF/8148/controls-and-libraries/layout-management/tile-and-layout/flow-layout-control)
* [MaximizedElementPosition](https://docs.devexpress.com/WPF/DevExpress.Xpf.LayoutControl.FlowLayoutControl.MaximizedElementPosition)
* [GroupBox.MaximizeElementVisibility](https://docs.devexpress.com/WPF/DevExpress.Xpf.LayoutControl.GroupBox.MaximizeElementVisibility)
* [GroupBox.State](https://docs.devexpress.com/WPF/DevExpress.Xpf.LayoutControl.GroupBox.State)
