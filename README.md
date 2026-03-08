# Document Background Grid for Measuring Typesetting in Various Units

Semester project for the BI-TEX course, Adam Barla, SS 2020/2021

This project is a tool for positioning typesetting. It is a macro for `OpTeX` designed to help find causes of incorrect typesetting placement or to determine the exact position of text in a document.
The macro creates a grid on the background of every page of your document without altering the existing text layout. However, any existing background defined in `\pgbackground` will be overwritten. You can define both the cell size and the overall grid size yourself.

## Documentation

A detailed description of the macro's usage and development can be found in the file `documentation.pdf`, located in the `\doc` folder. You can generate it with the command:

`optex documentation.tex`

In the same folder, you will also find three usage examples. They are described in more detail in the documentation.

## Quick Usage

The macro definition can be found in the file `grid.tex` in the `macro` folder. You must include this file in your document using `\include grid.tex`. Then you can use it with default settings by running:

`\grid ,(,,,)`

or you can define the grid parameters:

`\grid <horizontal spacing>,<vertical spacing>(<left margin>,<top margin>, <horizontal size>,<vertical size>)`

When defining parameters, you can leave some of them empty, in which case they will be set to their default values. Specify parameters with units defined in `TeX` (pt, in, mm, cm, etc.).

The `macro` folder also contains a test text used for the examples shown in the documentation.
