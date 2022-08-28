# mztabpy

[![Python application](https://github.com/bigbio/mztabpy/actions/workflows/python-app.yml/badge.svg)](https://github.com/bigbio/mztabpy/actions/workflows/python-app.yml)

Python library to handle mztab files. mzTab is a tab-delimited file format created by HUPO-PSI containing protein/peptide quantification and identification data. 


## Input
mzTab

## Output
Metadata, protein, peptide, and PSM subtables(.csv) or HDF5 file(.hdf5) with the four parts of information.

## Usage
`python mztabpy_click.py mztab_parse --mztab_path {mztab_path}
 --subtable {True or False}
 --hdf5 {True or False}
 --fillna {True or False}
 --filter {True or False}`

 ## Parameters
 -   --mztab_path: The path to mzTab
 -   --subtable: Whether to convert mzTab into subtables(.csv)
 -   --hdf5: Whether to convert mzTab into HDF5(.hdf5)
 -   --fillna: Whether to replace null values with "null"
 -   --filter: Whether to remove empty columns
