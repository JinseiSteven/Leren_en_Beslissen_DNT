# Leren en Beslissen DNT

[TODO:description]

# Installation

```
$ git clone https://github.com/JinseiSteven/Leren_en_Beslissen_DNT.git
$ cd Leren_en_Beslissen_DNT

# Run this if you want to create a virtual env for the dependencies
$ python3 -m venv env
$ source ./env/bin/activate

$ pip3 install -r requirements.txt
```

# Datasets

To train the model with the dataset, please request the dataset from one of the
authors mentioned at the [Authors](#authors) section.

All datasets should be put inside `./datasets/<DATASET_FOLDER_NAME>`

# Usage

### `train.py`

This file can be used to train the neural network with [YOLOv8](https://github.com/ultralytics/ultralytics).

Make sure to download one of the `YOLOv8x` models specified at the GitHub page
and place it inside the root of this repository.

Example run:

```
$ ./train.py --yolo-config=./yolov8n.yaml --train-config=./config/train_spl.yaml --epochs=3
```

**NOTE:** Apple Silicon users can specify `--device=mps`, see [Apple M1 and M2 MPS Training](https://docs.ultralytics.com/modes/train/#apple-m1-and-m2-mps-training)

See `./train.py --help` for all possible arguments.

# Authors

- Joost Weerheim (13769758)
- Kim Koomen (14621312)
- Ross Geurts (14599996)
- Stephan Visser (13977571)
