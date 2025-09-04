# Financial Statement Analysis Application
A comprehensive application for analyzing financial statements from PDF reports. This application combines a Python backend for PDF parsing and financial analysis with a React frontend for data visualization and exploration.

## Features
* PDF Parsing: Extract financial data from annual reports and financial statements
* Financial Analysis: Analyze income statements, balance sheets, and cash flow statements
* Data Visualization: Visualize financial trends and key metrics
* QA Checks: Automatic quality assurance checks on financial data
* Semantic Search: Search through financial notes and MD&A sections
## System Requirements
* Python 3.10+
* Node.js 18+
* Windows, macOS, or Linux
## Quick Start
For a quick start with minimal setup, use the provided run_app.bat script (Windows):   

run_app.bat   

This will:  
1.Create a Python virtual environment (if it doesn't exist)   
2.Install all Python dependencies   
3.Install all Node.js dependencies   
4.Start the backend server   
5.Start the frontend development server   
Once started, navigate to http://localhost:3000 in your web browser.

# Step by Step Installation
If you prefer to install and run the application manually, follow these steps:

## Backend Setup
 1.Clone the repository:   
 
 git clone https://github.com/your-username/Financial_statement_analysis.git   
 cd Financial_statement_analysis 
 
 2.Create a virtual environment:   
 
 python -m venv venv   
 
 3.Activate the virtual environment:

* Windows:
venv\Scripts\activate
* macOS/Linux:
source venv/bin/activate

4.Install Python dependencies:

pip install -r npnonlyf/requirements.txt   

## Frontend Setup
1.Navigate to the client directory:

cd client   
2.Install Node.js dependencies:

npm install
# Running the Application
## Start the Backend Server
python server.py    
The backend server will run at http://localhost:5000.

## Start the Frontend Server
In a new terminal, navigate to the client directory and run:   
npm run dev   
The frontend will be available at http://localhost:3000.

# Using the Application
## 1. Upload a Financial Statement PDF
Click on the "Upload" button on the dashboard
Select a financial statement PDF (annual report, 10-K filing, etc.)
Wait for the processing to complete
## 2. Analyze Financial Data
After processing, select a company from the dropdown
The application will display the available years for that company
View financial data, trends, and quality assurance findings
## 3. Search and Explore
Use the search functionality to find specific information in the financial notes
Export data as needed
# What Kind of PDFs Will Work?
## Supported Financial Document Types
* Annual Reports from publicly traded companies
* 10-K Filings submitted to the SEC
* Financial Statements with clear tabular data
* Both text-based and scanned PDFs (with OCR support)
# Required Content
## For best results, the PDF should contain:   
1.Income Statement data (revenue, expenses, profits)   
2.Balance Sheet data (assets, liabilities, equity)   
3.Cash Flow Statement data   
4.Clear tabular data with financial figures   
5.Financial notes sections for semantic search

# Developer Guide
## Backend Structure
* server.py: Flask API server
* npnonlyf/pdf_parser.py: PDF extraction logic
* npnonlyf/pipeline.py: Main data processing pipeline
* npnonlyf/embeddings.py: Text embeddings for semantic search
* npnonlyf/qa_checks.py: Quality assurance checks for financial data
## Frontend Structure
* src/context/AppContext.tsx: Main application state management
* src/components/: React components
* src/services/api.ts: API client for backend communication
* src/types/index.ts: TypeScript type definitions
## Adding New Features
Refer to the component architecture and API documentation in the codebase for guidance on extending the application.
