## Project Plan

1. GUI Design:
The application window is created using Tkinter with the title "Manufacturer specific DTCs" and a specific background color.
Various widgets such as labels, entry fields, buttons, and a footer label are created and arranged using grid layout.
2. File Handling:
The program allows the user to browse and select specific Excel files using the file dialog.
File paths for the summary table, SAE J2012DA file, and Manufacturer DTC file are stored in the corresponding entry fields.
3. Data Processing:
The program defines a method called process_row that takes a row from the summary table and performs operations based on the fault code.
The fault code column index is obtained from a spinbox widget.
A mapping dictionary is created to associate fault code prefixes with specific SAE J2012DA sheets.
The method checks if the fault code prefix is valid and if the corresponding sheet exists in the SAE J2012DA file.
Based on different conditions, the method updates values in the "Kommentar Capgemini" column of the summary table.
4. Event Handlers:
Event handlers are defined for browse buttons to open file dialogs and update the corresponding entry fields.
The process_summary_table method is called when the "Process" button is clicked.
It retrieves the user input values, reads the summary table, SAE J2012DA file, and Manufacturer DTC file using Pandas.
A progress window with a progress bar is created to show the processing progress.
A separate thread is started to process each row of the summary table using the process_row method.
Upon completion, the processed summary table is saved to an output file with a specific naming convention.
Appropriate messages are displayed to indicate the completion or any errors that occurred during the process.
5. Error Handling:
The program incorporates basic error handling by displaying error messages in case of exceptions during file handling or processing.
Errors are shown as message boxes with relevant error information.