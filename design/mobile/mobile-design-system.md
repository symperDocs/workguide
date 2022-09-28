# Mobile Design System

## **FOUNDATION**

The Symper mobile design system is based on the foundation of [Material design](https://material.io/design/introduction) and has been customized for the idea and concept of the symper brand and product. This product is for Symper internal use and purpose.

Access design folder here: [`link`](https://ywb69zeduvn.sharepoint.com/:f:/s/Symper347/Eh0w7yH0OYlElXJuR3-r\_qgBTCqsNVWt8t2pc1pSnmlHLw?e=h4ayDI)

## **LAYOUT**

### **LAYOUT - GRID SYSTEM**

**What is a 4pt grid system?**

The 4pt grid system uses multiple sets of columns and rows based on the arithmetic sequence with 4pt of arithmetic ratio.

![](https://lh6.googleusercontent.com/PdCR1wsgM0HfMBVZY7YzvbTMdJl2kHvtzLCo-brWM3q5CJnhgOx2j3k0\_6sYEf\_TaRnBAUxBVM1MtPjgOi8T3fE1awN\_nuo4qXn3abyfEvU89Ig3f9CMlO2ro7hnFaDvDjJRF6Mc)

![](https://lh4.googleusercontent.com/XnyJMWo0R9Vw9RhL3GZyfyKpq5uDAo5K4JMD33PN1GMCMiLFxlaoXYkjP40KBwC4QKQFVyHnRgSbuPVubySwmu5LOr7DGnZ86Ecy8S2HuIcVBg6IjdNsH2ztwtGy9SOPyQYa3RNb)

**Baseline grid**

All components align to an 8dp square baseline grid for mobile, tablet, and desktop.

![](https://lh4.googleusercontent.com/n1Znkdd9e\_wGpajLg89iCa73cWQmbIUTNLHtvDHxdh\_sexn3AVBz0zslBItV72GafrNtfkmdhy4FkufZlPxKoKmHkTa0BelMJEtLQTekyTrcD1vMYLeMSndodQ67aQ0toicZ1\_NS)

Icons, type, and some elements within components can align to a 4dp grid.

![](https://lh3.googleusercontent.com/t8YA93Lq96mlPTd2h8TzqUd\_4zlaq26jCSpZNgELZgqokjnW4Hnw7fxDv\_XwaluonM5W6CBBSwsCFnFHUV9ri8b93JSeusIWV4Y7ASY\_blJ7ULjB5JY9U8S5wFkQqYvP20IrZMpQ)

### **LAYOUT - SCALING WITH TEXTS**

**40 - 60 characters**

The ideal line length for text is 40-60 characters. This maintains readability when scaling elements, such as cards, that contain text. When elements contain text, margins and typographic properties should be responsive to ensure that lines of text don’t extend too long in a horizontal layout.

When longer line lengths are necessary, consider adjusting the line height to improve readability

### **LAYOUT - COLUMNS, GUTTERS, AND MARGINS**

#### **COLUMNS**

Content is placed in the areas of the screen that contain columns.

In responsive layouts, column width is defined with percentages, rather than fixed values. This allows content to adapt to any screen size. The number of columns displayed in the grid is determined by the breakpoint range, a range of predetermined screen sizes. A breakpoint can correspond with mobile, tablet, or other screen type.

![](https://lh6.googleusercontent.com/OmiIcXQx541B5U8hRz\_7ggfPnshhPQtgQnWS6q7dikzo8pnYzygYsZwLr9MEFI8SIy37q9D1deNyYa3bCz6EAQ253G9b9OsAWUgWD5ehwDdvsDEbBV-w3ECJif-nqfFTr2f9Zi-D)

On mobile, at a breakpoint of 360 dp, this layout grid uses 4 columns.

#### **GUTTER**

A gutter is the space between columns that helps separate content. Gutter widths are fixed values at each breakpoint range. To better adapt to a given screen size, gutter widths can change at different breakpoints.

Wider gutters are more appropriate for larger screens, as they create more open space between columns.

![](https://lh5.googleusercontent.com/Ub11FoFsUY8AVqSR219sRl5rkUnnMgGNBbdXaMvswDHQNQik8EWyXeEqYzGke7S\_4zbztWfT5fwVVrPNJFgJHqdnvBdIp3aTIe9KKs8zaJVmDBIzNADr9RjlTqHf-Ove7wr9Ud5M)

On mobile, at a breakpoint of 360 dp, this layout grid uses 16dp gutters.

#### **MARGIN**

Margins are the space between content and the left and right edges of the screen.\
Margin widths are defined using fixed or scaling values at each breakpoint range. To better adapt to the screen, the margin width can change at different breakpoints. Wider margins are more appropriate for larger screens, as they create more whitespace around the perimeter of content.

![](https://lh5.googleusercontent.com/XK6ZSdSs2X4RfDxh1M\_BMlSVIzVh1wprpOWLVNoc1AR\_3-2w3tOe9ivEBpu-cYm6xRFWhLG2B5C5ZwtglRDrMcbYoTLKSsiFryZYUXG0e14Mx-mN1hRX0h43SECbT2yK4YMK6IwK)

On mobile, at a breakpoint of 360 dp, this layout grid uses 16dp margins.

**BREAKPOINTS**

A breakpoint is the screen size threshold determined by specific layout requirements. At a given breakpoint range, the layout adjusts to suit the screen size and orientation.\
Material Design provides responsive layouts based on 4-column, 8-column, and 12-column grids, available for use across different screens, devices, and orientations.\
Each breakpoint range determines the number of columns, and recommended margins and gutters for each display size.

**Breakpoint system**

The responsive layout grid is primarily used to organize content and components in a layout’s body region. Layout regions are described in detail in the Understanding layout guidance.\
When scaling a layout for different screen sizes or orientations, the responsive grid adjusts margin and body widths as well as the number of columns in the layout.

![](https://lh3.googleusercontent.com/n1FTKsaia1KwiIeMAajRMWJnFoHh-nODiAOBKpFzVxoE91p20ArbGR0CoYuQinCknfUFErFHCV2nLVN0ommMlqdoa\_iyS\_hTQo5Mkbz8fgQ1FodqEWiJyELckxtx9fnbTTs8nRUd)

### **LAYOUT - SPACING METHOD**

Spacing methods are more granular than the responsive layout grid. Spacing methods are a set of rules around how to place elements within layouts and components.

#### **Padding**

Padding is the space between elements within a component.\
Padding refers to the space between UI elements. Padding is an alternative spacing method to keylines and is measured in increments of 8dp or 4dp.\
Padding can be measured both vertically and horizontally and does not need to span the whole height of a layout.

![](https://lh3.googleusercontent.com/aHBkij4i9YiUToyK2QZ48eA3UIRTK5Lo72TUz9\_5epdDf24QowvKj4dzuxVPTo1mOOa56RMiEudLVeVSfry0wqgbXNW46WOlpgw2rZaAEc1I\_FVGX36oilAkGOvt5TMnIjLxCC0U)

#### **Dimensions**

Dimensions describe the width and height of component elements.\
Dimensions refer to the width and height of component elements. Some components, such as an app bar or list, only outline the height of an element. The heights of these elements should align to the 8dp grid. Their widths are not specified because it’s responsive to a viewport width.

![](https://lh3.googleusercontent.com/n\_0GLNvFzBWf4vHikplR\_9aqWX6blhGA1eD9xcW\_lilsPMXSrBy1AfDqpXbfebjuxHVVfBbTrt34BcT4hNIrNSDqJ-5T4JcDjfYdkrfea8A56DGU14aKEWO311wye0hgrvfRgdYf)

#### **Alignment**

Alignment is the placement of elements within a component.

![](https://lh5.googleusercontent.com/2FskaBaF7\_LtBvDPpuacM2MkT4vFUxwKq1HJZ15zwng5\_SbhxROog38GflFZ9I9SvhAwTgI-EEPdSWKgeKezJ46xFNjHMpkTSyeRbYsNS7uxyJKuJJvxaw\_ycnHak4Y5KmnHMYVy)

#### **Aspect ratios**

An aspect ratio is the proportion of an element’s width to its height. Aspect ratios are written as width:height.\
To maintain consistency in your layout, use a consistent aspect ratio on elements like images, surfaces, and screen size.\
The following aspect ratios are recommended for use across your UI: 16:9; 3:2; 4:3; 1:1; 3:4; 2:3

![](https://lh6.googleusercontent.com/RBY9-Nz0u4GQCPWEW0RwlICd2ylOI1HPjDUm6sFJs-g9T48\_vVHPI9F515i3Sdp4U1bsk9Vrm-EnTjzTLNCkk4K32aw5d2JlcACNEfk4cc7SVOYhFpi89OdA8fDEnRig7\_VaXlCV)

#### **Touch targets**

Touch targets apply to any device that receives both touch and non-touch input. To balance information density and usability, touch targets should be at least 48 x 48 dp with at least 8dp of space between targets.

![](https://lh5.googleusercontent.com/HCAsSmLUeyt69i9XM3WmT6vhpBzJO7-arAVkqw9rlYnUIcODPA8bHmzov7CXkA3EfxgfI6XdYcuNflxmy6LYQdzRrdD-QhtH8qVBNGseuxrJAl7lKrDflvRsScDsZM9H1Gq-lYiK)

## **TYPOGRAPHY**

### **Tyle scale**

![](https://lh5.googleusercontent.com/lltCJzgdSHZ6ljOqrfH5QzCeT568I0Rbb4PgG3Sl9gLwB-r6wCJxhLjBa7lu3BOEZ\_zexdEla067xHYO3PzQYkSuhVA9PIpzlopxM2CggbWx-NjWocEiuBO4Ta75lrst2LG1HYbo)

## **COLOR SYSTEM**

### **Color usage and palettes**

The Material Design color system helps you apply color to your UI in a meaningful way. In this system, you select a primary and a secondary color to represent your brand. Dark and light variants of each color can then be applied to your UI in different ways

### **Colors and theming**

Color themes are designed to be harmonious, ensure accessible text, and distinguish UI elements and surfaces from one another.

![](https://lh6.googleusercontent.com/FSv2Dsszi1gbEi\_SrIywzg-jKo2nNzT1MW9oHAuuVGMsPnbMa02\_Aaoaelu9hbmjdhmz0cUb3sCr9YTzZdBU235c-lK\_-\_0tjz3fWMdFhlS9JDtZ7vSQ5-oHOY2IUPhHw7Wc7hIi)

1. Primary color
2. Light and dark variants

### **Symper mobile color palettes**

The symper’s signature color presenting the brand, idea and concept

**Primary color palette**\
Primary color of the primary color palette is the Symper brand color and will be used for significant purposes and objects such as important buttons, highlight important text, tag, active stage of an object, selected item, etc.

![](https://lh5.googleusercontent.com/9WtGDmZpbnSg47FECsW9CkREuUIN-YJk7XCjKXStcbcbJeZ8ESOW2LiXyiYD5bXGzB4fHA89ZsmdiR1lktAw6seSGPdWuX8sXlAou21Tixe6KVzpdCC9rxF6A\_uHFDnftix5ZVQ-)

**Secondary color palette**

Secondary color palette is mostly used for normal and common objects, text, border, box, dialog, etc.

![](https://lh5.googleusercontent.com/tv7DeByht\_uJ9DCPywmd9HKY1kNYaaAf2AGJCyLCXYr-n0twSIGljq1Wm2YjiQhO882NYZCgu0DcM875E93mJAiYNF8DFiu8tDOwRh\_hCkKHqxLdPHX-LKnPALeFeGS1A8iPS52t)

**Positive object color palette**

Positive color palette is used for the positive object such as open button, approve button, selection, positive number, increase number, etc.

![](https://lh4.googleusercontent.com/UCpWtVYWTSUTsoZ-CdoZITr11WkkH\_t1wYq445\_RKuU9k3P1jk3RKcOuCu6Ox4dU6DlRxRouaTB7xKswzlygM61eu-RvumpdcS9RgK7JtISG2CPFzb4LpoEy7h5w3Oet3GrxGSjK)

**Negative object color palette**

Negative color palette is used for the negative object such as close button, reject button, unchecked stage of checkbox, negative number, decrease number, etc.

## **FOUNDATION**

The Symper mobile design system is based on the foundation of [Material design](https://material.io/design/introduction) and has been customized for the idea and concept of the symper brand and product. This product is for Symper internal use and purpose.

Access design folder here: [`link`](https://ywb69zeduvn.sharepoint.com/:f:/s/Symper347/Eh0w7yH0OYlElXJuR3-r\_qgBTCqsNVWt8t2pc1pSnmlHLw?e=h4ayDI)

## **LAYOUT**

### **LAYOUT - GRID SYSTEM**

**What is a 4pt grid system?**

The 4pt grid system uses multiple sets of columns and rows based on the arithmetic sequence with 4pt of arithmetic ratio.

![](https://lh6.googleusercontent.com/PdCR1wsgM0HfMBVZY7YzvbTMdJl2kHvtzLCo-brWM3q5CJnhgOx2j3k0\_6sYEf\_TaRnBAUxBVM1MtPjgOi8T3fE1awN\_nuo4qXn3abyfEvU89Ig3f9CMlO2ro7hnFaDvDjJRF6Mc)

![](https://lh4.googleusercontent.com/XnyJMWo0R9Vw9RhL3GZyfyKpq5uDAo5K4JMD33PN1GMCMiLFxlaoXYkjP40KBwC4QKQFVyHnRgSbuPVubySwmu5LOr7DGnZ86Ecy8S2HuIcVBg6IjdNsH2ztwtGy9SOPyQYa3RNb)

**Baseline grid**

All components align to an 8dp square baseline grid for mobile, tablet, and desktop.

![](https://lh4.googleusercontent.com/n1Znkdd9e\_wGpajLg89iCa73cWQmbIUTNLHtvDHxdh\_sexn3AVBz0zslBItV72GafrNtfkmdhy4FkufZlPxKoKmHkTa0BelMJEtLQTekyTrcD1vMYLeMSndodQ67aQ0toicZ1\_NS)

Icons, type, and some elements within components can align to a 4dp grid.

![](https://lh3.googleusercontent.com/t8YA93Lq96mlPTd2h8TzqUd\_4zlaq26jCSpZNgELZgqokjnW4Hnw7fxDv\_XwaluonM5W6CBBSwsCFnFHUV9ri8b93JSeusIWV4Y7ASY\_blJ7ULjB5JY9U8S5wFkQqYvP20IrZMpQ)

### **LAYOUT - SCALING WITH TEXTS**

**40 - 60 characters**

The ideal line length for text is 40-60 characters. This maintains readability when scaling elements, such as cards, that contain text. When elements contain text, margins and typographic properties should be responsive to ensure that lines of text don’t extend too long in a horizontal layout.

When longer line lengths are necessary, consider adjusting the line height to improve readability

### **LAYOUT - COLUMNS, GUTTERS, AND MARGINS**

#### **COLUMNS**

Content is placed in the areas of the screen that contain columns.

In responsive layouts, column width is defined with percentages, rather than fixed values. This allows content to adapt to any screen size. The number of columns displayed in the grid is determined by the breakpoint range, a range of predetermined screen sizes. A breakpoint can correspond with mobile, tablet, or other screen type.

![](https://lh6.googleusercontent.com/OmiIcXQx541B5U8hRz\_7ggfPnshhPQtgQnWS6q7dikzo8pnYzygYsZwLr9MEFI8SIy37q9D1deNyYa3bCz6EAQ253G9b9OsAWUgWD5ehwDdvsDEbBV-w3ECJif-nqfFTr2f9Zi-D)

On mobile, at a breakpoint of 360 dp, this layout grid uses 4 columns.

#### **GUTTER**

A gutter is the space between columns that helps separate content. Gutter widths are fixed values at each breakpoint range. To better adapt to a given screen size, gutter widths can change at different breakpoints.

Wider gutters are more appropriate for larger screens, as they create more open space between columns.

![](https://lh5.googleusercontent.com/Ub11FoFsUY8AVqSR219sRl5rkUnnMgGNBbdXaMvswDHQNQik8EWyXeEqYzGke7S\_4zbztWfT5fwVVrPNJFgJHqdnvBdIp3aTIe9KKs8zaJVmDBIzNADr9RjlTqHf-Ove7wr9Ud5M)

On mobile, at a breakpoint of 360 dp, this layout grid uses 16dp gutters.

#### **MARGIN**

Margins are the space between content and the left and right edges of the screen.\
Margin widths are defined using fixed or scaling values at each breakpoint range. To better adapt to the screen, the margin width can change at different breakpoints. Wider margins are more appropriate for larger screens, as they create more whitespace around the perimeter of content.

![](https://lh5.googleusercontent.com/XK6ZSdSs2X4RfDxh1M\_BMlSVIzVh1wprpOWLVNoc1AR\_3-2w3tOe9ivEBpu-cYm6xRFWhLG2B5C5ZwtglRDrMcbYoTLKSsiFryZYUXG0e14Mx-mN1hRX0h43SECbT2yK4YMK6IwK)

On mobile, at a breakpoint of 360 dp, this layout grid uses 16dp margins.

**BREAKPOINTS**

A breakpoint is the screen size threshold determined by specific layout requirements. At a given breakpoint range, the layout adjusts to suit the screen size and orientation.\
Material Design provides responsive layouts based on 4-column, 8-column, and 12-column grids, available for use across different screens, devices, and orientations.\
Each breakpoint range determines the number of columns, and recommended margins and gutters for each display size.

**Breakpoint system**

The responsive layout grid is primarily used to organize content and components in a layout’s body region. Layout regions are described in detail in the Understanding layout guidance.\
When scaling a layout for different screen sizes or orientations, the responsive grid adjusts margin and body widths as well as the number of columns in the layout.

![](https://lh3.googleusercontent.com/n1FTKsaia1KwiIeMAajRMWJnFoHh-nODiAOBKpFzVxoE91p20ArbGR0CoYuQinCknfUFErFHCV2nLVN0ommMlqdoa\_iyS\_hTQo5Mkbz8fgQ1FodqEWiJyELckxtx9fnbTTs8nRUd)

### **LAYOUT - SPACING METHOD**

Spacing methods are more granular than the responsive layout grid. Spacing methods are a set of rules around how to place elements within layouts and components.

#### **Padding**

Padding is the space between elements within a component.\
Padding refers to the space between UI elements. Padding is an alternative spacing method to keylines and is measured in increments of 8dp or 4dp.\
Padding can be measured both vertically and horizontally and does not need to span the whole height of a layout.

![](https://lh3.googleusercontent.com/aHBkij4i9YiUToyK2QZ48eA3UIRTK5Lo72TUz9\_5epdDf24QowvKj4dzuxVPTo1mOOa56RMiEudLVeVSfry0wqgbXNW46WOlpgw2rZaAEc1I\_FVGX36oilAkGOvt5TMnIjLxCC0U)

#### **Dimensions**

Dimensions describe the width and height of component elements.\
Dimensions refer to the width and height of component elements. Some components, such as an app bar or list, only outline the height of an element. The heights of these elements should align to the 8dp grid. Their widths are not specified because it’s responsive to a viewport width.

![](https://lh3.googleusercontent.com/n\_0GLNvFzBWf4vHikplR\_9aqWX6blhGA1eD9xcW\_lilsPMXSrBy1AfDqpXbfebjuxHVVfBbTrt34BcT4hNIrNSDqJ-5T4JcDjfYdkrfea8A56DGU14aKEWO311wye0hgrvfRgdYf)

#### **Alignment**

Alignment is the placement of elements within a component.

![](https://lh5.googleusercontent.com/2FskaBaF7\_LtBvDPpuacM2MkT4vFUxwKq1HJZ15zwng5\_SbhxROog38GflFZ9I9SvhAwTgI-EEPdSWKgeKezJ46xFNjHMpkTSyeRbYsNS7uxyJKuJJvxaw\_ycnHak4Y5KmnHMYVy)

#### **Aspect ratios**

An aspect ratio is the proportion of an element’s width to its height. Aspect ratios are written as width:height.\
To maintain consistency in your layout, use a consistent aspect ratio on elements like images, surfaces, and screen size.\
The following aspect ratios are recommended for use across your UI: 16:9; 3:2; 4:3; 1:1; 3:4; 2:3

![](https://lh6.googleusercontent.com/RBY9-Nz0u4GQCPWEW0RwlICd2ylOI1HPjDUm6sFJs-g9T48\_vVHPI9F515i3Sdp4U1bsk9Vrm-EnTjzTLNCkk4K32aw5d2JlcACNEfk4cc7SVOYhFpi89OdA8fDEnRig7\_VaXlCV)

#### **Touch targets**

Touch targets apply to any device that receives both touch and non-touch input. To balance information density and usability, touch targets should be at least 48 x 48 dp with at least 8dp of space between targets.

![](https://lh5.googleusercontent.com/HCAsSmLUeyt69i9XM3WmT6vhpBzJO7-arAVkqw9rlYnUIcODPA8bHmzov7CXkA3EfxgfI6XdYcuNflxmy6LYQdzRrdD-QhtH8qVBNGseuxrJAl7lKrDflvRsScDsZM9H1Gq-lYiK)

## **TYPOGRAPHY**

### **Tyle scale**

![](https://lh5.googleusercontent.com/lltCJzgdSHZ6ljOqrfH5QzCeT568I0Rbb4PgG3Sl9gLwB-r6wCJxhLjBa7lu3BOEZ\_zexdEla067xHYO3PzQYkSuhVA9PIpzlopxM2CggbWx-NjWocEiuBO4Ta75lrst2LG1HYbo)

## **COLOR SYSTEM**

### **Color usage and palettes**

The Material Design color system helps you apply color to your UI in a meaningful way. In this system, you select a primary and a secondary color to represent your brand. Dark and light variants of each color can then be applied to your UI in different ways

### **Colors and theming**

Color themes are designed to be harmonious, ensure accessible text, and distinguish UI elements and surfaces from one another.

![](https://lh6.googleusercontent.com/FSv2Dsszi1gbEi\_SrIywzg-jKo2nNzT1MW9oHAuuVGMsPnbMa02\_Aaoaelu9hbmjdhmz0cUb3sCr9YTzZdBU235c-lK\_-\_0tjz3fWMdFhlS9JDtZ7vSQ5-oHOY2IUPhHw7Wc7hIi)

1. Primary color
2. Light and dark variants

### **Symper mobile color palettes**

The symper’s signature color presenting the brand, idea and concept

**Primary color palette**\
Primary color of the primary color palette is the Symper brand color and will be used for significant purposes and objects such as important buttons, highlight important text, tag, active stage of an object, selected item, etc.

![](https://lh5.googleusercontent.com/9WtGDmZpbnSg47FECsW9CkREuUIN-YJk7XCjKXStcbcbJeZ8ESOW2LiXyiYD5bXGzB4fHA89ZsmdiR1lktAw6seSGPdWuX8sXlAou21Tixe6KVzpdCC9rxF6A\_uHFDnftix5ZVQ-)

**Secondary color palette**

Secondary color palette is mostly used for normal and common objects, text, border, box, dialog, etc.

![](https://lh5.googleusercontent.com/tv7DeByht\_uJ9DCPywmd9HKY1kNYaaAf2AGJCyLCXYr-n0twSIGljq1Wm2YjiQhO882NYZCgu0DcM875E93mJAiYNF8DFiu8tDOwRh\_hCkKHqxLdPHX-LKnPALeFeGS1A8iPS52t)

**Positive object color palette**

Positive color palette is used for the positive object such as open button, approve button, selection, positive number, increase number, etc.

![](https://lh4.googleusercontent.com/UCpWtVYWTSUTsoZ-CdoZITr11WkkH\_t1wYq445\_RKuU9k3P1jk3RKcOuCu6Ox4dU6DlRxRouaTB7xKswzlygM61eu-RvumpdcS9RgK7JtISG2CPFzb4LpoEy7h5w3Oet3GrxGSjK)

**Negative object color palette**

Negative color palette is used for the negative object such as close button, reject button, unchecked stage of checkbox, negative number, decrease number, etc.

![](https://lh3.googleusercontent.com/H-S96hbgNmvhbgEwtA\_UzQ-vixzAZFn45TR5R3RJyv8BGbo-Ym8xsOqaCwkTFRTvUXaF8zGncuTfdOxEKMIZ4o0Wcxra9q8b6rOpXrWSrW1PPJcX0cKxTfDN5Pc6KgIO9qP2a\_r8)
