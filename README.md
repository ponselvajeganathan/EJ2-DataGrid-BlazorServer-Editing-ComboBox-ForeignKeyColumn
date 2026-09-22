# Blazor Server DataGrid - ComboBox Editing for Foreign Key Column

## Overview

This sample demonstrates how to edit a foreign key column in a Syncfusion [Blazor DataGrid](https://www.syncfusion.com/blazor-components/blazor-datagrid) by rendering a ComboBox editor for the related lookup field. The implementation uses an order collection as the primary grid data source and an employee collection as the lookup source for the foreign key relationship. During editing, users can select employee values through a ComboBox while the grid preserves the corresponding employee identifier in the underlying data model. This approach improves usability by presenting descriptive values instead of requiring users to work directly with numeric foreign key values.

## Key Features

- Uses the `Syncfusion.Blazor.Grids` namespace to render the DataGrid.
- Defines an `Order` model with the following fields:
  - `OrderID`
  - `EmployeeID`
  - `OrderDate`
  - `Freight`
- Defines an `EmployeeData` model with:
  - `EmployeeID`
  - `FirstName`
- Demonstrates editing of a foreign key field through a ComboBox-based editor.
- Uses a separate employee collection as the lookup source for employee names.
- Allows users to edit foreign key values through user-friendly text selections while maintaining the underlying relationship field.
- Generates sample data directly within `Pages/Index.razor` for demonstration purposes.

## Prerequisites

- Visual Studio 2022 or Visual Studio Code
- .NET SDK compatible with the project's target framework

## How to Run the Project

**Visual Studio 2022**

1. Clone or download this repository.
2. Open the solution file: `EditComboBoxwithForeignKey.sln`
3. Restore NuGet packages.
4. Set the startup project to: `EditComboBoxwithForeignKey`
5. Build the solution.
6. Run the application by pressing `Ctrl+F5`.
7. Open the local URL displayed by the application when it starts.
8. Edit a grid record and observe the ComboBox editor used for the foreign key field.

**Visual Studio Code**

1. Open the repository folder in Visual Studio Code.
2. Open the integrated terminal.
3. Navigate to the project directory.

```bash
cd EJ2-DataGrid-BlazorServer-Editing-ComboBox-ForeignKeyColumn
dotnet restore
dotnet run
```

4. Open the local URL displayed in the terminal after the application starts.
5. Navigate to the sample page and edit a record to view the foreign key ComboBox editing behavior.

## Project Structure

`Pages/Index.razor` — contains the DataGrid implementation, sample data generation logic, foreign key editing configuration, and the `Order` and `EmployeeData` model definitions.

## Support and Feedback

- For general product questions, visit the [Syncfusion Community Forum](https://www.syncfusion.com/forums) or [Syncfusion Support](https://www.syncfusion.com/support).
- To report an issue specific to this sample, open a GitHub issue in this repository.
- For official documentation related to DataGrid foreign key columns, visit https://help.syncfusion.com/grid-sdk/blazor/data-grid/foreignkey-column

## License

This is a Syncfusion sample project provided to demonstrate product usage. Review the [Syncfusion license terms](https://www.syncfusion.com/sales/pricing?category=ui-components) before using Syncfusion components in your own applications.
