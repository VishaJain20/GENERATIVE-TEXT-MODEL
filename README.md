# GENERATIVE-TEXT-MODEL

**Company**: CODTECH IT SOLUTIONS  
**Intern**: Visha Jain  
**Intern ID**: C0DF230  
**Domain**: AI/ML  
**Duration**: 4 weeks  
**Mentor**: Neela Santosh  
# 🧠 Generative Text Model using LSTM and Gradio

This project demonstrates a character-level text generator using an LSTM model built with PyTorch. A simple user interface is created using Gradio to allow interactive generation of text based on a starting string.

---

## 📌 Features

- Character-level text generation using LSTM.
- Trains on a small sample text.
- Generates up to 500 characters from a seed string.
- Simple and clean Gradio-based user interface.
- Modern design using custom CSS for enhanced UI.

---

## 🛠️ Requirements

- Python 3.x  
- PyTorch  
- NumPy  
- Gradio  

Install the dependencies using pip: `pip install torch numpy gradio`

---

## 🚀 How It Works

1. **Data Preparation**  
   A sample paragraph is used for training. Unique characters are extracted and mapped to integer indices for encoding and decoding.

2. **Sequence Generation**  
   Using a sliding window approach, overlapping character sequences are created for supervised learning.

3. **Model Architecture**  
   - Embedding layer to convert character indices into dense vectors  
   - LSTM layer to learn sequential dependencies  
   - Fully connected layer to predict the next character  

4. **Training**  
   Each input sequence is trained to predict the next character. CrossEntropyLoss is used along with the Adam optimizer.

5. **Text Generation**  
   - Accepts a starting string from the user.  
   - Encodes and feeds it into the LSTM model.  
   - Iteratively predicts and appends characters to generate 500 characters in total.  

6. **User Interface**  
   Built using Gradio Blocks with a modern, responsive layout. CSS is customized to enhance visual presentation and usability.

---

## 💡 Example Workflow

- Launch the app.  
- Enter a seed string like "Artificial".  
- Click the "Train Model" button to train the model on the provided text.  
- Click "Generate Text" to see a creatively extended output based on the seed.  
- Use the "Clear" button to reset the output fields.

---

## 🎨 UI/UX Design

The Gradio interface uses:

- A stylish header with gradient background  
- Input textbox for entering the seed  
- Output display with status box  
- Buttons for model training, text generation, and clearing  
- Custom CSS for:  
  - Rounded input/output boxes  
  - Shadows and hover effects  
  - Clean card-style components  

---

## 📂 File Structure

- `task4CODTech (1).py` – Main code file containing the model, training logic, and Gradio interface  
- `README.md` – This file

---

## ✅ Running the App

Run the Python script. A Gradio interface will launch in your browser automatically.  
Make sure all required Python libraries are installed.

