# Chatbot using BERT  

## 📌 Project Overview  
This project is a chatbot model trained using BERT for intent classification. The chatbot is designed to understand user queries and provide relevant responses based on predefined intents.  

## 📂 Dataset Used  
The dataset consists of a JSON file containing:  
- **Intents** with tags  
- **Patterns** (user inputs)  
- **Responses** (bot replies)  
- **Context setting**  

It includes **255 intents** and is sourced from Kaggle.  

## 🔧 Data Preprocessing  
The dataset undergoes preprocessing steps such as:  
- Removing null values  
- Converting text to lowercase  
- Removing punctuation, numbers, and stopwords  
- Tokenizing and encoding text using BERT  

## 📊 Exploratory Data Analysis (EDA)  
- Visualized the most frequent words using a **word cloud**  
- Extracted unique labels (tags) from the dataset  

## 🏋️ Model Training  
- Dataset split into **train and test sets**  
- BERT model initialized along with a tokenizer  
- A **custom DataLoader** was implemented  
- Evaluation metrics like **accuracy** and **F1-score** were used  

### **Results**  
- **Training Accuracy:** 99%  
- **Testing Accuracy:** 78%  

## 💾 Model Saving & Deployment  
The trained BERT model is saved and loaded using **Hugging Face’s pipeline** for real-time predictions.  

## 🚀 How to Run  
1. Clone this repository:  
   ```sh
   git clone https://github.com/your-username/chatbot-bert.git
   cd chatbot-bert
   ```  
2. Install dependencies:  
   ```sh
   pip install -r requirements.txt
   ```  
3. Train the model:  
   ```sh
   python train.py
   ```  
4. Run the chatbot:  
   ```sh
   python chatbot.py
   ```  

## 📜 Dependencies  
- Python  
- Transformers (Hugging Face)  
- TensorFlow / PyTorch  
- Scikit-learn  
- Pandas  

