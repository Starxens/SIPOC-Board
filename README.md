# Interactive SIPOC Board

A simple, web-based tool for creating and managing SIPOC (Suppliers, Inputs, Process, Outputs, Customers) diagrams for workshop sessions or process analysis. Built using HTML, CSS (Tailwind CSS), and vanilla JavaScript.

## Features

* **Process-Centric View:** Each process step has its own dedicated row with columns for Suppliers, Inputs, Outputs, and Customers.
* **Add/Edit Notes:** Easily add new process groups and add/edit individual notes within each SIPOC category (Suppliers, Inputs, Outputs, Customers) and for the Process itself.
* **Delete Items:** Remove individual notes or entire process group rows.
* **Local Storage Persistence:** Your board state is automatically saved in your browser's local storage, so your work persists between sessions on the same browser.
* **CSV Export:** Export the current state of the board to a CSV file (one row per process group).
* **CSV Import:** Import a previously exported CSV file to restore the board state (overwrites current board).
* **CSV Import to Excel:** The exported CSV file can easily be imported and edited in Excel 

## How to Use

1.  **Open `SIPOCboard.html`:** Simply open the `SIPOCboard.html` file in your web browser.
2.  **Add Process Group:** Click the "Add New Process Group" button to create a new row for a process step.
3.  **Add Notes:**
    * Click the "+" button within the Suppliers, Inputs, Outputs, or Customers columns to add a new note to that category for the specific process row.
    * Type directly into the main "Process" text area to describe the process step.
4.  **Edit Notes:** Click into any text area (Process or sub-notes) and type to edit. Changes are saved automatically.
5.  **Delete Notes:**
    * Hover over a sub-note (Supplier, Input, Output, Customer) and click the small '×' that appears.
    * Click the larger '×' button at the top-right of a process group row to delete the entire row (including all its notes).
6.  **Save/Load:**
    * Click "Save Status (CSV)" to download the current board state as a CSV file.
    * Click "Import Status (CSV)" to load a previously saved CSV file (this will replace the current board).

## Files

* `SIPOCboard.html`: The main HTML structure. Custom CSS styles (works alongside Tailwind CSS loaded via CDN). Contains all the JavaScript logic for interactivity, saving, loading, import/export.


## License

This project is licensed under the MIT License - see the LICENSE file for details.
