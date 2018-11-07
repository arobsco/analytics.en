---
description: Column settings let you configure column formatting, some of which can be conditional.
seo-description: Column settings let you configure column formatting, some of which can be conditional.
seo-title: Column settings
title: Column settings
uuid: 151d66da-04f7-4d0f-985c-4fdd92bc1308
index: y
internal: n
snippet: y
---

# Column settings

Column settings let you configure column formatting, some of which can be conditional.

* [Column settings](../../../../analyze/analysis-workspace/build-workspace-project/column-row-settings/column-settings.md#section_C5A9C13553BF4BFDAD7FACE0139AECA3) 
* [Conditional formatting](../../../../analyze/analysis-workspace/build-workspace-project/column-row-settings/column-settings.md#section_3DD847151DA14914888A70FC4FD7BDFB)

## Column settings {#section_C5A9C13553BF4BFDAD7FACE0139AECA3}

To access [!UICONTROL Column Settings], drag a Freeform Table to the project, then click the gear icon in the column heading.

![](assets/column_settings.png)

You can edit settings **for multiple columns at once**. Just select multiple columns and click the settings icon of any one of those columns. Any changes that you make apply to all columns with cells selected in them. 

<table id="table_8E88BB3AC2DD4F679F2663392BB52C6C"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Element </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr>
 </thead>
 <tbody> 
  <tr> 
   <td colspan="2"> <p><b>Display in Table Cells</b> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><b>Number</b> </p> </td> 
   <td colname="col2"> <p>Determines if a cell shows/hides the numeric value for the metric. For example, if the metric is Page Views, the numeric value is the number of page views for the row item. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><b>Percent</b> </p> </td> 
   <td colname="col2"> <p>Determines if a cell shows/hides the percent value for the metric. For example, if the metric is Page Views, the percent value is the number of page views for the row item divided by the total page views for the column. </p> <p>Note:  We can show percentages greater than 100%, to be more accurate. We are also moving the upper bound cap to 1,000% to ensure columns can grow in widths too large. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><b>Anomalies</b> </p> </td> 
   <td colname="col2"> <p>Determines if anomaly detection is run on the values in this column. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><b>Wrap Header Text</b> </p> </td> 
   <td colname="col2"> <p>Lets you wrap the header text in Freeform tables to make headers more readable and tables more shareable. This is useful for .pdf rendering and for metrics with long names. Enabled by default. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><b>Interpret zero as no value</b> </p> </td> 
   <td colname="col2"> <p>For cells with a 0 value, determines whether to show a 0 or a blank cell. This is useful when you look at data for each day of a month, and some days haven’t happened yet. </p> <p>Instead of showing 0's for future dates, blank cells can be shown instead. Charts respect this setting as well (i.e., they do not showing a line or bar with 0 values when this setting is checked). </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><b>Background</b> </p> </td> 
   <td colname="col2"> <p>Determines if a cell shows/hides all cell formatting, including the bar graph and conditional formatting. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><b>Bar Graph</b> </p> </td> 
   <td colname="col2"> <p>Shows a horizontal bar graph representing the cell’s value relative to the total for the column. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><b>Conditional Formatting</b> </p> </td> 
   <td colname="col2"> <p>See the section below. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><b>Table Cell Preview</b> </p> </td> 
   <td colname="col2"> <p>Shows a preview of how each cell appears with the currently selected formatting options applied. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Conditional formatting {#section_3DD847151DA14914888A70FC4FD7BDFB}

Conditional formatting applies formatting to upper, midpoint, and lower limits that you can define. Applying conditional formatting (colors, etc) within Freeform tables is also automatically enabled on breakdowns, unless “Custom” limits are selected.

![](assets/conditional-formatting.png)

<table id="table_F6D59140C59F488381DC67C928417E51"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Element </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr>
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p><b>Conditional Formatting </b> </p> </td> 
   <td colname="col2"> <p> Applies the following colors to cells, based on data values: </p> 
    <ul id="ul_C5576513EB0242F081A3E6202C87C8B5"> 
     <li id="li_71D49604ADFA4015986E2221A9ABAAF9">Green: high values </li> 
     <li id="li_2640E80446F947CF8669C9BB57FB8B25">Yellow: midpoint values </li> 
     <li id="li_34FB34158E264C028EAB9E537C14A65C">Red: low values </li> 
    </ul> <p>Replacing a dimension in the table resets the conditional formatting limits. Replacing a metric recalculates the limits for that column (where a metric is on the X axis and a dimension is on the Y axis). </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><b>Use Percent Limits </b> </p> </td> 
   <td colname="col2"> <p>Allows you to use upper, midpoint, and lower limits based on percentage values for each metric. This works for metrics that are solely percentage based (like Bounce Rate) as well as for metrics that have a count and a percentage (like Page Views.) </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><b>Auto-generated </b> </p> </td> 
   <td colname="col2"> <p>Automatically generates limits for conditional formatting. The upper limit is the largest value in this column. The lower limit is the lowest, and the midpoint is the average of the upper and lower limits. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><b>Custom</b> </p> </td> 
   <td colname="col2"> <p>You can manually assign the values for the <span class="uicontrol"> Upper</span>, <span class="uicontrol"> Midpoint</span>, and <span class="uicontrol"> Lower Limit</span> fields for conditional formatting. This gives you the flexibility to determine when a column value becomes good, average, or poor. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><b>Table Cell Preview</b> </p> </td> 
   <td colname="col2"> <p>Shows a preview of how each cell appears with the currently selected formatting options applied. </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!MORE_LIKE_THIS]
>
>* [Manage data sources](t_sync_visualization.md#task_A73B065DC3834AFCA422E364A1468099)