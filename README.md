# AI Movie Recommender

An intelligent movie recommendation system that combines SerpAPI's movie data with Groq's AI analysis to provide personalized movie suggestions.

![AI Movie Recommender](banner.png)

## 🎯 Features

- **Smart Category Selection**: Choose from various movie categories including Indian Cinema, Action & Adventure, Comedy, Drama, and Romance
- **Advanced Preference System**:
  - Multi-select genre preferences
  - Mood-based filtering
  - Content rating selection
  - Story element preferences
  - Duration preferences
- **AI-Powered Analysis**: Uses Groq AI to analyze movie themes, patterns, and provide personalized recommendations
- **Rich Movie Information**: 
  - Movie thumbnails
  - Ratings
  - Pricing
  - Detailed plot descriptions
- **Save Functionality**: Store your favorite recommendations for later reference

## 🚀 Getting Started

### Prerequisites

- Python 3.8 or higher
- API Keys:
  - SerpAPI Key (Get it from [SerpAPI](https://serpapi.com))
  - Groq API Key (Get it from [Groq](https://console.groq.com))

### Installation

1. Clone the repository:
```bash
git clone https://github.com/We4TechAI/AI-Movie-Recommender.git
cd AI-Movie-Recommender
```

2. Install required packages:
```bash
pip install -r requirements.txt
```

3. Create a `.env` file in the project root:
```plaintext
GROQ=your_groq_api_key
SERPAPI_KEY=your_serpapi_key
```

### Running with Docker

For Docker deployment:

1. Build the Docker image:
```bash
docker build --tag ai_movie_recommender:latest .
```

2. Run the container:
```bash
docker run -d --name ai_movie_recommender -p 8501:8501 ai_movie_recommender:latest
```

3. Access the application at `http://localhost:8501`

### Running Locally

To run the application locally:
```bash
streamlit run app.py
```

## 🎮 Usage

1. **Select Movie Category**:
   - Choose your preferred movie category from the dropdown menu

2. **Set Your Preferences**:
   - Navigate to the sidebar
   - Select preferred genres
   - Adjust mood preference slider
   - Choose content ratings
   - Select desired story elements
   - Pick preferred movie duration

3. **Get Recommendations**:
   - Click "Get Recommendations" button
   - Wait for movie analysis
   - Review personalized suggestions

4. **Save Recommendations**:
   - Click "Save Recommendations" to store analysis
   - Access saved recommendations in the sidebar

## 🛠️ Technical Details

### API Integration

- **SerpAPI**: Fetches movie data from Google Play Movies
- **Groq**: Provides AI-powered analysis and recommendations

### Key Components

- `get_movie_recommendations()`: Fetches movie data from SerpAPI
- `get_enhanced_recommendations()`: Processes movies through Groq AI
- `main()`: Handles UI and core application logic

## 📊 Project Structure

```
AI-Movie-Recommender/
├── main.py                 # Main application file
├── requirements.txt       # Python dependencies
├── .env                  # Environment variables
├── Dockerfile           # Docker configuration
├── banner.png            
└── README.md            # Project documentation

```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/your-feature`
3. Commit changes: `git commit -am 'Add new feature'`
4. Push to branch: `git push origin feature/your-feature`
5. Submit a Pull Request

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments

- [SerpAPI](https://serpapi.com) for movie data access
- [Groq](https://groq.com) for AI analysis capabilities
- [Streamlit](https://streamlit.io) for the web interface

## ⚠️ Important Notes

- Ensure API keys are kept secure and not committed to version control
- API usage may incur costs depending on your subscription plans
- Some features may be limited by API rate limits

## 🤔 Support

For issues and questions:
1. Check existing GitHub issues
2. Create a new issue if needed
3. Include relevant details and error messages
