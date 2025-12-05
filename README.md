# AWS-Amplify-Portfolio

## 🌐 About This Project

A modern, responsive portfolio website showcasing my journey as a Cloud Computing Professional with expertise in AWS services and Linux systems administration. This multi-page application highlights my transition from healthcare to IT, technical skills, certifications, and professional experience in cloud technologies.

---

## 🛠️ Technologies & Architecture

This portfolio is built using modern web technologies and AWS cloud services:

### Frontend Technologies
- **HTML5**: Semantic markup with accessibility features
- **CSS3**: Custom responsive design with modern animations and effects
- **Vanilla JavaScript**: Interactive elements including rotating titles and form handling
- **Font Awesome**: Professional iconography throughout the site

### AWS Cloud Services
- **AWS Amplify**: Static web hosting and continuous deployment
- **API Gateway**: RESTful API endpoint for contact form
- **AWS Lambda**: Serverless function for email processing
- **Amazon SES**: Email service for contact form submissions
- **S3**: Resume file hosting and storage

### Design Features
- **Responsive Design**: Mobile-first approach with breakpoints for all devices
- **Modern UI/UX**: Dark gradient theme with cyan and green accent colors
- **Glass Morphism**: Backdrop blur effects and translucent cards
- **Interactive Elements**: Hover effects, rotating job titles, and smooth animations
- **Consistent Design System**: Unified styling across all pages

---

## 📁 Project Structure

```
.
├── images/                    # Profile photos and background images
│   ├── Gustav V. Kiewiets.jpg # Professional headshot
│   └── Laptop.jpg            # Hero section background
├── about.html                # About me page with interests and background
├── contact.html              # Contact form with AWS integration
├── index.html                # Main landing page
├── location.html             # Location/availability information
├── qualifications.html       # Education and certifications
├── recommendations.html      # Professional recommendations
├── tools&platforms.html      # Technical skills and tools
├── style.css                 # Main stylesheet with responsive design
└── README.md                 # Project documentation
```

---

## 🚀 Key Features

### Core Functionality
- **Multi-page Portfolio**: Six dedicated pages covering all professional aspects
- **Interactive Landing Page**: Hero section with rotating job titles and statistics
- **Professional Timeline**: Visual qualifications and career progression
- **Skills Showcase**: Organized tools and platforms with hover effects
- **Recommendations**: Professional endorsements with download links
- **Contact Integration**: AWS-powered contact form with real-time feedback
- **Location Information**: Availability and work preferences

### Technical Highlights
- **Serverless Architecture**: Contact form powered by AWS Lambda and API Gateway
- **Modern CSS**: Flexbox layouts, CSS Grid, and smooth transitions
- **Vanilla JavaScript**: No framework dependencies for fast loading
- **SEO Optimized**: Semantic HTML structure and meta tags
- **Accessibility**: ARIA labels and keyboard navigation support

### Interactive Elements
- **Rotating Job Titles**: 4 different roles cycling every 3 seconds
- **Timeline Animation**: Interactive career progression with hover effects
- **Card Interactions**: Transform animations on all content cards
- **Form Feedback**: Loading states and success/error notifications
- **Responsive Navigation**: Mobile-friendly design across all pages

---

## 📸 Preview

https://github.com/user-attachments/assets/036113ef-e119-4c1f-88e8-602a68aeb513

---

## 🌐 Live Demo

**Portfolio Website**: [https://main.d3d5cnpn2eqq65.amplifyapp.com](https://main.d3d5cnpn2eqq65.amplifyapp.com)

---

## 🚀 Local Development

### Prerequisites
- Modern web browser (Chrome, Firefox, Safari, Edge)
- Local web server (optional, for testing contact form)

### Quick Start

1. **Clone the repository**
   ```bash
   git clone https://github.com/gus-hub-tech/gus-amplify-site.git
   cd gus-amplify-site
   ```

2. **Open in browser**
   ```bash
   # Option 1: Direct file access
   open index.html
   
   # Option 2: Local server (recommended)
   python -m http.server 8000
   # Then visit http://localhost:8000
   ```

### Development Notes
- **No Build Process**: Pure HTML/CSS/JS - no compilation required
- **Static Files**: All assets are self-contained
- **Contact Form**: Requires AWS services for full functionality
- **Responsive Testing**: Use browser dev tools to test different screen sizes

---

## 🏗️ AWS Infrastructure

### Contact Form Architecture
```
Contact Form → API Gateway → Lambda Function → Amazon SES → Email Delivery
```

### Services Configuration
- **API Gateway**: RESTful endpoint at `https://tmlwb24aff.execute-api.af-south-1.amazonaws.com/Production_Stage/SendMailFunctionSES`
- **Lambda Function**: Processes form data and sends emails via SES
- **S3 Bucket**: Hosts resume PDF with public read access
- **Amplify**: Continuous deployment from GitHub repository

---

## 📱 Responsive Breakpoints

- **Desktop**: 1200px and above
- **Tablet**: 900px - 1199px
- **Mobile Large**: 600px - 899px
- **Mobile Small**: Below 600px

---

## 🎨 Design System

### Color Palette
- **Primary**: `#00fff7` (Cyan)
- **Secondary**: `#00ff7f` (Green)
- **Background**: `linear-gradient(135deg, #0f0f23 0%, #1a1a2e 50%, #16213e 100%)`
- **Text**: `#fff` (White)
- **Muted Text**: `#ccc` (Light Gray)
- **Cards**: `rgba(24, 24, 24, 0.9)` with backdrop blur

### Typography
- **Primary Font**: Poppins (Google Fonts)
- **Fallback**: Arial, sans-serif
- **Icon Font**: Font Awesome 6.0+

---

## 🔧 Technical Implementation

### Contact Form Integration
The contact form uses a serverless architecture:

```javascript
// Form submission to AWS API Gateway
const payload = {
  "name": name,
  "email": email,
  "message": message
};

fetch(apiEndpoint, {
  method: 'POST',
  headers: { 'Content-Type': 'application/json' },
  body: JSON.stringify(payload)
});
```

### Performance Optimizations
- **Minimal Dependencies**: Only Font Awesome and Google Fonts
- **Optimized Images**: Compressed profile and background images
- **Efficient CSS**: Individual stylesheets per page for optimal loading
- **Fast Loading**: Pure HTML/CSS/JS with no frameworks
- **Modern Features**: CSS Grid, Flexbox, and backdrop-filter for performance

---

## 🤝 Contributing

Contributions and suggestions are welcome! Please feel free to:

- Report bugs or issues
- Suggest new features or improvements
- Submit pull requests for enhancements
- Provide feedback on design or functionality

### Development Guidelines
- Maintain responsive design principles
- Follow existing code style and structure
- Test across multiple browsers and devices
- Ensure accessibility standards are met

---

## 📬 Contact & Connect

- **📧 Email**: [gustav.kiewiets@hotmail.com](mailto:gustav.kiewiets@hotmail.com)
- **💼 LinkedIn**: [linkedin.com/in/gus88](https://www.linkedin.com/in/gus88)
- **🐙 GitHub**: [github.com/gus-hub-tech](https://github.com/gus-hub-tech)
- **📝 Medium**: [medium.com/@gustav.kiewiets](https://medium.com/@gustav.kiewiets)
- **🌐 Portfolio**: [Live Website](https://main.d3d5cnpn2eqq65.amplifyapp.com)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

**Thank you for exploring my portfolio! 🚀**

