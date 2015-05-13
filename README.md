# Data Package Registry

An MVP implementation of a Data Package registry. See [here](https://github.com/okfn/data.okfn.org/issues/184) for context.

## MVP

* A github repo with a `registry.csv` file
* Apart from the header, each row in `registry.csv` represents a Data Package Profile
* Each object represents a Data Package Profile, and has the following keys:
    * **id**: the identifier for the profile (eg: "openspending")
    * **title**: the human-readable name for the Profile (eg: "Open Spending Data Package")
    * **schema**: a URL to a valid json schema (eg: https://raw.githubusercontent.com/dataprotocols/schemas/master/data-package.json)
    * **specification**: a URL to the specification (eg: http://dataprotocols.org/tabular-data-package/)
* Launch with entries for "Data Package" and "Tabular Data Package"
* Accept new entries via pull request
* New entries need to have a fully documented specification, and a working schema in JSON Schema format
