# How to: Bind data to the Windows Forms DataGridView control
refer to https://docs.microsoft.com/en-us/dotnet/framework/winforms/controls/how-to-bind-data-to-the-windows-forms-datagridview-control

not finished yet.

The DataGridView control supports the standard Windows Forms data binding model, so it can bind to a variety of data sources. Usually, you bind to a BindingSource that manages the interaction with the data source. The BindingSource can be any Windows Forms data source, which gives you great flexibility when choosing or modifying your data's location. 

To connect a DataGridView control to data:
1. Implement a method to handle the details of retrieving the data. The following code example implements a `GetData` method that initializes a SqlDataAdapter, and uses it to populate a DataTable. It then binds the DataTable to the BindingSource.
2. In the form's Load event handler, bind the DataGridView control to the BindingSource, and call the `GetData` method to retrieve the data.

Populate the `connectionString` variable in the example with the values for your Northwind SQL Server sample database connection. Windows Authentication, also called integrated security, is a more secure way to connect to the database than storing a password in the connection string.
