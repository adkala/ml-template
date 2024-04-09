# ml-template

Template repo for setting up ml experiments quickly. Uses pytorch.

Includes basic training loop and scripting for experiment setup using hydra. Configure experiments in `exp` folder. Set `train.py` params in `exp/train.yaml`.

Need to implement `utils.py:get_dataset` before use.

## Usage

To run an experiment, run `python train.py +exp=exp0` to run `exp0.yaml` (found in `exp/exp` folder).

To run from a checkpoint, run `python train.py +exp=exp0 +ckpt=*checkpoint_file*`.
