# 📖 Story-Voice Fine-Tuner

An AI-powered writing assistant that learns and mimics your unique storytelling style.

The **Story-Voice Fine-Tuner** allows writers to train a lightweight language model on their own writing, or any selected corpus, to generate new content that matches their tone, voice, and narrative style.  
Think of it as your personal co-author.

---

## 🚀 Features

- ✍️ Fine-tunes a **GPT-2 small** model on custom writing samples  
- 🧠 Learns tone, pacing, and stylistic patterns  
- 💬 Generates story continuations from short prompts  
- 🌐 Interactive UI using **Gradio + React frontend**  
- ⚡ Runs on **Google Colab (GPU-supported)**, so no powerful hardware is required  
- 🔁 Supports iterative improvement through evaluation metrics  

---

## 🧠 How It Works

### 1. Data Collection
Provide writing samples, such as `.txt` files containing stories or chapters.

### 2. Preprocessing
Text is cleaned and tokenized into a format the model understands.

### 3. Fine-Tuning
A pre-trained GPT-2 model is trained on your dataset to adapt to your writing style.

### 4. Generation
The model generates text based on user prompts through a web interface.

### 5. Evaluation
Output quality is measured using:

- **Perplexity** — model confidence  
- **Human evaluation** — style and coherence  

---

## 🏗️ Tech Stack

### Frontend
- React
- Gradio

### Backend / ML
- Python
- Hugging Face Transformers
- PyTorch
- Hugging Face Datasets

### Environment
- Google Colab (GPU-enabled)

---

## 📂 Project Structure

```text
├── data/
│   └── my_stories.txt
├── notebooks/
│   └── training.ipynb
├── model/
│   └── fine_tuned_gpt2/
├── app/
│   ├── gradio_app.py
│   └── react_frontend/
├── utils/
│   └── preprocessing.py
└── README.md



---

## ⚙️ Setup & Installation

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/story-voice-fine-tuner.git
cd story-voice-fine-tuner


### 2. Install Dependencies

pip install transformers datasets torch gradio

### 3. Prepare Your Dataset

Add your .txt file to the data/ folder.
Recommended minimum size: 50–100 KB
Example:
data/my_stories.txt

## 🧪 Training the Model
Run the training notebook in Google Colab.
Enable GPU
Go to:
Runtime → Change runtime type → GPU

### Key Steps
Load the dataset
Tokenize the text
Fine-tune GPT-2
Save the trained model

## 💬 Running the App
Start the Gradio Interface:
python app/gradio_app.py

Then open the provided local URL in your browser.

## 🎛️ Generation Controls
Temperature — higher = more creative
Top-K Sampling — improves coherence
Max Length — controls output size

## 📊 Evaluation
Perplexity
Measures how well the model predicts text (lower is better)
Human Ratings (1–5)
Style similarity
Coherence
Creativity

## 🔄 Future Improvements

Better dataset preprocessing
Larger models (e.g., GPT-Neo)
Fine-grained style controls
Full web app deployment
Multiple writing profiles

## ⚠️ Limitations

Requires sufficient training data
GPT-2 small has limited understanding
Outputs may be inconsistent or repetitive

## 📌 Use Cases

Overcoming writer’s block
Style imitation
Draft generation
Creative brainstorming

##📜 License
This project is open-source under the MIT License.

## 🤝 Acknowledgements

Hugging Face Transformers
OpenAI GPT-2
Google Colab
