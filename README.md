# SEBI Safe Space - Fraud Detection System

A comprehensive web-based fraud detection and investor protection platform designed to combat various types of financial fraud in the securities market.

## 🎯 Project Overview

This project was developed for the SEBI hackathon to address the growing problem of investment fraud. The platform helps protect retail investors by providing tools to verify advisors, scan suspicious URLs, check entities against scam databases, and report fraudulent activities.

## 🚨 Problem Statement

Fraudsters employ various deceptive tactics to exploit investors:
- Fraudulent advisors impersonating registered professionals
- Deepfake videos/audios of corporate leaders
- Misleading stock tips via WhatsApp/Telegram groups
- Fake trading apps and IPO schemes
- False corporate announcements causing market manipulation

## 💡 Solution

A multi-faceted web platform that:
- **Verifies SEBI registered advisors** against official databases
- **Scans URLs** for security threats using VirusTotal and IPQualityScore APIs
- **Checks entities** against comprehensive scam databases
- **Enables fraud reporting** with structured data collection
- **Provides AI-powered fraud detection** with risk scoring

## 🛠️ Tech Stack

**Frontend:**
- HTML5, CSS3, JavaScript (Vanilla)
- Font Awesome icons
- Google Fonts (Poppins)
- Responsive design

**Backend:**
- Python Flask
- Flask-CORS for cross-origin requests
- Python-dotenv for environment management

**APIs & Services:**
- VirusTotal API (URL/file scanning)
- IPQualityScore API (fraud detection)
- ScamSearch API (scam database lookup)

**Data Storage:**
- JSON files for advisor database
- Structured fraud reports

## 📁 Project Structure

```
sebi-safe-space/
├── app.py                 # Flask backend server
├── index.html            # Main frontend interface
├── advisors.json         # SEBI advisors database
├── requirements.txt      # Python dependencies
├── .env                  # API keys (create this)
├── README.md            # Project documentation
└── static/              # Static assets (optional)
```

## 🚀 Installation & Setup

### Prerequisites
- Python 3.7 or higher
- pip (Python package installer)

### Step 1: Clone/Download Project
```bash
git clone <repository-url>
cd sebi-safe-space
```

### Step 2: Install Dependencies
```bash
pip install -r requirements.txt
```

### Step 3: Configure API Keys
Create a `.env` file in the project root:
```env
VIRUSTOTAL_API_KEY=your_virustotal_api_key
IPQUALITYSCORE_API_KEY=your_ipqualityscore_api_key
SCAMSEARCH_API_KEY=your_scamsearch_api_key
```

### Step 4: Run the Application
```bash
python app.py
```

### Step 5: Access the Platform
Open your browser and navigate to:
```
http://127.0.0.1:5000
```

## 🔧 API Configuration

### VirusTotal API
1. Sign up at [VirusTotal](https://www.virustotal.com/)
2. Get your free API key
3. Add to `.env` file

### IPQualityScore API
1. Register at [IPQualityScore](https://www.ipqualityscore.com/)
2. Obtain API key
3. Add to `.env` file

### ScamSearch API
1. Contact ScamSearch for API access
2. Add credentials to `.env` file

**Note:** The system works with mock data even without API keys for testing purposes.

## 📊 Features

### 1. SEBI Advisor Verification
- Search by advisor name or registration number
- Real-time verification against SEBI database
- Displays complete advisor details and validity

### 2. URL Security Scanner
- Multi-engine URL scanning
- VirusTotal integration for malware detection
- IPQualityScore for phishing and fraud detection
- Detailed threat analysis and recommendations

### 3. Scam Watch Database
- Entity name verification
- Phone number fraud checking
- Domain reputation analysis
- Risk scoring and fraud indicators

### 4. Fraud Reporting System
- Structured fraud report collection
- Multiple fraud type categorization
- Evidence upload capability
- Automatic report ID generation

### 5. AI-Powered Fraud Detection
- Pattern recognition algorithms
- Risk scoring (0.0 to 1.0 scale)
- Behavioral analysis
- Continuous learning system

## 🔍 Usage Examples

### Verify an Advisor
1. Navigate to "Verify Advisor" section
2. Enter advisor name (e.g., "Abhishek Kumar") or registration number
3. Click "Verify Now"
4. Review detailed verification results

### Scan a Suspicious URL
1. Go to "Scan URL" section
2. Enter the website URL
3. Wait for multi-engine analysis
4. Review security assessment and recommendations

### Check Against Scam Database
1. Visit "Scam Watch" section
2. Select search type (Entity/Phone/Domain)
3. Enter the query
4. Analyze fraud risk indicators

## 📈 API Endpoints

| Endpoint | Method | Description |
|----------|--------|-------------|
| `/` | GET | Main application interface |
| `/verify_sebi` | POST | Verify SEBI advisor credentials |
| `/enhanced_url_scan` | POST | Comprehensive URL security scan |
| `/check_scam_database` | POST | Check entity against scam database |
| `/report_fraud` | POST | Submit fraud report |
| `/test` | GET | API health check and status |

## 🛡️ Security Features

- Input validation and sanitization
- CORS protection
- Rate limiting considerations
- Secure API key management
- Error handling with security in mind

## 📱 Responsive Design

- Mobile-friendly interface
- Tablet optimization
- Desktop experience
- Cross-browser compatibility

## 🚧 Development Status

**Current Version:** 1.0.0

**Features Implemented:**
- ✅ SEBI advisor verification
- ✅ Multi-API URL scanning
- ✅ Scam database integration
- ✅ Fraud reporting system
- ✅ Responsive UI/UX

**Planned Enhancements:**
- 🔄 Machine learning model integration
- 🔄 Real-time social media monitoring
- 🔄 Corporate announcement verification
- 🔄 Advanced fraud pattern detection

## 🤝 Contributing

This project was developed for the SEBI hackathon. Future contributions are welcome for:
- Enhanced fraud detection algorithms
- Additional API integrations
- UI/UX improvements
- Performance optimizations

## 📄 License

This project is developed for educational and hackathon purposes. Please ensure compliance with all applicable regulations and terms of service for integrated APIs.

## 📞 Support

For issues or questions:
1. Check the Flask console for error messages
2. Verify all dependencies are installed
3. Ensure API keys are properly configured
4. Test individual endpoints using `/test`

