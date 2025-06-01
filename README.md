# Echoing Healthy Ageing - Interactive Strategy

An interactive web application showcasing a comprehensive marketing strategy for dementia awareness in India. This project aims to increase awareness, early detection, and compassionate care for India's ageing population.

## 🚀 Live Demo

Visit the live site: [https://adarshalexbalmuchu.github.io/echoinghealthyageing/](https://adarshalexbalmuchu.github.io/echoinghealthyageing/)

## ✨ Features

- **Interactive Personas**: Detailed profiles of key audience segments
- **Data Visualizations**: Charts showing dementia prevalence and treatment gaps
- **AI-Powered Insights**: Gemini AI integration for personalized advice
- **Responsive Design**: Mobile-first design with Tailwind CSS
- **Smooth Navigation**: Sticky navigation with scroll-based highlighting

## 🛠️ Setup Instructions

### For GitHub Pages Deployment

1. **Fork or Clone** this repository
2. **Enable GitHub Pages** in your repository settings
3. **Set source** to deploy from the main branch
4. **Optional**: Configure custom domain if desired

### For AI Features (Optional)

To enable the full AI-powered insights feature:

1. **Get a Gemini API Key**:
   - Visit [Google AI Studio](https://makersuite.google.com/app/apikey)
   - Create a new API key
   - Copy the key

2. **Configure the API Key Securely**:
   
   **Option A: Using config.js (Recommended for local development)**
   ```bash
   # Copy the example configuration file
   cp config.example.js config.js
   
   # Edit config.js and add your API key
   # The file is already in .gitignore so it won't be committed
   ```
   
   **Option B: Using environment variables (For production)**
   - Set `GEMINI_API_KEY` as an environment variable in your hosting service
   - The application will automatically use it

   **⚠️ SECURITY WARNING**: Never commit API keys directly in your code! Always use:
   - Configuration files that are gitignored
   - Environment variables
   - Secure secret management services

3. **Deploy** your changes

> **Note**: Without an API key, the application will show helpful fallback content instead of AI-generated insights.

## 📊 Data Sources

The visualizations are based on research data about dementia in India:
- Population statistics from national health surveys
- Prevalence data from medical research studies
- Treatment gap analysis from healthcare reports

## 🎨 Design System

- **Primary Color**: `#c7923e` (Golden brown)
- **Background**: `#fdfaf7` (Warm cream)
- **Text**: `#3f3c3a` (Dark brown)
- **Font**: Inter (Google Fonts)

## 🔧 Technologies Used

- **HTML5**: Semantic markup
- **CSS3**: Custom styles with Tailwind CSS
- **JavaScript**: Vanilla JS for interactivity
- **Chart.js**: Data visualization library
- **Gemini AI**: Google's AI for personalized insights
- **GitHub Pages**: Static site hosting

## 📱 Browser Support

This application is compatible with all modern browsers:
- Chrome (recommended)
- Firefox
- Safari
- Edge

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📧 Contact

For questions or feedback about this project, please open an issue in the GitHub repository.

---

**Built with ❤️ for advancing dementia awareness in India**
