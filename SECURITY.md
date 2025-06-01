# Security Guidelines

## API Key Management

### Current Security Measures

1. **No Hardcoded Secrets**: All API keys have been removed from the source code
2. **Environment Variable Support**: The application checks for `process.env.GEMINI_API_KEY`
3. **Configuration File Support**: Optional `config.js` file for local development
4. **Gitignore Protection**: `config.js` is excluded from version control

### API Key Configuration Options

#### Option 1: Configuration File (Local Development)
```bash
# Copy the example file
cp config.example.js config.js

# Edit config.js and add your API key
# This file is gitignored and will not be committed
```

#### Option 2: Environment Variables (Production)
Set the `GEMINI_API_KEY` environment variable in your hosting service:
- Vercel: Add to Environment Variables in project settings
- Netlify: Add to Site Settings > Environment Variables
- GitHub Pages: Use GitHub Secrets for build actions

### Security Checklist

- ✅ API keys removed from source code
- ✅ Configuration files gitignored
- ✅ Environment variable support added
- ✅ Fallback handling for missing keys
- ✅ Security documentation created
- ✅ README updated with secure setup instructions

### What to Do if Keys are Exposed

1. **Immediately revoke** the exposed API key in Google AI Studio
2. **Generate a new** API key
3. **Update** your configuration with the new key
4. **Verify** the old key is no longer functional
5. **Review** git history and consider rewriting if necessary

### Regular Security Maintenance

- Review and rotate API keys periodically
- Monitor for any new secrets in code using tools like GitHub's secret scanning
- Keep dependencies updated
- Use security scanning tools in CI/CD pipeline

## Contact

For security issues, please create a private issue or contact the repository maintainer directly.
