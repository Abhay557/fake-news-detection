# ML-Based-NewsDetection

*Fake News Detection and Classification using NLP & Machine Learning.*  
This project aims to detect and classify **fake news** using **Natural Language Processing (NLP)** and **Machine Learning** techniques.  
The trained model analyzes news articles and predicts whether they are **real or fake** based on their content.

🔗 **Live Demo:** [Click Here](https://ml-based-newsdetection.onrender.com)  
🔗 **Dataset:** [Click Here](https://www.kaggle.com/datasets/emineyetm/fake-news-detection-datasets)

![App Screenshot](/img1.png)
![App Screenshot](/img2.png)

---

## About This Project
I wanted to build a complete project from scratch to tackle a real-world problem, and fake news felt like a big one. My goal was to create a simple but smart app that could quickly classify an article. This project was a huge learning journey for me, from cleaning the initial dataset all the way to deploying a live application.

### A Note on the Model's Accuracy (My Biggest Learning Moment)
One of the most important things I learned was about the data itself. The model's 99.6% accuracy looks amazing, but this high score is actually a direct result of being trained on a relatively small and specific dataset (mostly US political news).
Because the data is so narrow, the model became an "expert" on that one topic but can still make mistakes on news about different subjects or from different parts of the world. It was a powerful lesson in how a model's performance is completely dependent on the quality and diversity of its training data.

## My Technical Approach
Here's a quick look at the core technical decisions I made while building this project:
**The Problem: I framed this as a classic binary classification task. The model just has to decide between two options: "real" or "fake."**
Making Sense of Words (NLP): The first big challenge was turning text into numbers a model can understand. I used a core NLP technique: TF-IDF (Term Frequency-Inverse Document Frequency). I chose this because it’s a smarter method than just counting words—it gives more weight to terms that are important and unique to an article, which is much better for finding predictive patterns.
Choosing the Right Algorithm: For the actual prediction model, I used a Passive Aggressive Classifier. After researching, I learned it's incredibly efficient and a top performer for NLP tasks like this, especially with the high-dimensional data that TF-IDF produces. It was the perfect fit.

### Skills 
This project pushed me to learn a ton. Here’s a quick rundown of everything involved:<br>
**Core Skills**: NLP | End-to-End ML Pipelines | Full-Stack Development | REST API Creation | Cloud Deployment <br>
**Tech Stack**: Python | Flask | Scikit-learn | Pandas | NLTK | HTML | Bootstrap | JavaScript | Gunicorn | Render


## Key Machine Learning Techniques

### **Text Vectorization: TF-IDF**
- Converts unstructured text into numerical format.
- Weights words higher if they are frequent in one article but rare across others.
- Provides strong predictive features for classification.

### **Classification Model: Passive Aggressive Classifier**
- Efficient **online learning** algorithm for text classification.
- Remains *passive* on correct predictions, *aggressive* on mistakes.
- Fast, scalable, and highly accurate (achieved **99.6% accuracy**).
- *one of the biggest backfall is that model is trined on small dataset.*

---

## Installation & Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/ML-Based-NewsDetection.git
   cd ML-Based-NewsDetection
   ```

2. **Create virtual environment & install dependencies**

   ```bash
   python -m venv venv
   source venv/bin/activate   # On Windows: venv\Scripts\activate
   pip install -r requirements.txt
   ```

3. **Run the Flask app**

   ```bash
   python app.py
   ```

4. Open your browser and go to:

   ```
   http://localhost:5000/
   ```

---

## License

This project is licensed under the **MIT License** – free to use, modify, and distribute.

---
