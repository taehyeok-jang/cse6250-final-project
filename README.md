# CSE 6250 BD4H - Final Project 

# Prerequisites

## Dependency 

- Pytorch >=0.4
- Python >=3.5

## Dataset 

- MIMIC-III

Download [MIMIC-III dataset](https://mimic.mit.edu/docs/gettingstarted/) and put DIAGNOSES_ICD.csv, PRESCRIPTIONS.csv, PROCEDURES_ICD.csv in ./data
 
- Drug-Drug Interactions

Download [Drug-Drug Interactions dataset](https://www.dropbox.com/s/8os4pd2zmp2jemd/drug-DDI.csv?dl=0) and put drug-DDI.csv in ./data/


## On-board the Project in Google Colab

To import the project in Google Colab, plz we recommend you to read below articles.

- [Different Ways to Connect Google Drive to a Google Colab Notebook! (Part 1)](https://towardsdatascience.com/different-ways-to-connect-google-drive-to-a-google-colab-notebook-pt-1-de03433d2f7a)
- [Different Ways to Connect Google Drive to a Google Colab Notebook! (Part 2)](https://towardsdatascience.com/different-ways-to-connect-google-drive-to-a-google-colab-notebook-part-2-b867786aed55)


# Run the Code

## Modify Project Path

In the code, there are certain specified paths that currently access to our dedicated Google Drive directory.

You are able to customize the project path in your own Google Drive directory.

``` 
<CSE6250_Team_G3_final_submission.ipynb>

drive.mount('/content/gdrive')

sys.path.append("/content/gdrive/.../GAMENet/colab_env/lib/python3.10/site-packages")

path = "/content/gdrive/.../GAMENet/code_"
os.chdir(path)
```

## End-to-End ML Pipeline

1. Open './CSE6250_Team_G3_final_submission.ipynb'
2. Runtime > Change runtime type > T4 GPU (or any available GPU)
3. Runtime > Run all

## Training

1. Open './CSE6250_Team_G3_final_submission.ipynb'
2. Runtime > Change runtime type > T4 GPU (or any available GPU)
3. Run the End-to-End ML Pipeline to warm-up
4. In the section **'Running the Model - Train'**, adjust 'epoch_' to the target epoch (by default, a single epoch)
5. Run the cell
6. Model checkpoints and a final model will be saved in './code_/saved...'


## Testing


1. Open './CSE6250_Team_G3_final_submission.ipynb'
2. Runtime > Change runtime type > T4 GPU (or any available GPU)
3. Run the End-to-End ML Pipeline to warm-up
4. In the section **'Running the Model - Test'**, modify 'resume_path' to the target model (by default, a pre-trained model will be loaded)
5. Run the cell
6. Evaluation will be printed out




