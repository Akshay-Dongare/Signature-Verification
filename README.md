# Signature-Verification
# Steps to set up:
1. Clone the repo and `cd` into it
2. Downloading required models
   * Download [https://huggingface.co/Akshay-Dongare/kerasVggSigFeatures.h5](https://huggingface.co/Akshay-Dongare/kerasVggSigFeatures.h5) and place it in `SOURCE\vgg_finetuned_model`
   * Download [https://huggingface.co/Akshay-Dongare/bbox_regression_cnn.h5](https://huggingface.co/Akshay-Dongare/bbox_regression_cnn.h5) and place it in `SOURCE\vgg_finetuned_model`
   * Download [https://huggingface.co/Akshay-Dongare/yolov5-CustomDatasetFromTobacco800](https://huggingface.co/Akshay-Dongare/yolov5-CustomDatasetFromTobacco800) and place it in `SOURCE\yolo_files`
   * Download [https://huggingface.co/Akshay-Dongare/CycleGAN-Signature-Verification-Dataset](https://huggingface.co/Akshay-Dongare/CycleGAN-Signature-Verification-Dataset) and place it in `SOURCE/gan_files/checkpoints/gan_signdata_kaggle`
3. In `SOURCE/vgg_finetuned_model/vgg_verify.py`, go to line 50 and put your own model path as raw string https://github.com/Akshay-Dongare/Signature-Verification/blob/5f6d9a123374549d976b340909f0474bb6a6e5b6/SOURCE/vgg_finetuned_model/vgg_verify.py#L50
4. Create Conda Environment (env exported from Windows 11 system)
   ```
   conda env create -f ./environment.yml
   ```
5. Activate Conda Environment
   ```
   conda activate signature-verification
   ```
6. Run Streamlit App
   ```
   streamlit run ./ui.py
   ```
