** Tools **
Google colaboratory - https://colab.research.google.com/


** Folder Structure **

code
|--templates
|	|--index.html
|--commonsense_data.csv
|--commonsense_single_sent.csv
|--create_data_for_commonsense.ipynb
|--Flask.ipynb
|--Single_sentence_classification.ipynb
|--Two_sentence_classification.ipynb


** Files and Folders **

templates 				- containes index.html which contains the code for the frontend UI
commonsense_data.csv 			- CSV file containing the dataset for two sentences
commonsense_single_sent.csv 		- CSV file containing the dataset for a single sentence
create_data_for_commonsense.ipynb 	- Colab Notebook to create single sent and two sent data from the original semeval dataset
Flask.ipynb  				- Colab Notebook that runs as a server for the frontend.
Single_sentence_classification.ipynb  	- Colab Notebook to train models for single sentence
Two_sentence_classification.ipynb  	- Colab Notebook to train models for two sentences

-Link to online files and folders-
https://drive.google.com/drive/folders/18tH0-8KEuNXwplw9ST8PCdjbRrVSxGxy?usp=sharing

Single_Models				- Models trained on single sentences
Two_Sentence_Models			- Models trained on two sentences
S-Bert					- Code and trained models for S-Bert
K-Bert					- Code and files related to K-Bert
data					- Contains orignal dataset files


** How to create dataset? **

1. Open https://colab.research.google.com/
2. Go to File > Click Upload notebook > Select Upload > Click Choose File > Select the file "create_data_for_commonsense.ipynb"
3. Set the appropriate paths for all the csv files in the cell within the above ipynb file. The dataset files are present in the data folder shared in the above link.
4. Set the path for output folder as well.
5. Press "Ctrl+F9" or go to Runtime > Run All


** How to train models? **

1. Open https://colab.research.google.com/
2. Go to File > Click Upload notebook > Select Upload > Click Choose File > Select the file "Single_sentence_classification.ipynb" or "Two_sentence_classification.ipynb"
3. Set the appropriate paths for two_sentences_dataset_path or single_sentences_dataset_path depending on the task. Also set the saved_model_output_directory.
4. Select the pretrained_model you want to use and set the epochs
5. Press "Ctrl+F9" or go to Runtime > Run All


** How to run the demo? **

1. Open https://colab.research.google.com/
2. Go to File > Click Upload notebook > Select Upload > Click Choose File > Select the file "Flask.ipynb"
3. Set the appropriate paths for all the models. Use Single_Models and Two_Sentence_Models from the drive link to access the trained models.
4. Press "Ctrl+F9" or go to Runtime > Run All
5. ngrok url will be created when the last cell starts to run.
6. Upload the templates folder in the colab using the Files option on the left pane.
7. Change the form action url in the index.html to the above ngrok url. Save the html file.
8. Open the ngrok url in a browser. Follow the instructions on the screen to run the demo.


