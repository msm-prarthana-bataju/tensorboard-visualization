# Tensorboard-Data-Visualization

●　By Prarthana Bataju 2020.06.05

●　Steps to run the code

①　vgg16-feature-extraction.py
●　Used for extracting features from your images using VGG-16 model.

line 86 : change the path to your data folder link.
line 26 : def_image_model(): This function will automatically download the VGG-16 model.
line 105 and line 107 : change name of feature vector (*.txt and *.pkl [please give same name]

●　Then run the code
●　If run sucessfully, you will see the feature vector in the path where you have saved your data.


②　own-data-embedding-visualization.py
●　This py file create　checkpoints, spirite image and metadata used for tensorboard visualization.
●　Create folder name "embedding-logs” in the same path where you have put your data folder and feature vector.
●　Line 21: Change name of data folder.
●　Line 51:　Change name of feature vector　(*.txt file) created from vgg16-feature-extraction.py
●　Line 76: Change metadata name (if you like)
●　Line 125：　Change sprite png file name (if you like）
●　Line 132：　Change checkpoint name (if you like）
●　Line　139: Change metadata name same name of line 76
●　Line　141: Change spirte name same name of line 125

●　Then run the code.
●　If run sucessfully, you will get the above files in embedding-logs folder.

③　Tensorboard Visualization
●　Used embedding-logs data to visualize your data in tensorboard.
●　Initilaize tensorboard in commandprompt：
tensorboard --logdir="path to embedding logs"
●　This will host your port in 6006
●　Copy and paste the port link in your broswer and visualize the data in tensorboard visualization.
