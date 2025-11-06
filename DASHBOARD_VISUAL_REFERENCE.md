# Dashboard Visual Reference

## Dashboard Mock-up Structure

This document provides a visual reference for the expected dashboard layout and design.

## Layout Overview

```
╔═══════════════════════════════════════════════════════════════════════════════╗
║                                                                               ║
║                        🚴 BIKE SALES DASHBOARD 🚴                            ║
║                                                                               ║
╠═══════════════════════════════════════════════════════════════════════════════╣
║                                                                               ║
║  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐       ║
║  │   📊 KPI 1  │  │   📊 KPI 2  │  │   📊 KPI 3  │  │   📊 KPI 4  │       ║
║  │             │  │             │  │             │  │             │       ║
║  │    Total    │  │ Conversion  │  │   Average   │  │   Total     │       ║
║  │    Bikes    │  │    Rate     │  │   Buyer     │  │  Customers  │       ║
║  │    Sold     │  │             │  │   Income    │  │  Analyzed   │       ║
║  │             │  │             │  │             │  │             │       ║
║  │     53      │  │   53.0%     │  │  $66,226    │  │     100     │       ║
║  │             │  │             │  │             │  │             │       ║
║  └─────────────┘  └─────────────┘  └─────────────┘  └─────────────┘       ║
║                                                                               ║
║  ┌────────────────────────────────────────────────────────────────────────┐  ║
║  │                                                                        │  ║
║  │         AVERAGE INCOME BY CUSTOMER DEMOGRAPHICS                        │  ║
║  │                                                                        │  ║
║  │   $90K ┤                                                               │  ║
║  │        │     ██        ██                                              │  ║
║  │   $70K ┤   ████      ████      ██        ██                            │  ║
║  │        │ ██████    ██████    ████      ████                            │  ║
║  │   $50K ┤████████  ████████  ██████    ██████                           │  ║
║  │        │████████  ████████  ██████    ██████                           │  ║
║  │   $30K ┴────────┴────────┴────────┴────────                            │  ║
║  │          Married  Married   Single   Single                            │  ║
║  │           Male    Female    Male    Female                             │  ║
║  │                                                                        │  ║
║  │         ██ Purchased: Yes    ██ Purchased: No                          │  ║
║  │                                                                        │  ║
║  └────────────────────────────────────────────────────────────────────────┘  ║
║                                                                               ║
║  ┌───────────────────────────────────┐  ┌────────────────────────────────┐  ║
║  │                                   │  │                                │  ║
║  │  PURCHASES BY COMMUTE DISTANCE    │  │  CUSTOMER AGE DISTRIBUTION     │  ║
║  │                                   │  │                                │  ║
║  │   30 ┤        ●                   │  │   40 ┤                        │  ║
║  │      │       ╱ ╲                  │  │      │      ●──────●          │  ║
║  │   20 ┤      ●   ●                 │  │   30 ┤    ╱          ╲        │  ║
║  │      │     ╱     ╲                │  │      │   ●            ●       │  ║
║  │   10 ┤    ●       ●──●            │  │   20 ┤  ╱              ╲      │  ║
║  │      │                            │  │      │ ●                ●     │  ║
║  │    0 ┴──────────────────          │  │   10 ┴───────────────────     │  ║
║  │      0-1  1-2  2-5 5-10 10+       │  │      Young  Middle   Old      │  ║
║  │      Miles                        │  │      Adult    Age              │  ║
║  │                                   │  │                                │  ║
║  │  ─●─ Purchased Bikes              │  │  ─●─ Yes  ─●─ No              │  ║
║  │                                   │  │                                │  ║
║  └───────────────────────────────────┘  └────────────────────────────────┘  ║
║                                                                               ║
║  ┌────────────────────────────────────────────────────────────────────────┐  ║
║  │                                                                        │  ║
║  │              BIKE SALES PERFORMANCE BY REGION                          │  ║
║  │                                                                        │  ║
║  │   40 ┤                                                                 │  ║
║  │      │                                                                 │  ║
║  │   30 ┤    ████              ████              ████                     │  ║
║  │      │  ████████          ████████          ████████                   │  ║
║  │   20 ┤  ████████          ████████          ████████                   │  ║
║  │      │██████████        ████████████      ████████████                 │  ║
║  │   10 ┤██████████        ████████████      ████████████                 │  ║
║  │      │██████████        ████████████      ████████████                 │  ║
║  │    0 ┴──────────────────────────────────────────────                  │  ║
║  │         Europe       North America         Pacific                     │  ║
║  │                                                                        │  ║
║  │         ██ Purchased: Yes    ██ Purchased: No                          │  ║
║  │                                                                        │  ║
║  └────────────────────────────────────────────────────────────────────────┘  ║
║                                                                               ║
║  ┌──────────────────────────────────────────────────────────────────────┐   ║
║  │  FILTERS                                                             │   ║
║  │  ┌──────────┬──────────┬──────────┐                                  │   ║
║  │  │  Europe  │   N.A.   │ Pacific  │  Region                          │   ║
║  │  └──────────┴──────────┴──────────┘                                  │   ║
║  │  ┌──────────┬──────────┬──────────┐                                  │   ║
║  │  │  Young   │  Middle  │   Old    │  Age Bracket                     │   ║
║  │  └──────────┴──────────┴──────────┘                                  │   ║
║  │  ┌──────────┬──────────┐                                             │   ║
║  │  │ Married  │  Single  │  Marital Status                             │   ║
║  │  └──────────┴──────────┘                                             │   ║
║  │  ┌──────────┬──────────┐                                             │   ║
║  │  │   Male   │  Female  │  Gender                                     │   ║
║  │  └──────────┴──────────┘                                             │   ║
║  └──────────────────────────────────────────────────────────────────────┘   ║
║                                                                               ║
║  Last Updated: [Date]                          Data Source: Bike Sales DB   ║
║                                                                               ║
╚═══════════════════════════════════════════════════════════════════════════════╝
```

## Color Scheme Details

### Primary Palette
- **Success/Positive (Yes)**: #70AD47 (Green)
  - Used for: Purchased = Yes data series
  - RGB: (112, 173, 71)
  
- **Negative (No)**: #FF6B6B (Red) or #A6A6A6 (Gray)
  - Used for: Purchased = No data series
  - RGB Red: (255, 107, 107)
  - RGB Gray: (166, 166, 166)
  
- **Accent/Primary**: #4472C4 (Blue)
  - Used for: Single line charts, borders, accents
  - RGB: (68, 114, 196)
  
- **Secondary Accent**: #FFA500 (Orange)
  - Used for: Second data series in dual-line charts
  - RGB: (255, 165, 0)

### Background Colors
- **Dashboard Background**: #F2F2F2 (Light Gray)
  - RGB: (242, 242, 242)
  
- **Chart/Card Background**: #FFFFFF (White)
  - RGB: (255, 255, 255)
  
- **Grid Lines**: #D9D9D9 (Light Gray)
  - RGB: (217, 217, 217)

### Text Colors
- **Titles/Headers**: #262626 (Dark Gray)
  - Font: Calibri, Bold, 18-24pt
  - RGB: (38, 38, 38)
  
- **Body Text/Labels**: #595959 (Medium Gray)
  - Font: Calibri, Regular, 10-12pt
  - RGB: (89, 89, 89)
  
- **KPI Numbers**: #262626 (Dark Gray)
  - Font: Calibri, Bold, 28-36pt

## Component Specifications

### KPI Cards
- **Size**: 150px width × 100px height
- **Border**: 2px solid, color matches data type
- **Border Radius**: 10px (rounded corners)
- **Shadow**: Optional subtle drop shadow
- **Layout**: 
  - Top: Icon (emoji or small graphic)
  - Middle: Label text (12pt)
  - Bottom: Value (36pt, bold)

### Charts
- **Chart Area**: White background, no border
- **Plot Area**: White background
- **Title**: 16pt, Bold, Dark Gray
- **Axis Labels**: 10pt, Regular, Medium Gray
- **Data Labels**: 9pt, Regular, positioned on/near data points
- **Legend**: 10pt, positioned at bottom or right
- **Gridlines**: Horizontal only, light gray, subtle

### Slicers
- **Style**: Modern tile style with rounded corners
- **Button Size**: 100px × 35px
- **Spacing**: 5px between buttons
- **Active State**: Blue highlight (#4472C4)
- **Hover State**: Light blue background
- **Font**: 11pt, Segoe UI or Calibri

## Chart-Specific Details

### Chart 1: Average Income Bar Chart
- Type: Clustered Column
- Bar Width: 60% of category width
- Gap: 40% between categories
- Data Labels: On top of bars
- Y-Axis: $0 to $100K, increments of $20K
- Format: Currency with no decimals

### Chart 2: Commute Distance Line Chart
- Type: Line with Markers
- Line Width: 2.5pt
- Marker Size: 7pt
- Marker Shape: Circle
- Smooth Lines: No (angular for emphasis)
- Y-Axis: 0 to max+10%, integer values

### Chart 3: Age Distribution Line Chart
- Type: Line with Markers (two series)
- Line Width: 2.5pt
- Markers: Circle, 6pt
- Smooth Lines: Yes
- Y-Axis: 0 to max+10%, integer values
- Legend: Bottom center

### Chart 4: Regional Bar Chart
- Type: Clustered Column
- Bar Width: 70% of category width
- Gap: 30% between categories
- Data Labels: On top of bars
- Y-Axis: 0 to max+10%, integer values
- Secondary calculation: % rate above bars

## Responsive Considerations

### For Print (Letter/A4)
- Margin: 0.5 inches all sides
- Orientation: Landscape
- Scale: Fit to 1 page wide × 1 page tall
- Print Quality: High (600 DPI)

### For Screen Sharing
- Resolution: 1920×1080 minimum
- Zoom: 100% recommended
- No scrolling required
- All text readable at 3 feet distance

### For Mobile/Tablet
- Simplified single-column layout
- Larger text (minimum 14pt)
- Simplified charts (one metric per chart)
- Touch-friendly slicers (minimum 44px tap targets)

## Accessibility Features

### Color Blindness Considerations
- Don't rely solely on green/red distinction
- Use patterns or shapes in addition to colors
- Ensure sufficient contrast ratios (4.5:1 minimum)
- Provide text labels for all data points

### Screen Reader Compatibility
- Add alt text to all charts
- Use clear, descriptive labels
- Provide text summary of key insights
- Ensure logical tab order

### High Contrast Mode
- Test dashboard in Windows high contrast mode
- Ensure borders remain visible
- Verify text remains readable
- Check that colors don't disappear

## Interactive Behavior

### Slicer Interactions
1. Click slicer button → All connected charts filter
2. Multi-select: Hold Ctrl and click multiple options
3. Clear filters: Click funnel icon in slicer header
4. Visual feedback: Selected items highlighted in blue

### Chart Interactions
1. Hover over data point → Tooltip shows details
2. Click on legend item → Series shows/hides
3. Right-click → Context menu for chart options

### KPI Card Behavior
- Numbers update dynamically when filters applied
- Change color based on thresholds (optional):
  - Green: Above target
  - Yellow: Near target
  - Red: Below target

## Export Formats

### PDF Export
- Page Size: Letter (8.5" × 11")
- Orientation: Landscape
- Quality: High (600 DPI)
- Embed fonts: Yes
- Include: Dashboard sheet only

### Image Export
- Format: PNG with transparency
- Resolution: 300 DPI
- Dimensions: 1920×1080px (16:9)
- Usage: Presentations, reports, email

### Excel Workbook
- Protected sheets: All except Dashboard
- Allow: Filtering, Pivot Table refresh
- Password: Optional
- Include: All sheets or Dashboard-only version

## Version Control

### File Naming Convention
```
Bike_Sales_Dashboard_v[MAJOR].[MINOR]_[YYYY-MM-DD].xlsx

Examples:
- Bike_Sales_Dashboard_v1.0_2024-01-15.xlsx
- Bike_Sales_Dashboard_v1.1_2024-02-01.xlsx
- Bike_Sales_Dashboard_v2.0_2024-03-15.xlsx
```

### Version History Tracking
Maintain a version log in separate sheet:
- Version number
- Date created
- Changes made
- Author
- Notes

## Performance Optimization

### File Size Management
- Remove unused styles and formats
- Compress embedded images
- Clear pivot table cache periodically
- Delete hidden sheets not needed for distribution

### Calculation Speed
- Use manual calculation for large datasets
- Minimize volatile functions (NOW, RAND)
- Reference specific ranges, not entire columns
- Consider Power Pivot for 10K+ rows

### Refresh Speed
- Update data source only, not entire workbook
- Refresh visible sheets first
- Use background refresh for large data
- Schedule refresh during off-peak hours

## Quality Checklist

Before finalizing dashboard:
- [ ] All charts display correctly at 100% zoom
- [ ] KPIs show accurate calculations
- [ ] Slicers affect all relevant visualizations
- [ ] Colors are consistent with brand/scheme
- [ ] Text is readable without zooming
- [ ] No #REF, #N/A, or #DIV/0 errors
- [ ] Charts have clear titles and labels
- [ ] Legend is easy to understand
- [ ] Data source is documented
- [ ] Last updated date is current
- [ ] File is protected appropriately
- [ ] Tested on target Excel version
- [ ] PDF export looks professional
- [ ] All links and formulas work
- [ ] Dashboard fits on one screen

## Support and Maintenance

### Regular Updates
- **Daily**: Check for data refresh needs
- **Weekly**: Verify calculations accuracy
- **Monthly**: Review and update insights
- **Quarterly**: Major design refresh if needed
- **Annually**: Architecture review and optimization

### Issue Resolution
Common issues and solutions:
1. **Slow performance**: Reduce data size, optimize formulas
2. **Charts not updating**: Refresh all, check connections
3. **Formatting lost**: Reapply styles, check cell formats
4. **Print issues**: Adjust margins, scale, and page breaks
5. **Compatibility**: Save in Excel 97-2003 format if needed

---

This visual reference should be used in conjunction with the implementation guide to create a professional, functional bike sales dashboard.
