# Endowment Executive Dashboard

> **Repository:** fundriverdashboard  
> **Product Name:** Endowment Executive Dashboard

An interactive, browser-based financial dashboard for viewing and analyzing endowment fund performance data stored in Airtable.

## 📊 Overview

The Endowment Executive Dashboard is a standalone HTML application that connects to your Airtable database to provide comprehensive visualization and analysis of endowment fund data. It offers real-time insights into fund performance, trends, and detailed metrics through an intuitive, customizable interface.

**Version:** 2.1.0  
**Last Updated:** January 2026

## ✨ Key Features

### Data Visualization
- **Interactive KPI Cards** - Display key metrics including total assets, returns, and fund performance
- **Dynamic Charts** - Visualize trends and compare fund performance over time using Chart.js
- **Fund Details View** - Comprehensive data table with sortable columns and detailed fund information

### Customization Options
- **Brand Colors** - Customize 4 brand colors (primary, secondary, positive, negative) to match your organization
- **Custom Logo** - Upload and display your organization's logo
- **Field Name Customization** - Rename field labels to match your organization's terminology
- **Persistent Settings** - All customizations are saved in browser localStorage

### Data Management
- **Excel Export** - Export filtered data to Excel format for further analysis
- **Advanced Filtering** - Filter by fund type, purpose, date ranges, and more
- **Print Support** - Optimized print layout for reports

### Security & Privacy
- **Client-Side Only** - All data processing happens in your browser
- **Secure Storage** - API credentials stored only in browser localStorage
- **No External Servers** - Data is transmitted only between your browser and Airtable

## 🚀 Quick Start

### Prerequisites
- Modern web browser (Chrome, Firefox, Safari, or Edge)
- Airtable account with endowment fund data
- Airtable Personal Access Token

### Setup Instructions

1. **Download the Dashboard**
   - Download `Endowment Dashboard.html` from this repository
   - Save it to your local computer

2. **Open in Browser**
   - Double-click the HTML file to open it in your default browser
   - Or right-click and select "Open with" to choose a specific browser

3. **Configure Airtable Connection**
   - Click the "Settings" button in the header
   - Navigate to the "API Configuration" tab
   - Enter your credentials:
     - **Personal Access Token**: Get from [Airtable Settings](https://airtable.com/create/tokens)
     - **Base ID**: Found in your Airtable base URL
     - **Table ID**: Found in your Airtable table URL
   - Click "Connect" to load your data

4. **Customize Your Dashboard** (Optional)
   - **Brand Colors**: Set your organization's color scheme
   - **Logo**: Upload your organization's logo
   - **Field Names**: Customize field labels to match your terminology

## 📋 Required Airtable Fields

Your Airtable table must include the following fields:

| Field Name | Type | Description |
|------------|------|-------------|
| Date | Date | Transaction or reporting date (MM/DD/YYYY) |
| Fund ID | Text/Number | Unique fund identifier |
| Fund Name | Text | Name of the fund |
| Fund Type | Single/Multi-select | Type or category of fund |
| Purpose | Single/Multi-select | Fund purpose or designation |
| Beginning MV | Currency/Number | Beginning market value |
| Ending MV | Currency/Number | Ending market value |
| Ending Historical Gift | Currency/Number | Historical gift value |
| Realized Gains | Currency/Number | Realized gains for period |
| Unrealized Gains | Currency/Number | Unrealized gains for period |
| Investment Fees | Currency/Number | Investment management fees |
| Income | Currency/Number | Income generated |
| Gifts All | Currency/Number | All gifts received |
| Distributions All | Currency/Number | All distributions made |
| Expenses All | Currency/Number | All expenses incurred |
| Income to Principal | Currency/Number | Income transferred to principal |
| Transfers All | Currency/Number | All transfers |

## 🎨 Customization

### Brand Colors
Customize four color themes to match your organization:
- **Primary**: Main brand color (used in charts and KPI cards 1 & 3)
- **Secondary**: Accent color (used in trend lines and KPI cards 2 & 4)
- **Positive**: Color for gains and positive values
- **Negative**: Color for losses and negative values

### Logo Upload
- Upload your organization's logo (PNG, JPG, or SVG)
- Logo displays in the dashboard header
- Recommended size: 200x50 pixels

### Field Names
Customize field labels to match your organization's terminology while maintaining data field mappings.

## 🔒 Security & Privacy

- **Local Storage Only**: API credentials are stored exclusively in your browser's localStorage
- **No Third-Party Transmission**: Data is never sent to any server except Airtable
- **Clear Data**: Remove credentials and settings by clearing your browser data
- **Client-Side Processing**: All calculations and filtering happen in your browser

## 🛠️ Technologies Used

- **HTML5** - Structure and content
- **Tailwind CSS** - Styling and responsive design
- **JavaScript** - Application logic and interactivity
- **Chart.js** - Data visualization and charting
- **SheetJS (xlsx)** - Excel export functionality
- **Airtable API** - Data source integration

## 📖 Usage Tips

- **Filtering**: Use the filter panel to narrow down data by fund type, purpose, or date range
- **Exporting**: Click the "Export to Excel" button to download filtered data
- **Printing**: The dashboard automatically formats for print with a clean, professional layout
- **Data Refresh**: Data refreshes automatically when filters are applied or settings are changed

## 🤝 Support

For Airtable setup assistance or dashboard customization support, please contact your system administrator or refer to the [Airtable API documentation](https://airtable.com/developers/web/api/introduction).

## 📝 License

This project's license has not yet been specified. Please contact the repository owner for licensing information.

## 👥 Credits

Developed for endowment fund management and financial reporting.

---

**Note**: This is a standalone HTML application. No installation or server setup is required. Simply open the HTML file in a web browser and configure your Airtable connection to get started.
