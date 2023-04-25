# Template for projects using map4sci

## Prerequisites

1. Docker (and Docker Compose) installed and running
2. If running through CWL, cwl-runner must also be installed. You can install the reference runner in python with `python -m pip install cwl-runner cwltool`

## Crating Datasets

To create a dataset, follow these steps:

1. Create a folder with the name of the dataset inside `datasets`.
2. Inside the folder, create a `config.sh` file and a `network.dot` file.
3. for configuring the dataset refer [configuring the dataset](https://github.com/cns-iu/map4sci/tree/code-cleanup-documentation#configuring-the-dataset).

`Note that you can create multiple datasets to be processed.`

## Running

1. `quick run`: Run the `run.sh` script which will loop through all datasets in the datasets directory and run map4sci over them. It skips datasets which have succesfully finished already.
2. `Running through CWL`: refer [Running using cwltool/cwl-runner](https://github.com/cns-iu/map4sci/tree/code-cleanup-documentation#running-using-cwltoolcwl-runner).
3. `Running through Docker`: refer [Running using Docker](https://github.com/cns-iu/map4sci/tree/code-cleanup-documentation#running-using-docker).
4. `Running through Docker Compose`:refer [Running using Docker Compose](https://github.com/cns-iu/map4sci/tree/code-cleanup-documentation#running-using-docker-compose)

## Results

Results will be in the `raw-data` directory and a fully built static website in the `site` directory.
