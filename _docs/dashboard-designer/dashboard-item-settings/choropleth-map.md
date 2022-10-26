---
title: Choropleth Map
layout: default
nav_order: 8
parent: Dashboard Item Settings
grand_parent: Dashboard Designer
---
# Choropleth Map
The topics in this section describe the features available in the Choropleth Map dashboard item, that allows you to colorize the required areas in proportion to the provided values.

![wdd-dashboard-items-choropleth-map](../../../images/img125119.png)

## Providing Data
The **Web Dashboard** allows you to bind various dashboard items to data in a virtually uniform manner. To learn more, see the [Bind Dashboard Items to Data](../../bind-dashboard-items-to-data.md) topic.

The only difference is in the data sections that the required dashboard item has. This topic describes how to bind a **Choropleth Map** dashboard item to data.

### Binding to Data in the Web Dashboard
The image below shows a sample Choropleth Map dashboard item that is bound to data.

![wdd-choropleth-map-binding](../../../../images/img125398.png)

To bind the Choropleth Map dashboard item to data, click a placeholder contained in one of the available data sections and select the required data source field in the **Binding** section of the invoked [data item menu](../../ui-elements/data-item-menu.md).

The list below illustrates the Choropleth Map's data sections.
* **Attribute** - Processed as _Dimension_ - Allows you to associate map shapes with data source field values. To learn more about attributes, see the [Map Attributes](providing-maps.md) section.
* **Maps** - Processed as _Measure_ - Contains data items whose values are used to color map shapes. Map shape colors vary based on the map type.
	
	By default, map shapes are colored depending on the provided values. If you add an additional target value, the coloring of map shapes depends on the difference between two values called [Delta](delta.md).
* **Tooltip Measures** - Processed as _Measure_ - Allows you to add supplementary content to the tooltips. Add the required measures to provide additional data.
	
	![wdd-choropleth-map-tooltips](../../../../images/img125400.png)


## Delta
The Choropleth Map allows you to indicate the difference between the actual and target values of a particular parameter. This difference is called **delta**.

By default, map shapes are colored depending on the values provided. If you add an additional target value to create delta, the coloring of map shapes depends on the difference between two values.

![wdd-choropleth-map-delta](../../../../images/img125405.png)

### Add Delta
**Delta** is bound to two measures that provide two values: the _Actual_ value and the _Target_ value. The difference between these values is displayed on the map.

When you switch the map type to _Delta_, a new **Target** data item container appears.

![wdd-choropleth-map-add-delta](../../../../images/img125406.png)

Click it to open the target [data item menu](../../ui-elements/data-item-menu.md) and provide data for the target value.

### Delta Options
To specify delta indication settings, go to the **Delta Options** section of the [data item menu](../../ui-elements/data-item-menu.md). Here you can specify the delta display mode (e.g., value or bar), value type, result indication, comparison tolerance, etc.

The following options are available.

| Option | Description |
|---|---|
| **Value Type** | Specifies which values to display within map tooltips as the delta value. |
| **Result Indication** | Specifies the condition that will be used to select the indicator color. |
| **Threshold Type** | Specifies the comparison tolerance in percentage values or in absolute values. You can specify that a required indicator should only be displayed when the difference between the actual and target values exceeds a specified value. |
| **Threshold Value** | Specifies the comparison tolerance value. |


## Map Navigation
The Choropleth Map dashboard item allows you to perform navigation actions such as zooming and scrolling using the mouse.

You can enable or disable the capability to scroll/zoom the map using the **Lock Navigation** setting in the Choropleth Map's [Options](../../ui-elements/dashboard-item-menu.md) menu.

![wdd-map-lock-navigation](../../../../images/img125404.png)

To display the entire map within the dashboard item, use the **Initial Extent** button (the ![wdd-map-initial-size-icon](../../../../images/img125402.png) icon) in the Choropleth Map's [caption](../../dashboard-layout/dashboard-item-caption.md).

![wdd-choropleth-map-initial-state](../../../../images/img125403.png)


## Interactivity
To enable interaction between the **Choropleth Map** and other dashboard items, you can use the interactivity features. These features include **Master Filtering**.

### Master Filtering
You can use the **Choropleth Map** dashboard item as a filter for other dashboard items.

The Choropleth Map dashboard item supports filtering by shapes. When Master Filtering is enabled, you can click a shape (or multiple shapes) to make other dashboard items only display data related to the selected shape(s).

![wdd-choropleth-map-master-filter-interativity](../../../../images/img125414.png)

To learn more about filtering concepts common to all dashboard items, see the [Master Filtering](../../interactivity/master-filtering.md) topic.

To enable **Master Filtering**, go to the Choropleth Map's [Interactivity](../../ui-elements/dashboard-item-menu.md) menu and select the required Master Filtering mode.

![wdd-interactivity-section-without-drill-down](../../../../images/img125455.png)

To reset filtering, use the **Clear Master Filter** button (the ![wdd-master-filtering-icon](../../../../images/img125072.png) icon) in the Choropleth Map's [caption](../../dashboard-layout/dashboard-item-caption.md).

## Labels
A Choropleth Map provides the capability to display titles within map shapes and allows you to manage what data to show in the shape tooltips.

To manage map titles and tooltips, go to the **Shape Labels** section of the Choropleth Map's [Options](../../ui-elements/dashboard-item-menu.md) menu.

![wdd-choropleth-map-shape-labels](../../../../images/img125421.png)

The following settings are available.

| Option | Description |
|---|---|
| **Shape Title Attribute** | Allows you to select the attribute whose values are displayed within corresponding map shapes. Summary values are included to shape titles by default. |
| **Tooltip Attribute** | Allows you to configure information related to a hovered shape. You can choose whether to use a binding attribute to display as the title of shape tooltips (the **Use binding attribute** value) or specify a custom attribute from the dropdown list. |

## Legend
A **legend** is an element of a map that shows values corresponding to each color.

To display a legend within a map, open the Choropleth Map's [Options](../../ui-elements/dashboard-item-menu.md) menu and go to the **Color Legend** section.

![wdd-choropleth-map-legend](../../../../images/img125418.png)

The following options are available.

| Option | Description |
|---|---|
| **Show Legend** | Allows you to control the visibility of legend. |
| **Position** | Specifies the legend's position on a map. |