# LLM Web Application - Make Friends with English

## Project Description
This project is to develop a web application tailored to English learners from Japanese or Mandarin-speaking backgrounds. The app is able to identify errors in sentences written by learners and suggest accurate corrections, ultimately enhancing their learning experience and improving their language proficiency. The **Methods & Techniques** section below illustrates the implementation details for an end-to-end NLP pipeline. 

## 🤝 Team Members
Our team is named A Very Beta ChatGPT 4.5 and made up of the following members:
- Stefan Hall
- Tim Wang
- Amy Yang

## 🛠 Methods & Techniques
![Flow Chart](https://github.com/amy-panda/LLM_Web_App/blob/main/Images/flow_chart.jpg)


## 🖥 Deployment
To run the application locally, navigate to the 'Model Deployment' folder and execute the code below in your terminal:
- `pip install -r requirements.txt`
- `streamlit run app.py`

To enable the public access, the web application was deployed on Hugging Face Space. Find web app [**here**](https://huggingface.co/spaces/amyyang/webapp_englishtool). You can also find the [fine-tuned models](https://huggingface.co/amyyang) on Hugging Face.

### The web application layout

![Layout](https://github.com/amy-panda/LLM_Web_App/blob/main/Images/web%20app%20layout.jpg)

You can make selection for your native language and the language model to be used. 
- Your native language Japanese or Madarin. (For this project, only two foreign language backgrounds are considered.)
- Language model to use BART or GPT-2. 

Once the options above are selected, you can enter the sentence and click 'Generate' button to get the recommended/corrected sentence as well as the POS tagging and Dependency Tree to visualise the relationships between words in a sentence. &nbsp;  &nbsp;  

![Sentence](https://github.com/amy-panda/LLM_Web_App/blob/main/Images/correct%20sentence.png)

## ℹ️ Data Source
The dataset used in this project is from [NAIST Lang-8 Learner Corpora](https://sites.google.com/site/naistlang8corpora/home?authuser=0). The python file `extract_err-cor-pair_new.py` in the repository is used for data extraction into csv files. It is a modified version of [this](https://github.com/tomo-wb/Lang8-NAIST-extractor/blob/master/scripts/extract_err-cor-pair.py) original file. 


## 📚 References
- [BART Model](https://huggingface.co/docs/transformers/main/en/model_doc/bart)
- [CaliberAI/streamlit-nlg-gpt-2](https://github.com/CaliberAI/streamlit-nlg-gpt-2)
- [Video: Deploy Fine Tuned BERT or Transformers model on Streamlit Cloud](https://www.youtube.com/watch?v=mvIp9TvPMh0&t=348s)
- [OpenAI GPT2](https://huggingface.co/docs/transformers/main/en/model_doc/gpt2#overview)
- Gupta, S. (2020, December 10). Parts-of-Speech tagging app using Streamlit, spacy and Python. Srishti Gupta's Blog. https://srishti.hashnode.dev/parts-of-speech-tagging-app-using-streamlit-spacy-and-python 
- [Lang8-NAIST-extractor](https://github.com/tomo-wb/Lang8-NAIST-extractor/tree/master)
