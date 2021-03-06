# speaker-recognition

# Team: Csapat1
# Members: Kis Ákos (AR4G0T), Vezse Botond (JWS3X8), Balogh Artúr Botond (BBBLAN)


# All three of us are writing our thesis now!!!

# VIDEO LINK: https://youtu.be/XKDs5Vnn8EI

## The database
We used the Voxceleb1 dataset, which contains over 100,000 utterances for 1,251 celebrities, extracted from videos uploaded to YouTube.

The following lines are from the Voxceleb trainer project, which contains the download method for the data too:
(https://github.com/clovaai/voxceleb_trainer)

We modified the codes by adding additional dependencies and made it to work on Windows.

### Dependencies
```
pip install -r requirements.txt
```
In addition to the Python dependencies, wget must be installed on the system.

### Downloading the database (Windows)

The required files and folder (lists, dataprep.py, requirements.txt) are in the root of the project
The following script can be used to download and prepare the VoxCeleb1 dataset for training.

```
python ./dataprep.py --save_path data --download --user USERNAME --password PASSWORD 
python ./dataprep.py --save_path data --extract
```
The USERNAME and PASSWORD need to be requested from this link: https://docs.google.com/forms/d/e/1FAIpQLSdQhpq2Be2CktaPhuadUMU7ZDJoQuRlFlzNO45xO-drWQ0AXA/viewform?fbzx=7440236747203254000

For the easy use of the provided data preparation, we suggest using the root of this project as a --save path

The downloading is not stable, so we recomment to download it manualy.

### Data preparation 

You can find the data processing in the Big_Homework.ipynb in the root directory of the project

### Training and Evaluation

We can find the code containing the training and evaluation of the model in Big_Homework.ipynb

### Testing and Optimization

We managed to expand the code with hyperoptimalization and added some visualization as well as some testing with different input parameters

The tmp folder contains the optimization log files (tensorboard) that should be placed to the root of the current drive
