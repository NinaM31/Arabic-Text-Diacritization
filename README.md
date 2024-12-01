# Arabic Text Diacritization
Submission of my final project for Artificial Intelligence CSC562. The aim of the project is to explore a research topic within the field of Artificial Intelligence.
My topic is Arabic text diacritization, this project experiments with word sense features, and part of speech, trained on a small sample ~10K.

# How To Run
- [X] [Install tensorflow<2.11 for GPU usage](https://www.tensorflow.org/install/pip#windows-native_1) 
- [X] Install Jupyter Notebook
- [X] Install numpy==1.23.1
``` 
pip install virtualenv
```
```
virtualenv -p python3.10 env
```
```
env\Scripts\activate
```
```
pip install -r requirements.txt
```


# Results
The models were trained for 10 epochs using RTX 3060, Adam optimization algorithm with 0.001 learning rate, only the first model had 256 batch size the rest were trained on 64 batch size to avoid out of memory error. Table 7 summarizes the configurations. All the models were trained on 10K lines of text.
### The training accuracy of the models 
![Untitled](https://github.com/user-attachments/assets/b7ab482e-fb63-47f6-97d8-1961ee627693)


### Diacritic Error Rate (DER) & Word Error Rate (WER)

![image](https://github.com/user-attachments/assets/5374d01e-c112-4db9-a3f6-4dea6fc3a3a1)

### Sample Results
![image](https://github.com/user-attachments/assets/35909d08-ab8c-4e7d-a25b-a8a27a460fc7)

# Credits
## Dataset
- [X] [20 % of Cleaned Data by Ali Fadel et all](https://github.com/AliOsm/arabic-text-diacritization/tree/master/dataset)
- [X] [Used Gemini API to add word sense](https://github.com/NinaM31/Arabic-Text-Diacritization/tree/master/Dataset)

## Code
- [X] [DER & WER Calculations](https://github.com/AliOsm/arabic-text-diacritization/blob/master/helpers/diacritization_stat.py)
  
## API's
- [X] [Gemini-Flash-1.5 api](https://ai.google.dev/pricing#1_5flash)
      
## Software & Hardware
- [X] RTX 3060
- [X] TensorFlow
- [X] Gensim

# Sample Demo

### BiLSTM-WSD



### BiLSTM-POS

https://github.com/user-attachments/assets/3dd3174a-0670-4c74-a92f-79d9e60cc324

### BiLSTM-W2V

https://github.com/user-attachments/assets/2b8194dd-25a3-444b-9f32-226e6a2c2c2b




