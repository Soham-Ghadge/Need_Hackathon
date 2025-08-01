# 📊 Neueda – Portfolio Management App

A modular Streamlit-based application for comprehensive stock portfolio analysis and management. Built with clean architecture principles for hackathons, rapid prototyping, and professional development.

## 🚀 Features

- **Portfolio Performance Analysis** - Track returns, volatility, and key metrics
- **Individual Stock Analysis** - Detailed stock-level insights and visualizations  
- **Risk Management** - Value at Risk (VaR) calculations and risk metrics
- **Correlation Analysis** - Understand portfolio diversification and relationships
- **Interactive Dashboard** - Clean, responsive UI with real-time updates
- **File Upload Support** - Easy CSV import for portfolio data
- **Customizable Weights** - Dynamic portfolio weight adjustments

## 🗂️ Project Structure

```
portfolio_management/
├── app.py                          # Main application entry point
├── models/
│   ├── __init__.py
│   └── portfolio.py               # Portfolio management logic
├── components/
│   ├── __init__.py
│   ├── sidebar.py                 # Sidebar with file upload and weights
│   ├── overview.py                # Overview tab component
│   ├── individual_stocks.py       # Individual stock analysis
│   ├── portfolio_analysis.py      # Portfolio performance analysis
│   ├── correlation_analysis.py    # Correlation analysis
│   └── risk_metrics.py            # Risk metrics and VaR
├── utils/
│   ├── __init__.py
│   ├── data_loader.py             # Data loading utilities
│   └── calculations.py            # Financial calculations
└── config/
    ├── __init__.py
    └── settings.py                # Configuration and styling
```

## 🛠️ Installation & Setup

### Prerequisites
- Python 3.8+
- pip package manager

### Quick Start

1. **Clone and create project structure:**
   ```bash
   git clone <your-repo-url>
   cd neueda-portfolio-management
   
   # Create directory structure if not present
   mkdir -p models components utils config
   ```

2. **Create Python packages:**
   ```bash
   # Add __init__.py files to make proper Python packages
   touch models/__init__.py components/__init__.py utils/__init__.py config/__init__.py
   ```

3. **Install dependencies:**
   ```bash
   pip install streamlit pandas numpy plotly seaborn matplotlib yfinance
   ```

4. **Run the application:**
   ```bash
   streamlit run app.py
   ```

5. **Access the app:**
   Open your browser to `http://localhost:8501`

## 📋 Usage

1. **Upload Portfolio Data**: Use the sidebar to upload a CSV file with your portfolio holdings
2. **Adjust Weights**: Modify portfolio weights using the interactive controls
3. **Analyze Performance**: Navigate through different tabs for comprehensive analysis:
   - **Overview**: High-level portfolio summary
   - **Individual Stocks**: Stock-by-stock breakdown
   - **Portfolio Analysis**: Performance metrics and trends
   - **Correlation Analysis**: Diversification insights
   - **Risk Metrics**: VaR and risk assessment

## 📊 CSV Format

Your portfolio CSV should include columns such as:
```csv
Symbol,Shares,Price
AAPL,100,150.00
GOOGL,50,2500.00
MSFT,75,300.00
```

## 🏗️ Architecture

### Modular Design
- **`app.py`**: Clean main orchestrator with minimal logic
- **`models/portfolio.py`**: Core portfolio management with clean interfaces
- **`utils/data_loader.py`**: Robust file handling and data validation
- **`utils/calculations.py`**: Centralized financial calculations
- **`components/`**: Focused, reusable UI components for each analysis tab
- **`config/settings.py`**: Centralized configuration management

### Key Benefits
- **Separation of Concerns**: Each module has a single responsibility
- **Testability**: Isolated functions easy to unit test
- **Maintainability**: Clear structure for easy debugging and updates
- **Scalability**: Modular design supports feature additions
- **Reusability**: Components can be easily reused across projects

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🐛 Issues & Support

If you encounter any issues or have questions:
- Check the [Issues](../../issues) page
- Create a new issue with detailed description
- Include error messages and steps to reproduce

## 🎯 Roadmap

- [ ] Real-time data integration
- [ ] Advanced portfolio optimization
- [ ] Export functionality for reports
- [ ] Machine learning predictions
- [ ] Multi-currency support
- [ ] Backtesting capabilities

---

**Built with ❤️ for efficient portfolio management and analysis**
