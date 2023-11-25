# What is Time-Travelling Visualization?

# How to Use it?

## Pull Our Code

//TODO for yifan and yiming, prepare a huggingface for a training process

The project structure looks as follow:
XXX fold is for XXX
XXX fold is for XXX
XXX fold is for XXX

Note that, the XXX folder and XXX folder stores the training process and the target dataset. 
We can download them as follows:

demo data store in /training_dynamic

## Training Process Dataset (the training process of a model)

//TODO for yifan and yiming, prepare a huggingface for a training process

you can download by https://huggingface.co/yvonne1123/trustvis_with_dataset
then you can store the dataset in /training_dynamic (default path)

## Target Dataset

//TODO for yifan and yiming, prepare a huggingface for a training process

# Environment Configuration

```
conda activate myvenv
cd Trustvis
python subject_model_eval.py
```
The trainig dynamic performance will be store in /training_dynamic/Model/subject_model_eval.json

# Train Your Time-Travelling Visualizer


# Run Your Time-Travelling Visualizer

## Run Tool

```
# backend
cd /Tool/backend/server
python server.py

# frontend
cd /Tool/frontend
we have the built version: down load url: https://drive.google.com/file/d/1MoGPYC6cO1Kxgsz3dVxf4cvRLfhqbz7X/view?usp=sharing 
unzip and use browser open /vz-projector/standalone.html

input content_path and backend ip
click login 
```

## Run TrustVis
```
cd Trustvis
conda activate myvenv
# proxy only
python porxy.py --epoch num --content_path "dataset path"(default: /training_dynamic)

the vis result will be store in /training_dynamic/Proxy/***.png
the evaluation resulte wiil be store in /training_dynamic/Model/proxy_eval.json

# trustvis with AL
python active_learning.py  --epoch num --content_path "dataset path"(default: /training_dynamic)

the vis result will be store in /training_dynamic/Trust_al/***.png

the evaluation resulte wiil be store in /training_dynamic/Model/trustvis_al_eval.json

```

