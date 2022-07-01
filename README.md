# Detection of ADHD based on Eye Movements during Natural Viewing

In this paper, we explore whether Attention-deficit/hyperactivity disorder (ADHD) can be detected based on recorded eye movements together with information about the video stimulus in a free-viewing task

## Setup

Install dependencies:

```
pip install -r requirements.txt
```

## Run Experiments

### Prepare saliency maps
Please download videos from ..., break it down into frames (e.g. use ffmpeg packages) and put them under the folder /Data/videos/frames_{video_name}/

We use a state-of-the-art saliency model, DeepGazeII to compute salinecy maps for our video stimuli. Download the files you need to run the DeepGazeII model (https://drive.google.com/file/d/1kYUwoatqQUS5EabeeSDc6gRmCysnVZ6N/view)，and stored under the folder /DNN_model/DataGeneration/

To generate the saliency maps for all videos, run
```
bash gen_saliency_map_data.sh
```

### Prepare model input files

To generate model input files, run

```
bash gen_model_input_data.sh
```

### Run models

```
bash run_models.sh
```


## Cite our work
.
