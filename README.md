# Signature-Verification
# Steps to set up:
1. Clone the repo and `cd` into it
2. Downloading required models
   * Download  and place it in `SOURCE\vgg_finetuned_model`
   * Download [https://huggingface.co/Akshay-Dongare/kerasVggSigFeatures.h5](https://huggingface.co/Akshay-Dongare/kerasVggSigFeatures.h5) and place it in `SOURCE\vgg_finetuned_model`
   * Download [https://huggingface.co/Akshay-Dongare/bbox_regression_cnn.h5](https://huggingface.co/Akshay-Dongare/CycleGAN-Signature-Verification-Dataset) and place it in `SOURCE\vgg_finetuned_model`
   * Download [https://huggingface.co/Akshay-Dongare/yolov5-CustomDatasetFromTobacco800](https://huggingface.co/Akshay-Dongare/yolov5-CustomDatasetFromTobacco800) and place it in `SOURCE\yolo_files`
   * Download [https://huggingface.co/Akshay-Dongare/CycleGAN-Signature-Verification-Dataset](https://huggingface.co/Akshay-Dongare/CycleGAN-Signature-Verification-Dataset) and place it in `SOURCE\gan_files`
3. Create Conda Environment
   * Open Terminal
   * Type
     ```
     conda env create -f ./environment.yml
     ```
4. Activate Conda Environment
   ```
   conda activate sing
   ```
5. Run Streamlit App
   ```
   streamlit run ./ui.py
   ```
