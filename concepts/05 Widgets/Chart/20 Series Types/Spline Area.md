The *splineArea* series type is useful when you need to emphasize a change in values, but smooth the line that connects the points. With this series type, data is displayed as points joined using a spline interpolation, and the shaded area between the spline and the argument axis. The joining line is the series' border, and it is not visible by default.

![SplineAreaSeriesType ChartJS](/images/ChartJS/SplineArea.png)

To use this series type, assign *'splinearea'* to the **type** property of the **series** configuration object.

    <!--JavaScript-->var chartOptions = {
        // ...
        series: {
            type: 'splinearea'
        }
    };

To learn how to specify data for a series, refer to the [Data Binding](/concepts/05%20Widgets/zz%20Common/10%20Data%20Visualization%20Widgets/85%20Charts%20-%20Data%20Binding/10%20Provide%20Data '/Documentation/Guide/Widgets/Common/Data_Visualization_Widgets/Charts_-_Data_Binding/Provide_Data/') topic.

To change the series default appearance, set the options of the **series** configuration object. For instance, you can change the following.

*   **Area Color**  
    A color from the chart's [palette](/concepts/05%20Widgets/zz%20Common/10%20Data%20Visualization%20Widgets/70%20Appearance%20Customization/1%20Palettes/10%20Palettes.md '/Documentation/Guide/Widgets/Common/Data_Visualization_Widgets/Appearance_Customization/#Palettes') is used by default. Set a custom color using the series' [color](/api-reference/20%20Data%20Visualization%20Widgets/dxChart/5%20Series%20Types/CommonSeries/color.md '/Documentation/ApiReference/Data_Visualization_Widgets/dxChart/Configuration/commonSeriesSettings/#color') property. This color will be used for the series' border. The color of the series area will be the same, but a specified [opacity](/api-reference/20%20Data%20Visualization%20Widgets/dxChart/5%20Series%20Types/CommonSeries/opacity.md '/Documentation/ApiReference/Data_Visualization_Widgets/dxChart/Series_Types/AreaSeries/#opacity') will be applied.
    
*   **Border Options**  
    Make a border visible by setting the **visible** property of the series' [border](/api-reference/20%20Data%20Visualization%20Widgets/dxChart/5%20Series%20Types/CommonSeries/border '/Documentation/ApiReference/Data_Visualization_Widgets/dxChart/Configuration/commonSeriesSettings/border/') object. When the border is visible, you can change its width, color and style, using the **width**, **color** and **dashStyle** properties of the series' **border** object. In addition, you can change the border settings when the series is hovered or selected. To do this, set the properties of the **border** object within the series' [hoverStyle](/api-reference/20%20Data%20Visualization%20Widgets/dxChart/5%20Series%20Types/CommonSeries/hoverStyle '/Documentation/ApiReference/Data_Visualization_Widgets/dxChart/Series_Types/SplineAreaSeries/hoverStyle/') or [selectionStyle](/api-reference/20%20Data%20Visualization%20Widgets/dxChart/5%20Series%20Types/CommonSeries/selectionStyle '/Documentation/ApiReference/Data_Visualization_Widgets/dxChart/Series_Types/SplineAreaSeries/selectionStyle/') configuration object.
    
*   **Points**  
    Make points visible by setting the **visible** property of the series' [point](/api-reference/20%20Data%20Visualization%20Widgets/dxChart/5%20Series%20Types/CommonSeries/point '/Documentation/ApiReference/Data_Visualization_Widgets/dxChart/Configuration/commonSeriesSettings/point/') object. For details on other point options, refer to the [Series Points](/concepts/05%20Widgets/Chart/10%20Visual%20Elements/020%20Series%20Points/10%20Series%20Points.md '/Documentation/Guide/Widgets/Chart/Visual_Elements/#Series_Points') topic.
    
*   **Point Labels**  
    Make point labels visible by setting the **visible** property of the series' [label](/api-reference/20%20Data%20Visualization%20Widgets/dxChart/5%20Series%20Types/SplineAreaSeries/label '/Documentation/ApiReference/Data_Visualization_Widgets/dxChart/Series_Types/SplineAreaSeries/label/') object. For details on other label options, refer to the [Series Point Labels](/concepts/05%20Widgets/Chart/10%20Visual%20Elements/030%20Series%20Point%20Labels.md '/Documentation/Guide/Widgets/Chart/Visual_Elements/#Series_Point_Labels') topic.

These and other options that can be set for series of the splineArea type are explained in the [SplineAreaSeries](/api-reference/20%20Data%20Visualization%20Widgets/dxChart/5%20Series%20Types/SplineAreaSeries '/Documentation/ApiReference/Data_Visualization_Widgets/dxChart/Series_Types/SplineAreaSeries/') Reference section. Set the required series options within the [series](/api-reference/20%20Data%20Visualization%20Widgets/dxChart/1%20Configuration/series '/Documentation/ApiReference/Data_Visualization_Widgets/dxChart/Configuration/series/') object of the chart's configuration object.

<a href="http://js.devexpress.com/Demos/WidgetsGallery/#demo/chartschartsareaseriesspline/" class="button orange small fix-width-155" style="margin-right: 20px;" target="_blank">View Demo</a>