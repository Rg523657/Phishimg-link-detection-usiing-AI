# Phishing Link Detection System

A simplified machine learning-based system to detect potentially malicious URLs and protect users from phishing attacks.

## Features

- **Real-time URL Analysis**: Instantly analyze any URL for phishing indicators
- **ML-Powered Detection**: Uses feature extraction and scoring algorithms
- **Detailed Risk Assessment**: Shows specific risk factors and confidence scores
- **User-Friendly Interface**: Clean, responsive web interface
- **Educational**: Explains how the detection works

## How It Works

### 1. Feature Extraction
The system analyzes various URL characteristics:
- URL length and structure
- Domain properties
- HTTPS usage
- Subdomain count
- Suspicious keywords
- IP address usage
- URL shorteners

### 2. Risk Scoring
Each feature contributes to a risk score:
- Long URLs (+0.2)
- No HTTPS (+0.25)
- Suspicious keywords (+0.3)
- IP addresses (+0.4)
- Multiple subdomains (+0.2)

### 3. Classification
URLs with risk scores > 0.5 are flagged as potentially malicious.

## Usage

1. Enter a URL in the input field
2. Click "Analyze URL"
3. Review the detailed results including:
   - Safety classification
   - Confidence score
   - Feature analysis
   - Risk factors

## Example URLs to Test

**Safe URLs:**
- https://www.google.com
- https://github.com
- https://stackoverflow.com

**Suspicious Patterns:**
- http://secure-bank-update.suspicious.com/login
- https://192.168.1.1/microsoft-account
- http://bit.ly/account-verify-now

## Technical Implementation

- **Frontend**: Next.js with React and Tailwind CSS
- **Backend**: Next.js API routes
- **ML Approach**: Feature-based scoring with rule-based classification
- **Training Script**: Python script showing how to train a more sophisticated model

## Limitations

This is a simplified educational example. Production systems would need:
- Larger training datasets (10,000+ samples)
- More sophisticated ML models
- Real-time threat intelligence
- Regular model updates
- Advanced feature engineering

## Security Note

This tool is for educational purposes. Always use multiple layers of security and keep your systems updated.
