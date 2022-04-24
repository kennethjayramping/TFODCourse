# Before doing anything else, click CTRL + SHIFT + P, then click Open Workspace Settings. Add in this code,

"terminal.integrated.profiles.windows": {
  "PowerShell": {
    "source": "PowerShell",
    "icon": "terminal-powershell",
    "args": ["-ExecutionPolicy", "Bypass"]
  }
},
"terminal.integrated.defaultProfile.windows": "PowerShell",


Initialize repo Step 1-4 on this link: https://github.com/nicknochnack/tfodcourse

Activate virtual environment everytime when working on project by running this command on terminal



# then click Save. Restart VS Code, close all terminals and start a new terminal by hitting the + sign.

# Run these in the terminal.
python -m pip install --upgrade pip
pip install ipykernel
python -m ipykernel install --user --name=tfodj

pip uninstall pyzmq
pip install pyzmq==19.0.2

# Install Visual C++ Build Tools on this link: https://visualstudio.microsoft.com/down 



PART 2 - Collect and label images
Ready your IDs to be slected and make sure the folder and the label for those images are set using the previous cells.
Run 4. Capture Images. Each pic takes about 2 seconds, and ae autosaved to the folder for collected images.

# Install labeling tools.
pip install pyqt5 lxml

Then run Part 5

Label images using the tool.

# After all labeling, create 'train' and 'test' folder inside images folder. Copy to train except one from all classes (image, label file). Put one set from each class to test.


**********************
For model evaluation:

 # PRECISION = True positive / (True positive + False positive)
 # RECALL = True positive / (True Positive + False negative)
**********************

*****
Available models for training: https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/tf2_detection_zoo.md
*****
     To be used: SSD MobileNet V2 FPNLite 320x320, link: http://download.tensorflow.org/models/object_detection/tf2/20200711/ssd_mobilenet_v2_fpnlite_320x320_coco17_tpu-8.tar.gz

     Can also use the 640x640, depends na sa imuha

  # Download NVIDIA CUDA, remove Nvidia Frameview SDK first then install Nvidia CUDA. Make sure Visual Sutdio 2017 is present beofre installing Nvidia CUDA. Then, install Nvidua CUDNN. Matching versions fr tensorflow-CUDA-cudnn here: https://www.tensorflow.org/install/source_windows


Follow instructios at 2:00:00-2:05:00

Then, add variables to system by searching in Start menu: EDIT ENVIRONMENT VARIABLES, then add new to System = New "PYTHONPATH", then contents (filepath of slim folder);(filepath of research folder)

Then train




