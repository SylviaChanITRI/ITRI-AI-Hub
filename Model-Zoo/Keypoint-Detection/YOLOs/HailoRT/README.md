# Deploy YOLOs on HailoRT (Preview)

HailoRT is an inference engine designed specifically for the Hailo expansion accelerator, providing developers with high-performance and low-power deep learning operations.

To illustrate the process of delegating a model from the ONNX format to a Hailo binary file (.hef), we will use Ultralytics' pre-built YOLOv8n-pose model as an example. The model is trained on the COCO-Pose dataset, which contains 1 class of people with 17 keypoints. Please follow the instructions provided in the previous table of contents to obtain the model on your workstation, then proceed with the steps outlined in this document to complete the conversion process. Finally, a simple Python example is used to verify the accuracy of the inference results.

### Prerequisites

* Exported **YOLOv8n-pose** model in ONNX format ([[Tutorial]](https://github.com/R300-AI/ITRI-AI-Hub/blob/main/Model-Zoo/Object-Detection/YOLOs/Delegate_Models_to_ONNX_and_TFLite.ipynb)).
* **Ubuntu 22.04 LTS x86_64 Workstation** which **Data-Compiler** has been installed.
* A **Evaluation Board (with Hailo-8 M.2 expansion)** board which **HailoRT** Library has been installed.
