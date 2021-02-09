# Blue Brain Search and Graph Examples

## How to Use

To use the BBS_BBG_poc notebook, first make sure to have python version at least 3.6. Run the following commands to
set everything up:

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

Once everything is set up, you can run the notebook server.

```bash
jupyter-lab
```

The jupyter interface will open up in your default browser. Select and open the
BBS_BBG_poc notebook and follow the instructions there.

For more information about the Search and Graph components, please refer to the corresponding project pages:
- Blue Brain Search: https://github.com/BlueBrain/BlueBrainSearch
- Blue Brain Graph: https://github.com/BlueBrain/BlueBrainGraph
