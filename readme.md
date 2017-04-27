Torch Integrated Cell
===============================
Image-driven generative cell modelling with adversarial autoencoders

## Installation
Installing on linux is recommended.

### prerequisites
Running on docker is recommended, though not required.

- install torch on docker / nvidia-docker as in e.g. this guide: https://github.com/gregjohnso/dl-docker
- download the training images from s3://aics.integrated.cell.arxiv.paper.data

### Steps:
After you clone this repository, in `run_docker.sh` you will need to edit the mount points for the images to point to where you saved them.
Once those locations are properly set, you can start the docker image with

`bash run_docker.sh`

Once you're in the docker container, you can train the model with 

`bash train_model_2D.sh`

This will tkae a while, probably about 12-18 hours.

## Project website
Example outputs of this model can be viewed at http://www.allencell.org

## Citation
If you find this code useful in your research, please consider citing the following paper::

    @article{johnson2017generative,
       title={Generative Modeling with Conditional Autoencoders: Building an Integrated Cell},
       author={Gregory R. Johnson, Rory M. Donovan-Maiye, Mary M. Maleckar},
       journal={arXiv preprint arXiv:some.numeric.id},
       year={2017}
    }
    
## Contact
Gregory Johnson
E-mail: gregj@alleninstitute.org
