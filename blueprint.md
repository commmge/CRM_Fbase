
# Project Blueprint

## Overview

This project is a sales tracking application. It allows users to manage sales offers, track their status, and view them in a filterable and sortable table. The application supports importing and exporting data in various formats.

## Implemented Features

*   **Offer Management:** Create, edit, and delete sales offers.
*   **Data Visualization:** View offers in a table with sorting and filtering capabilities.
*   **Data Persistence:** Data is stored locally in the browser's IndexedDB.
*   **Import/Export:** Import and export data in JSON and XLSX formats.

## Current Task: Enhance Import/Export Functionality

### Plan

1.  **Modify "Proposta ID" Field:**
    *   Change the input type for the "Proposta ID" to `number`.
    *   Set the minimum value to `0` and the maximum value to `99999`.
    *   Remove any logic that allows text in this field.

2.  **Improve Date Recognition:**
    *   Modify the import logic to correctly parse dates in the following formats:
        *   `yyyy-mm-dd`
        *   `dd-mm-yyyy`
        *   `yyyy/mm/dd`
        *   `dd/mm/yyyy`
    *   Ensure that the export function uses a consistent date format (`yyyy-mm-dd`).
