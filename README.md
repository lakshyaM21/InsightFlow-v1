📊 Insight Flow
AI-Assisted Business Analytics Dashboard

Python Streamlit Plotly Gemini AI

A fully customizable, retro desktop-inspired analytics platform that turns raw CSV data into interactive insights and comprehensive PDF reports using the power of Google's Gemini AI.




🚀 Overview
Insight Flow is a fully Python-driven analytics platform that allows users to upload structured CSV business datasets, visualize insights through interactive dashboards, and interact with a context-constrained Gemini AI assistant.

It features a professional, retro desktop-inspired aesthetic with dynamic UI theme switching and the ability to export complete analytics sessions—including AI chat history—to a stylized PDF report.

✨ Features
📁 Seamless Data Ingestion: Upload any structured CSV. The system automatically detects dates, numbers, and categories, handling missing data gracefully.
🎨 Dynamic Theming Engine: Change the entire dashboard appearance in real time. Features 6 bespoke themes that automatically synchronize Plotly charts with the UI:
🟠 Normal Default
🔵 Vintage Blue
👑 Royal Gold
⬛ Dark Matte
🌫️ Slate
🧊 Glassmorphism
📈 Interactive Visualizations: Includes fully interactive bar, line, area, pie, donut, scatter, stacked bar charts, histograms, and heatmaps.
🤖 AI-Assisted Analytics (Gemini API): An executive summary generator and a dedicated AI chat assistant strictly constrained to the context of the uploaded dataset.
📄 Executive PDF Export: Generate professional presentation-ready PDF reports with all-time business KPI overviews, visual charts, and a complete session log of your AI Q&A conversation.
📂 Folder Structure
InsightFlow-v1/
├── app.py                   # Main Streamlit application
├── analytics_engine.py      # Business logic & KPI calculations
├── chart_builder.py         # Dynamic Plotly visualizations
├── data_processor.py        # CSV parsing & validation
├── gemini_handler.py        # AI integration & conversation management
├── pdf_generator.py         # ReportLab-powered PDF exporter
├── styles.py                # CSS generation & injection
├── theme_engine.py          # Configuration for the 6 visual themes
├── requirements.txt         # Project dependencies
├── sample_data.csv          # Example dataset
├── generate_project_pdf.py  # Utility to export codebase
├── .env.example             # Environment template
└── README.md                # Project documentation
📊 CSV Data Format Requirements
Insight Flow works best with standard structured business or time-series data (e.g., sales logs, website analytics, user data, etc.).

To ensure the system works as intended, your CSV must contain:

🗓️ At least one Date column: (e.g., Date, Timestamp, Created_At). The system is quite flexible and parses most standard date formats (like YYYY-MM-DD, MM/DD/YYYY).
🔢 At least one Numeric column: (e.g., Revenue, Sales, Quantity, Visits, Temperature). Used for KPI generation and primary chart axes.
Optional but recommended:

🏷️ Categorical columns: (e.g., Region, Product Category, Status, User Segment). Used to generate breakdowns, pie charts, and segment analysis.
Example CSV Structure:
Date,Region,Product,Revenue,Quantity
2023-01-15,North,Software,1500.50,10
2023-01-16,South,Hardware,850.00,5
2023-01-17,North,Hardware,1200.00,8
🏢 Our Services InsightFlow services
📊 Direct use InsightFlow v1
💻 How to Run
Prerequisites
Python 3.8+
Gemini API Key (Optional, but highly recommended for AI insights and chat features)
Installation
Clone the repository and navigate to the project directory:

git clone https://github.com/yourusername/InsightFlow-v1.git
cd InsightFlow-v1
Install the required dependencies:

pip install -r requirements.txt
Configuration (Optional)
To automatically connect the AI without typing your key in the dashboard every time:

Copy or rename .env.example to .env (or create a new .env file in the root directory).
Add your Gemini API key to the file:
GEMINI_API_KEY=your_actual_api_key_here
🚀 Running the Application
Start the Streamlit server by running the following command in your terminal:

streamlit run app.py
This will automatically open the dashboard in your default web browser at http://localhost:8501.



Built with ❤️ using Python and Streamlit
