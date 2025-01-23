# 🌿🐦 Bird Atlas 🐦🌿

### AI-Powered Bird Species Identification

Welcome to **Bird Atlas**! This project is a deep dive into the fascinating world of birds. By harnessing the power of deep learning, this tool can identify over **500 bird species** with astonishing **97+% accuracy**! Whether you're an avid birdwatcher, a curious nature enthusiast, or someone looking to explore the diversity of our feathered friends, this project is for you. 🌿🐦

## 🌟 Features
- **Deep Learning Powerhouse**: Built using the EfficientNetB4 architecture, fine-tuned specifically for bird identification.
- **Accuracy You Can Trust**: With an accuracy of **97.83%**, you can rely on this tool to correctly classify birds.
- **Interactive Web App**: Upload a photo of a bird and get instant predictions, along with additional information about the species.
- **Educational Tool**: Learn about birds with Wikipedia links and detailed descriptions presented directly in the app.

## 🧠 How It Works

### 1. Data Augmentation 🖼️
Birds come in all shapes, colors, and poses. To ensure the model can handle this diversity, data augmentation techniques like random flipping, shifting, zooming, rotation, and contrast adjustment were applied. This makes the model robust to variations in:
- Lighting conditions
- Bird poses
- Background environments

### 2. Transfer Learning with EfficientNet 🚀
The backbone of this project is the **EfficientNetB4** model, a state-of-the-art neural network pre-trained on the large-scale ImageNet dataset. By leveraging its pre-learned knowledge, we:
- Extracted features relevant to bird classification.
- Added custom layers to tailor it specifically to bird species.

### 3. Fine-Tuning for Perfection 🎯
After training the custom layers, we fine-tuned the last 10 layers of the EfficientNetB4 model for an additional 5 epochs. This step refined the model's understanding of bird-specific features, ensuring unmatched classification performance.

## 📊 Model Performance
This bird classifier was rigorously tested on unseen data and achieved:
- **Accuracy**: 97.83%
- **Precision**: 98.19%
- **Recall**: 97.82%
- **F1 Score**: 97.79%

The results speak for themselves: this model is a powerhouse for bird classification! 🐦✨

## 🖥️ Streamlit Web Application
To bring this tool to life, I developed an interactive and user-friendly web app using **Streamlit**. Here’s what you can do:

1. **Upload Bird Photos**: Simply drag and drop an image, and the model will classify the bird species for you.
2. **Probability Bar Plot**: View the top 3 predicted species, along with their probabilities.
3. **Learn About Birds**: Each species name is linked to its Wikipedia page, so you can dive deeper into the bird’s characteristics and habitat.
4. **Visual Confirmation**: The app displays a sample image of the identified bird species from the test dataset.

## 🚀 Getting Started

### Prerequisites
- Python 3.8+
- Libraries: TensorFlow, Streamlit, NumPy, Pandas, and more (see `requirements.txt` for full details).

### Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/bird-atlas.git
   ```
2. Navigate to the project directory:
   ```bash
   cd bird-atlas
   ```
3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Launch the Streamlit app:
   ```bash
   streamlit run app.py
   ```

## 🐤 Why Birds?
Birds are some of the most captivating creatures on Earth. From their vibrant feathers to their melodic calls, they inspire awe and curiosity. With over 10,000 species worldwide, every bird is a story waiting to be told. This project is a tribute to their beauty and diversity—and a step toward making bird identification accessible to everyone. 🌍💚

## 🤝 Contributions
Contributions are welcome! Whether it’s improving the model, enhancing the web app, or expanding the dataset, your help will make this project soar higher. 🦅

## 📜 License
This project is licensed under the MIT License. Feel free to use, modify, and distribute it as you see fit.

## 🌈 Acknowledgments
- **EfficientNet**: For providing the backbone architecture.
- **Streamlit**: For making the web app development a breeze.
- **Wikipedia API**: For enriching the app with bird information.

Let’s make the world of birds a little more accessible, one species at a time. Happy birding! 🐦❤️

