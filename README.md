# Data Package Registry

This is a basic (minimum viable product) registry of profiles of [Data Packages](http://data.okfn.org/doc/data-package). In the future, a more sophisticated implementation may replace it. See [here](https://github.com/okfn/data.okfn.org/issues/184) for the rationale behind it.

## How it works

* The registry is maintained as a github repository with a single `registry.csv` file
* Apart from the header, each row in `registry.csv` represents one Data Package Profile. It has the following keys:
    * **`id`**: a locally unique identifier for the profile (eg: "`openspending`")
    * **`title`**: a human-readable name for the profile (eg: "`Open Spending Data Package`")
    * **`schema`**: a URL to a valid JSON schema, which validates whether Data Packages conform to this profile (eg: https://raw.githubusercontent.com/dataprotocols/schemas/master/data-package.json)
    * **`specification`**: a URL to the human-readable specification of the profile (eg: http://dataprotocols.org/tabular-data-package/)
* To begin with, it contains two profiles: "Data Package" and "Tabular Data Package".
* To add new profiles, create a pull request meeting the above requirements.
