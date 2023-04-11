# Object_detection_by_torchvision_faster_RCNN_Resnet50
This code demonstrates how to perform object detection on an image using the Faster R-CNN model with ResNet-50 backbone.

## Dependencies
This code requires the following libraries:

torch
torchvision
PIL
matplotlib


## Usage
Upload an image using the files.upload() method.
Load the model using the load_model() function.
Detect objects in the image using the detect_objects() function.
Display the original image and the image with predicted bounding boxes using the display_image_with_predictions() function.


## Functions
### load_model()
This function loads the Faster R-CNN model with ResNet-50 backbone that has been pre-trained on the COCO dataset. The function sets the model to evaluation mode and, if a GPU is available, moves the model to the GPU.

### detect_objects(image_path, model, threshold=0.5)
This function takes an image file path, a pre-trained model, and an optional threshold parameter as inputs. The function performs object detection on the image using the provided model and returns a list of dictionaries, where each dictionary represents a detected object and contains the bounding box coordinates, label ID, and detection score.

### display_image_with_predictions(image_path, detections, class_names)
This function takes an image file path, a list of detected objects, and a list of class names as inputs. The function displays the original image and the image with predicted bounding boxes for each detected object, along with the class name and detection score.

## Example
An example of how to use this code can be found at the end of the script. After uploading an image, the script loads the model, detects objects in the image, and displays the image with predicted bounding boxes for each detected object.
