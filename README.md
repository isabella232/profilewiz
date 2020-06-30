![](profilewiz.png)

# ProfileWiz
A tool to support round-tripping between modular and flattened versions of profiles of data models expressed using OWL, JSON-Schema, SHACL etc.


## Status
In development, focussed on Use Case 1.


## Use Cases
1. **Flattened => Modular**  
Take a data model (such as an OWL ontology) containing copied (and potentially modified) versions of definitions from "standard" models, intended to document a profile of those external models, and build a better Modular version that contains clear expression of the intended constraints on the original model, and create implementation resources such as JSON-LD contexts with imports of reusable, cachable modules.
2. **Modular Model => Flattened**  
Take a modular profile hierarchy and create "flattened" versions with no requirement for imports
3. **Profile validity**  
Consistency checking of profiles with respect to their base specifications - do they break any of the specs' rules?
4. **Implementation => Models**  
Extract data models from implementation resources - such as JSON-schema and JSON-LD context documents


## Installation
Clone this repository.

run python profilewiz --help

or to install as a editable module

pip install -e <workingcopy>

TODO: replace with package install once stable


## Usage
usage:  
```
~$ profilewiz.py [-h] [-o [OUTPUT]] [-q] [-r] [-p P [P ...]] input
```

Create JSON context, schema and other views of an ontology

positional arguments:
```bash
  input                 input file containing ontology in TTL format
```

optional arguments:
```bash
  -h, --help            show this help message and exit
  -o [OUTPUT], --output [OUTPUT]
                        output file
  -q, --qnames_only     use qnames only for JSON elements
  -r, --force_relative  use relative filenames and cached copies for imports
  -p P [P ...], --profiles P [P ...]
                        file name or URL of profiles model with pre-configured
                        resource locations
```


## License
*Coming!*


## Contributing
This project encourages contributions and collaboration! Please create Issues for the code or, better, Pull Requests to enhance function. Contributions will be recognised in release notes and other documetation.

For more information on contributing, please contact us via the *Contact* details below.


## Contacts
*Coming!*
