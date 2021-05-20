# gnn-exp

To run experiments, first set up virtualenv. After activating the virtul environment, run 
```
pip3 install -r requirements.txt
```

## System and software config
The experiments are run locally on Ubuntu 20.04, with NVCC 10.2 and Python 3.8.5. The Python module versions can be found in `requirements.txt`.

## Positional and structural node classification
### RUN
```
cd graphsage-simple
bash train_nodes.sh
```
You can specify the initialization method, dataset, epoch, feature dimension and learning rate in `train_nodes.sh`.
The results can be found in `results` folder.

## Graph classification
Refer to `gnn_comparison/experiment.sh` for example runbook. 

## Deepwalk
Deepwalk is one of the initialization methods that we explore in this project. To generate deepwalk features, refer to https://github.com/phanein/deepwalk.

Make sure to include dataset directory in the `--input` and `--ouput` flag value, and set the `--format`. 
