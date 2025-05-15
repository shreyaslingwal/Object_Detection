# Object_Detection using YOLOV8
This project implements a real-time object detection system using the YOLOv8 model from the Ultralytics library. It captures video frames from a webcam, processes each frame through the YOLOv8 model to detect objects, and then displays the video feed with bounding boxes and labels indicating the detected objects along with their confidence scores. The project uses the OpenCV library for video capture and display, and cvzone to enhance the visual presentation of the bounding boxes with corner rectangles and text labels.

The YOLOv8 model used is pre-trained on the COCO dataset, which includes 80 common object classes such as person, car, dog, laptop, and many others. An additional class, "earbuds," has also been included, which can be used for custom detection purposes if the model is trained accordingly.

Different versions of YOLOv8 model weights are available to suit various needs and hardware capabilities. These include nano (yolov8n), small (yolov8s), medium (yolov8m), large (yolov8l), and extra-large (yolov8x). The nano version is optimized for speed and low resource consumption, suitable for edge devices, while the large and extra-large models provide higher accuracy at the cost of increased computational requirements. Users can select the desired model by changing the weight file loaded in the code.

The system continuously reads frames from the webcam, detects objects in each frame, and overlays bounding boxes with labels and confidence percentages in real time. The program runs until the user exits, providing a smooth and interactive experience for object detection.

This implementation demonstrates how deep learning models like YOLOv8 can be integrated with computer vision tools to create practical, real-time applications. It is flexible and can be extended to other input sources, customized for different object classes, or adapted for deployment on different hardware platforms.

| Model        | Size    | Speed ⏩   | Accuracy 🎯 | Use Case                           |
| ------------ | ------- | --------- | ----------- | ---------------------------------- |
| `yolov8n.pt` | Nano    | Very Fast | Lower       | Edge devices, Raspberry Pi         |
| `yolov8s.pt` | Small   | Fast      | Moderate    | Real-time detection on CPUs        |
| `yolov8m.pt` | Medium  | Balanced  | Good        | General-purpose                    |
| `yolov8l.pt` | Large   | Slower    | High        | Accuracy-focused CPU applications  |
| `yolov8x.pt` | X-Large | Slowest   | Highest     | Powerful GPUs, high-accuracy needs |
