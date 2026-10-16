# ELMA-IoT MIE

![ELMA-IoT MIE](assets/mie.png)

**ELMA-IoT MIE** is a portable Windows equipment-list and schematic-library application, part of [ELMA-IoT](https://github.com/elma-iot).

## Version 1.2

- Portable single EXE with the ELMA-IoT animated startup logo and green application icon.
- Master equipment tables with search, direct editing, existing dropdown choices, typed dates and session undo/redo.
- Save/Discard/Cancel protection before closing or replacing unsaved work.
- Duplicate serial highlighting and hover explanations showing matching records within the same equipment category.
- Linked schematics with native grouped-vector rendering and export to XLSX, PDF, PNG or JPEG; multi-page image exports retain all pages.
- Reusable Illustration Library with enlarged previews and independent placement dimensions, scale, rotation and flips.
- File, View, Language and Help menus, contextual tooltips and button press feedback.
- Interactive searchable user guide with a navigation tree.
- Twenty offline interface languages, live switching, Arabic/Persian interface direction and external JSON catalogs for adding languages. Imported data retains its original text.
- Save project as XLSX restores the master workbook and linked Schematics folder for further editing in Excel.

## Requirements and formats

Windows 10/11 with .NET Framework 4.8. Microsoft Excel is required on the importing PC to render XLSX schematics. Saved drawings can be viewed without Excel. Source workbooks are opened read-only with macros, events and external link updates disabled. No application macros are used.

Native XLSX drawings retain their editable source objects. PDF-origin XLSX exports are labelled image-based references, with original PDFs preserved alongside them. PDF export uses Excel when available and otherwise renders the saved pages at 300 dpi. PNG and JPEG exports use 300 dpi.

## Repository scope

This public repository provides application information and branding. Source is maintained privately. No operational data, customer drawings, imported projects, generated exports or data-bearing executables are published here.

Copyright (c) 2026 ELMA IoT. All rights reserved. This information page does not grant a license to the application source or organizational branding.
