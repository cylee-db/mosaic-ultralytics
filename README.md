# mosaic-ultralytics
Examples to run the Ultralytics library on Mosaic

The end-to-end example downloads images stored on ADLS and stores them to a location used by Ultralytics to train the YOLOv11 model on Mosaic AI Training.

There are two config files to take note of:

- `mcli/yolo11_coco8_az.yaml`: Downloads image files from an URL you provide and run training on a designated GPU cluster on Mosaic.
- `ultralytics/cfg/datasets/coco8az.yaml`: Override of the data config file used by Ultralytics. Specifies the location of the downloaded images, where Ultralytics should read from.
