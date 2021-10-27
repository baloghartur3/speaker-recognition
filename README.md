# speaker-recognition

## Installing the database

The required files and folder (lists, dataprep.py, requirements.txt) are in the root of the project
### Dependencies
```
pip install -r requirements.txt
```

### Downloading the database

The following script can be used to download and prepare the VoxCeleb dataset for training.

```
python ./dataprep.py --save_path data --download --user USERNAME --password PASSWORD 
python ./dataprep.py --save_path data --extract
python ./dataprep.py --save_path data --convert
```
