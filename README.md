# Doom-Dataset

## Tested on
```
Python > 3.6
Ubuntu - 18.0.1
PyTorch == 1.8.1+cu102 and 1.9.0+cu102
```

## Setup
```
sudo apt-get update
sudo apt install cmake libboost-all-dev libsdl2-dev libfreetype6-dev libgl1-mesa-dev libglu1-mesa-dev libpng-dev libjpeg-dev libbz2-dev libfluidsynth-dev libgme-dev libopenal-dev zlib1g-dev timidity tar nasm
pip install vizdoom
pip install opencv-python
```

## Training
```
python arnold.py --exp_name test --main_dump_path $PWD/dumped --scenario defend_the_center --frame_skip 2 --action_combinations "turn_lr+attack" --gpu_id -1 --replay_memory_size 1000000 --labels_mapping "0" 
```
