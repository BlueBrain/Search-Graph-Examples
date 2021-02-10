# Blue Brain Search and Graph Examples

## How to Use

To use the BBS_BBG_poc notebook, first make sure to have python version at least 3.6. To be able to install Blue
Brain Search package correctly, it is also import to set up MySQL (see [link](https://pypi.org/project/mysqlclient)) for instructions to install it depending on your OS).

Run the following commands to set everything up:

```bash
python -m venv venv
source venv/bin/activate
pip install --upgrade pip wheel setuptools
pip install --requirement requirements.txt
```

Next follow the instructions on the [Blue Brain Search project page](https://github.com/BlueBrain/BlueBrainSearch#getting-started) to setup the servers. In particular, it is important that the
following environment variables are defined:

```bash
export DB_URL=<value>
export SEARCH_ENGINE_URL=<value>
export TEXT_MINING_URL=<value>
```

where `<value>` has to be replaced by the correct value.


Next, set the paths to the Nexus-forge configuration and the ontology linking data as the following environment variables:

```bash
export FORGE_CONFIG_FILE=<path_to_file>
export ONTOLOGY_LINKING_DATA_FILE=<path_to_file>
```

An example Nexus-forge configuration file is distributed with the repository (`config/forge-config.yml`), while an example of the ontology linking data can be found by the [link](https://github.com/BlueBrain/BlueBrainGraph/blob/master/cord19kg/examples/data/NCIT_ontology_linking_3000_papers.csv.zip) (linking data corresponds to the `csv` table obtained by decompressing the file provided by the link).


Once everything is set up, you can run the notebook server.

```bash
jupyter-lab
```

The jupyter interface will open up in your default browser. Select and open the
BBS_BBG_poc notebook and follow the instructions there.


For more information about the Search and Graph components, please refer to the corresponding project pages:
- Blue Brain Search: https://github.com/BlueBrain/BlueBrainSearch
- Blue Brain Graph: https://github.com/BlueBrain/BlueBrainGraph
