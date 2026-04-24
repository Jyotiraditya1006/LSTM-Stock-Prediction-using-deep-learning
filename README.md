📈 Stock Price Prediction using LSTM Neural Networks
Python Keras Streamlit License Deploy

A professional deep learning application for predicting stock prices using LSTM neural networks with an interactive web dashboard.

🚀 Live Demo | 📖 Documentation

✨ Features
🎯 Core Capabilities
Deep Learning Model: 4-layer LSTM neural network with dropout regularization
Real-time Data: Fetches live stock data from Yahoo Finance
Interactive Dashboard: Professional Streamlit web interface with 5 specialized tabs
Technical Analysis: RSI, MACD, Bollinger Bands, and ADX indicators
Future Predictions: Forecast stock prices up to 90 days ahead
Performance Metrics: RMSE, MAE, MAPE, and accuracy calculations
Data Export: Download predictions and historical data as CSV
📊 Dashboard Tabs
Overview - Real-time stock data with key metrics
Predictions - Historical predictions vs actual prices
Technical Analysis - Interactive charts with indicators
Model Performance - Detailed metrics and evaluation
About - Project information and documentation
🛠️ Tech Stack
Category	Technologies
Deep Learning	Keras 3.11, JAX Backend, NumPy
Data Processing	Pandas, Scikit-learn
Visualization	Plotly, Matplotlib, Seaborn
Web Framework	Streamlit 1.50
Data Source	yfinance API
Technical Indicators	TA-Lib
Deployment	Render, Docker-ready
🚀 Quick Start
Prerequisites
Python 3.10+ (Python 3.14 recommended)
Git
2GB RAM minimum
Local Installation
Clone the repository
git clone https://github.com/sohamrp172-sys/stock-price-prediction.git
cd stock-price-prediction
Create virtual environment
python -m venv dl-project
# Windows
dl-project\Scripts\activate
# Linux/Mac
source dl-project/bin/activate
Install dependencies
pip install -r requirements.txt
Train the model (Optional - pre-trained model included)
# Run the Jupyter notebook or Python script
jupyter notebook "Stock Predictions Model.keras.ipynb"
Run the application
streamlit run app_enhanced.py
Open in browser
http://localhost:8501
📦 Project Structure
stock-price-prediction/
├── 📄 app_enhanced.py              # Main Streamlit application
├── 📓 Stock Predictions Model.keras.ipynb  # Training notebook
├── 🧠 Stock_Predictions_Model.keras        # Trained model file
├── 📋 requirements.txt             # Python dependencies
├── 📖 README.md                    # This file
├── 🔧 render.yaml                  # Render deployment config
├── 🔧 start.sh                     # Startup script
├── 📁 .streamlit/
│   └── config.toml                 # Streamlit configuration
🎓 Model Architecture
Input (100-day sequences)
    ↓
LSTM(50 units) + Dropout(0.2)
    ↓
LSTM(60 units) + Dropout(0.3)
    ↓
LSTM(80 units) + Dropout(0.4)
    ↓
LSTM(120 units) + Dropout(0.5)
    ↓
Dense(1 unit) - Price Prediction
Training Details
Optimizer: Adam
Loss Function: Mean Squared Error (MSE)
Training Epochs: 50
Batch Size: 32
Train/Test Split: 80/20
Data Normalization: MinMaxScaler [0,1]
Lookback Window: 100 days
📊 Performance
Metric	Value
RMSE	~$X.XX
MAE	~$X.XX
MAPE	~X.XX%
Accuracy	~XX%
Note: Run the model to see actual metrics

🌐 Deployment
Deploy to Render (Free)
Fork this repository to your GitHub account

Sign up at Render.com

Create New Web Service

Connect your GitHub repository
Select this project
Render will auto-detect render.yaml
Deploy!

Click "Create Web Service"
Wait 5-10 minutes for deployment
Your app will be live! 🎉
For detailed instructions, see DEPLOYMENT.md

Alternative Deployments
Streamlit Cloud: One-click deployment
Heroku: Traditional PaaS
AWS/GCP/Azure: Cloud platforms
Docker: Container deployment
📚 Usage
Basic Usage
Open the web application
Enter a stock ticker (e.g., GOOG, AAPL, TSLA)
Select date range
View predictions and technical analysis
Download data as CSV
Advanced Features
Custom Date Ranges: Analyze any historical period
Future Predictions: Forecast 7-90 days ahead
Technical Indicators: RSI, MACD, Bollinger Bands
Interactive Charts: Zoom, pan, and explore data
Model Metrics: Detailed performance analysis
🔬 Technical Indicators
Indicator	Description	Use Case
RSI	Relative Strength Index	Identify overbought/oversold conditions
MACD	Moving Average Convergence Divergence	Trend momentum and direction
Bollinger Bands	Volatility bands	Price volatility and breakouts
ADX	Average Directional Index	Trend strength
Moving Averages	100-day & 200-day MA	Long-term trends
📝 License
This project is licensed under the MIT License - see the LICENSE file for details.

⚠️ Disclaimer
Important: This application is for educational and research purposes only.

❌ NOT financial advice
❌ NOT investment recommendations
❌ Past performance does NOT guarantee future results
✅ Use for learning and portfolio demonstration
✅ Always do your own research before investing
🙏 Acknowledgments
Yahoo Finance for providing free stock data API
Streamlit for the amazing web framework
Keras Team for the deep learning framework
JAX Team for the high-performance backend
Open Source Community for all the amazing libraries
🔮 Future Enhancements
 Add more stock exchanges (NSE, BSE, etc.)
 Implement sentiment analysis from news
 Multi-stock portfolio analysis
 Real-time WebSocket data streaming
 Mobile-responsive design
 User authentication and saved preferences
 Email alerts for price targets
 API endpoint for predictions
 Docker containerization
 CI/CD pipeline
