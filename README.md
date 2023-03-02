# Aerial Object Detection

Contextualized YOLOv5 model to detect aerial objects, specifically balloons.

Here is our [presentation]{https://drive.google.com/file/d/1pMDMGtbxPL8r8ubyexeZ6U9gx2dKwEac/view?usp=share_link} at the Northrop Grumman Innovation Challenge at UMD.

## Usage: transfer_learning_balloon.ipynb
- Run cell 1 to clone YOLOv5 repository, switch into directory, and install all requirements
- Upload balloons-dataset.zip to root directory (same level as yolov5 directory)
- Add the line "test: ../test/images" to the balloons-data/data.yaml
- Run rest of cells
- Save best.pt to use as weights argument for inferencing in the inferencing_balloon notebook.

## Usage: inferencing_balloon.ipynb
- Run cell 1 to clone YOLOv5 repository and cell 2 to switch into directory and install all requirements
- Add the input images and videos to the yolov5 directory
- Add the best.pt file to the yolov5 directory
- Run rest of cells
- Classified images and videos are stored in yolov5/runs/detect/exp{#}/
