# promptTo3D : Neural 3D Scene Generation with stable-dreamfusion

The promptTo3D repository is a collection of code that demonstrates the generation of 3D scenes using neural rendering techniques, specifically leveraging the stable-dreamfusion library. This repository provides a framework for training and testing a neural rendering model called NeRF (Neural Radiance Fields) using prompts.

NeRF is a deep learning-based approach that represents 3D scenes using volumetric function approximations. By learning the underlying scene geometry and appearance from a set of input images, NeRF can generate novel views of the scene from arbitrary camera viewpoints. The promptTo3D repository extends the capabilities of NeRF by incorporating textual prompts, allowing users to specify high-level instructions or descriptions for generating 3D scenes.

## Prerequisites

- NVIDIA GPU with CUDA support
- Python 3.10 and ^

## Installation

1. Clone the repository:

```shell
git clone https://github.com/ashawkey/stable-dreamfusion.git
```

2. Change into the cloned directory:

```shell
cd stable-dreamfusion
```

3. Install the required dependencies:
```shell
pip install -r requirements.txt
pip install git+https://github.com/NVlabs/nvdiffrast/
```

4. Install the CUDA extensions (this may take a few minutes):

```shell
pip install ./raymarching
pip install ./shencoder
pip install ./freqencoder
pip install ./gridencoder
```


## Usage

The code provides functionality for both training and testing the NeRF model. Follow the instructions below to train and test the model.

### Training

Open the Jupyter Notebook file promptTo3D.ipynb.

Modify the training settings as desired:

- Set the `Prompt_text` variable to specify the prompt text for training.
- Adjust other training settings such as the number of training iterations, learning rate, resolution, etc.

Execute the training process.

### Testing

Open the Jupyter Notebook file promptTo3D.ipynb.

Modify the testing settings as desired:

- Set the `Workspace_test` variable to specify the workspace for testing.

Execute the testing process.

### Displaying Results

After the training and testing processes are completed, the generated RGB video can be viewed. Follow the instructions below:

- Locate the RGB video file in the results directory of the workspace.
- Open the video file to view the generated RGB video.

## Screenshots

* Prompt and controls manipulation settings.

![settingsWindow](https://github.com/viv3k19/promptTo3D-using-Python-stable-dreamfusion/assets/82309435/a78b2b96-90f0-4fa5-9ee2-f835e8014e66)

* Training and testing Epoch Snippet.

![epochWindow](https://github.com/viv3k19/promptTo3D-using-Python-stable-dreamfusion/assets/82309435/956d4a85-582f-47f8-9bfd-9bcd94cd5409)

* Generated output as video file.

![result](https://github.com/viv3k19/promptTo3D-using-Python-stable-dreamfusion/assets/82309435/34234ba4-baf4-4ae2-9fe7-c652f25e312c)

## License

This project is licensed under the MIT License.

# Project Creator
* Vivek Malam - Feel free to contact me at viv3k.19@gmail.com for any questions or feedback.

