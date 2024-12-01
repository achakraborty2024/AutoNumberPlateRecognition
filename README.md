# AutoNumberPlateRecognition

This notebook demonstrates a number plate recognition system using various techniques. It begins by loading a pre-trained object detection model and provides a basic web interface for image upload and bounding box prediction. Subsequently, it explores the use of YOLOv10 for real-time object detection, fine-tunes the model on a custom dataset, evaluates its performance, and integrates it with OCR for text extraction from detected number plates. The notebook also includes functionalities for creating a Gradio interface for user interaction, processing video frames to detect moving vehicle number plates, and deploying the final model to Hugging Face. Key components include model loading, prediction, OCR integration, model training and validation, and model deployment.

1. YOLO-based detection:
   - Uses YOLOv8 to detect license plates in images and videos.
   - Employs the supervision library for visualization of detections.
   - Uses pytesseract for OCR to extract plate numbers.
   - Monitoring the metrics using Tensorboard
   - Includes functionalities for:
       - Single image prediction.
       - Prediction on a set of test images.
       - Real-time detection with a video stream.
       - A Gradio interface for interactive prediction.
       - Detection of license plates in traffic signals

2. UNet-based segmentation:
   - Uses a UNet model to perform image segmentation for license plate localization.
   - Preprocesses images, generates a binary mask representing plate regions.
   - Demonstrates training and inference of the UNet model.

3. Comparison of YOLO and UNet:
   - Presents a summary table highlighting the differences between the two architectures in terms of:
       - task, output, architecture, speed, accuracy, and applications.

Key improvements and additions in the code include:
   - Enhanced visualization using the `supervision` library
   - A Gradio interface for easy interaction
   - Handling of multiple image formats for prediction.
   - Improved error handling and robustness

Overall the code provides a comprehensive solution for number plate recognition, comparing two distinct deep learning approaches.
