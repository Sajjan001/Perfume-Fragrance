# 🌸 AI Perfume Recommendation System

A modern, premium AI-powered web application that recommends the perfect fragrance based on environmental conditions and personal preferences.

## ✨ Features

- **AI-Powered Recommendations**: Uses a trained RandomForestClassifier to predict the perfect perfume for you
- **Modern UI**: Beautiful, responsive design with glassmorphism effects
- **Smart Inputs**: 
  - Environmental factors (Temperature, Humidity, Air Quality Index)
  - Personal preferences (Time of Day, Mood, Occasion, Preferred Type)
- **Real-time Predictions**: Instant fragrance recommendations with descriptions
- **Animated Interactions**: Smooth animations and loading states

## 🎨 Design Features

- Gradient background (purple → pink → blue)
- Glassmorphism cards with blur effects
- Smooth hover animations
- Mobile-responsive layout
- Premium SaaS-style interface

## 🚀 Installation

### Prerequisites
- Python 3.8+
- pip or conda

### Local Setup

1. Clone the repository:
```bash
git clone <your-repo-url>
cd Perfume
```

2. Create a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Run the app:
```bash
streamlit run app.py
```

The app will be available at `http://localhost:8501`

## 📊 Model Information

- **Model Type**: Random Forest Classifier (200 estimators)
- **Training Data**: 10,000+ fragrance samples
- **Features**: 7 input variables
- **Accuracy**: 24.60% (baseline model)

## 📁 Project Structure

```
Perfume/
├── app.py                 # Main Streamlit application
├── train_model.py         # Model training script
├── perfume_dataset.csv    # Training dataset
├── model.pkl              # Trained model
├── encoders.pkl           # Label encoders
├── requirements.txt       # Python dependencies
├── README.md              # This file
└── .streamlit/
    └── config.toml        # Streamlit configuration
```

## 🌐 Deployment

### Deploy on Streamlit Cloud (Recommended)

1. Push your project to GitHub
2. Go to [https://streamlit.io/cloud](https://streamlit.io/cloud)
3. Click "New app"
4. Connect your GitHub repository
5. Select the branch and main file (`app.py`)
6. Click "Deploy"

### Deploy on Other Platforms

- **Heroku**: See `Procfile` setup
- **AWS**: Use EC2 or Lambda
- **Google Cloud**: Use Cloud Run
- **Azure**: Use App Service

## 🔧 Technologies Used

- **Streamlit**: Web framework for ML apps
- **Scikit-Learn**: Machine learning model
- **Pandas**: Data processing
- **NumPy**: Numerical computations

## 📝 Customization

### Change Color Theme
Edit `.streamlit/config.toml` to modify colors:
```toml
[theme]
primaryColor = "#your-color"
backgroundColor = "#your-color"
```

### Modify Perfumes & Taglines
Edit `app.py` and update the dictionaries:
```python
perfume_icons = {...}
perfume_taglines = {...}
```

## 🤝 Contributing

Feel free to fork and submit pull requests for improvements!

## 📄 License

This project is open source and available under the MIT License.

## 💡 Future Enhancements

- [ ] Add user preferences history
- [ ] Implement user authentication
- [ ] Add more fragrance types
- [ ] Improve model accuracy with larger dataset
- [ ] Add perfume price information
- [ ] Integration with e-commerce platforms
- [ ] Mobile app version

## 📧 Support

For issues or questions, please open an issue on GitHub.

---

**Powered by AI** 🤖 | **Premium Fragrance Intelligence** ✨
