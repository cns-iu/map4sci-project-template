# Template for projects using map4sci

## Prerequisites

1. Docker (and Docker Compose) installed and running
2. If running through CWL, cwl-runner must also be installed. You can install the reference runner in python with `python -m pip install cwl-runner cwltool`
3. datasets directory filled with datasets in the proper format (network.dot + config.sh)

## Running

Run the `run.sh` script which will loop through all datasets in the datasets directory and run map4sci over them. It skips datasets which have succesfully finished already.

## Results

Results will be in the `raw-data` directory and a fully built static website in the `site` directory.
