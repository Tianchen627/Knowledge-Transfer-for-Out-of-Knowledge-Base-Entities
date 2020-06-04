# Knowledge Transfer for Out-of-Knowledge-Base Entities
## Requirements
- `python3.6` or higher.
- `chainer 6.5.0` 

## Train the model
- Type `python3 train.py ` on terminal.
- Information about args of train.py.More details can be found in the code.
    - `--seed 0`: Set the seed of random generator. The accuracies changes by few percent depending on `seed`.
    - `--bS 5000`: Set the batch size by 5000.
    - `--Op Adam`: Using Adam optimization algorithm in training.
    - `--D 81`: Set the embedding size for entities as 81.
    - `--rF both-1000-dim81-kernel0.txt`: The training process will be recorded in file `both-1000-dim81-kernel0.txt`.
    - `-iBeT`: Using bernoulli trick during negative sampling. 
## Modify the model
- Modify the code in `model.py`.