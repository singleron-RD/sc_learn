1. `submit.sh`
```
#!/usr/bin/env bash

#SBATCH --job-name=sample1           # job name
#SBATCH --partition=general           # partition
#SBATCH --ntasks=4            # CPU need
#SBATCH --mem=30G                     # Memory need
#SBATCH --output=%j.out               # stdout file
#SBATCH --error=%j.err                # stderr file

conda activate celescope
sh ./shell/test1.sh
```

2. 
```
sbatch submit.sh
```

3. 
```
squeue
```