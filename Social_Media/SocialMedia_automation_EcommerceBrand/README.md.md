# AI Social Media Agent for E-commerce

An intelligent, autonomous social media automation system that generates and publishes daily content for Facebook and Instagram using product data from an e-commerce website.

## 🎯 Workflow Overview

![AI Social Media Agent Workflow](workflow_screenshot.png)

The workflow is organized into four distinct phases:

1. **Data Collection & Storage Phase** (Blue) - Fetches and processes product data from XML feeds
2. **Content Selection & Creation Phase** (Purple) - Selects products and generates AI-powered content
3. **Media Processing & Publishing Phase** (Red) - Publishes optimized content to social platforms
4. **Status Tracking & Database Update Phase** (Green) - Updates posting history and prevents duplicates

## 📋 Problem Statement

The client needed to automate repetitive social media marketing tasks:

- **Manual Content Creation**: Daily social media posts required 30+ minutes of manual work
- **Platform Optimization**: Different content formats needed for Facebook vs Instagram
- **Content Management**: Risk of duplicate posts without proper tracking
- **Scalability**: Growing product catalog made manual posting unsustainable
- **Cost Concerns**: Required budget-friendly, self-hosted solution

## ✨ Key Features

### Intelligent Content Generation
- **AI-Powered**: Uses AI for natural, engaging content in target language
- **Platform-Specific**: 
  - Facebook: 150-250 words with storytelling
  - Instagram: 50-100 words with 5-7 hashtags
- **Brand Voice**: Maintains consistent brand tone

### Smart State Management
- **Duplicate Prevention**: Google Sheets tracks all posted products
- **Queue System**: Manages pending products automatically
- **Status Tracking**: Records posting dates and social media IDs

### Robust Error Handling
- **Rate Limit Compliance**: Respects Instagram's 20 posts/day limit
- **Automatic Recovery**: Handles API failures gracefully
- **Email Notifications**: Real-time alerts for any issues
- **Comprehensive Logging**: Detailed error tracking in Google Sheets

## 🛠️ Technical Stack

- **Automation**: n8n (self-hosted)
- **AI Service**: OpenAI API
- **Social APIs**: Meta Graph API (Facebook & Instagram)
- **Storage**: Google Sheets
- **Deployment**: Docker on VPS (~$5-10/month)

## 📊 How It Works

1. **Schedule Trigger** - Runs daily at scheduled time
2. **Fetch Products** - Retrieves XML feed from e-commerce site
3. **Parse & Structure** - Converts XML to structured product data
4. **Update Database** - Syncs products with Google Sheets
5. **Select Product** - Randomly chooses from pending products
6. **Generate Content** - AI creates platform-optimized posts
7. **Process Images** - Downloads and prepares product photos
8. **Publish Posts** - Posts to Facebook and Instagram
9. **Update Status** - Marks products as posted, logs results

## 🚀 Results

- ✅ **100%** automation of daily posting
- ✅ **Zero** duplicate content
- ✅ **30+ minutes** saved daily
- ✅ **99%+** uptime with error handling
- ✅ **365 days/year** consistent presence

## 📈 Monitoring

Track performance through:
- **Google Sheets Dashboard**: Posting history and success rates
- **Error Logs**: Detailed failure analysis
- **Email Alerts**: Real-time error notifications
- **Execution History**: Complete audit trail

## 🔒 Security

- Self-hosted deployment ensures data privacy
- Secure credential management via n8n
- No third-party data storage
- Regular backup procedures

## 📞 Maintenance

Designed for minimal maintenance:
- Automatic error recovery
- Self-updating product data
- Comprehensive logging for troubleshooting
- Modular design for easy updates

---

*Built with n8n to demonstrate enterprise-grade automation combining AI, multiple APIs, and robust error handling for professional social media management.*