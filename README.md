# AI/ML Projects for Students - Flask Website

A modern Flask website for an AI/ML startup that helps college students get beginner-level AI/ML projects for submissions and internships.

## Features

- **Home Page**: Welcome message and service overview
- **Services Page**: Detailed list of AI/ML services offered
- **Submit Project Page**: Google Form integration for project submissions
- **Contact Page**: Multiple contact methods and FAQ section
- **Responsive Design**: Mobile-friendly interface
- **Modern UI**: Clean, professional design with smooth animations

## Project Structure

```
website/
├── app.py                 # Main Flask application
├── requirements.txt       # Python dependencies
├── README.md             # Project documentation
├── static/
│   └── style.css         # CSS styles
└── templates/
    ├── base.html         # Base template with navigation
    ├── index.html        # Home page
    ├── services.html     # Services page
    ├── submit.html       # Submit project page
    └── contact.html      # Contact page
```

## Setup Instructions

### Prerequisites
- Python 3.7 or higher
- pip (Python package installer)

### Installation

1. **Clone or download the project files**

2. **Navigate to the project directory**
   ```bash
   cd website
   ```

3. **Create a virtual environment (recommended)**
   ```bash
   python -m venv venv
   ```

4. **Activate the virtual environment**
   - On Windows:
     ```bash
     venv\Scripts\activate
     ```
   - On macOS/Linux:
     ```bash
     source venv/bin/activate
     ```

5. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

6. **Run the application**
   ```bash
   python app.py
   ```

7. **Open your browser and go to**
   ```
   http://localhost:5000
   ```

## Customization

### Adding Your Google Form

1. Create a Google Form with your project submission fields
2. Click "Send" and copy the embed code
3. Replace the placeholder in `templates/submit.html` with your iframe code

### Updating Contact Information

Edit `templates/contact.html` to update:
- Email address
- Telegram handle
- WhatsApp number

### Styling

Modify `static/style.css` to customize colors, fonts, and layout.

## Free Deployment Options

### 1. Render (Recommended)
- **Pros**: Free tier, easy setup, automatic deployments
- **Steps**:
  1. Create account at [render.com](https://render.com)
  2. Connect your GitHub repository
  3. Create a new Web Service
  4. Set build command: `pip install -r requirements.txt`
  5. Set start command: `gunicorn app:app`

### 2. Replit
- **Pros**: Free, includes IDE, instant deployment
- **Steps**:
  1. Go to [replit.com](https://replit.com)
  2. Create new Python project
  3. Upload your files
  4. Add `gunicorn` to requirements.txt
  5. Set run command: `gunicorn app:app --bind 0.0.0.0:8080`

### 3. Railway
- **Pros**: Free tier, GitHub integration
- **Steps**:
  1. Create account at [railway.app](https://railway.app)
  2. Connect GitHub repository
  3. Deploy automatically

### 4. Heroku (Alternative)
- **Note**: No longer free, but still popular
- **Steps**:
  1. Create account at [heroku.com](https://heroku.com)
  2. Install Heroku CLI
  3. Add `gunicorn` to requirements.txt
  4. Create `Procfile` with: `web: gunicorn app:app`
  5. Deploy using Heroku CLI

## Additional Files for Deployment

### For Render/Railway/Heroku, add to requirements.txt:
```
gunicorn==21.2.0
```

### For Heroku, create Procfile:
```
web: gunicorn app:app
```

## Development

### Running in Development Mode
```bash
python app.py
```

### Running in Production Mode
```bash
gunicorn app:app
```

## Features Included

- ✅ Responsive navigation with mobile menu
- ✅ Modern gradient backgrounds
- ✅ Hover animations and transitions
- ✅ Contact form with validation
- ✅ FAQ section
- ✅ Google Form integration placeholder
- ✅ Professional typography with Inter font
- ✅ Mobile-first responsive design
- ✅ Clean, modern UI/UX

## Support

For any issues or questions, please contact:
- Email: 29pranjalgupta@gmail.com
- Update the contact page with your actual Telegram/WhatsApp details

## License

This project is open source and available under the MIT License. 