# diputils
Utilities to support the [**Data Innovation Program** (DIP)](https://www2.gov.bc.ca/gov/content/data/about-data-management/data-innovation-program). Generally Windows, Mac and Linux environments supported, some aspects may require POPDATA SRE to run

## Features

This package presently supports several big-data friendly operations for tabular data

Properties of data in DIP environment
- Zipped
- Quite large, potentially **up to tens of GB per file**
- Produced from DIP metadata available on BC Data Catalogue
- **Fixed width format** with data dictionary or header file specifying field names and widths

## Project Status

This project is currently developed and supported by DPD Partnerships and Capacity (PAC) branch

## Projects Supported incl.
CYMH / DIP Development proeject / Children in Care (in care network) / Educ. Special needs project / Race based data initiative (RBD)

## Contents by Directory:

THIS REPO HAS BEEN SLEEPING BUT IT WILL WAKE UP...STAY TUNED FOR UPDATES / WORKFLOW EXAMPLES..

#### [/](.//)
- **get_metadata.py**: fetch DIP metadata from BC Data Catalogue (BCDC)
- **make_fakedata.py**: synthesize DIP data from the above metadata
- **csv_to_fixedwidth.py**: convert CSV data to "fixed width" format
- **indent.py**: indent a code file
- **misc.py**: shared functions

## Usage:

#### get_metadata.py
Terminal:
```python3 get_metadata.py```
(Alternately, can open in Python IDLE and select RUN from menu, or press F5 key)

#### make_fakedata.py
Terminal:
```python3 make_fakedata.py```
(Alternately, can open in Python IDLE and select RUN from menu, or press F5 key)

Optional arguments:

```python3 make_fakedata.py [minimum number of rows, per file] [maximum number of rows, per file]```
* minimum number of rows, per file: lower bound for random number of rows of synthetic to generate
* maximum number of rows, per file: upper bound for random number of rows of synthetic to generate

**Notes:** CSV format synthetic data (.csv) are supplied alongside zipped fixed-width format synthetic data (.zip) for comparison. In the actual DIP environment
* data are provided in fixed-width format ONLY (no CSV files)
* the data dictionaries don't typically appear in the same folder as the fixed-width files they're associated with. Software for matching fixed-width files with data dictionaries, will soon be provided in this repository 

## Relevant Repositories

#### []()

## Getting Help
Please contact Ashlin.Richardson@gov.bc.ca for assistance or to provide feedback

## Contributors


## License

Copyright 2020 Province of British Columbia

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and limitations under the License.
