# AWS-Amplify-Portfolio

## 🌐 About This Project

A modern, responsive portfolio website showcasing my journey as a Cloud Computing Professional.This multi-page application highlights my technical skills, certifications, and professional experience in cloud technologies.

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

### Page Structure
- **Landing Page (index.html)**: Hero section with rotating titles, stats, and social links
- **About Page**: Personal background, interests, and interactive cards
- **Qualifications Page**: Timeline of certifications and career milestones
- **Tools & Platforms Page**: Technical skills organized by category
- **Recommendations Page**: Professional endorsements with download links
- **Contact Page**: AWS-integrated contact form with real-time feedback
- **Location Page**: Availability status and work preferences

### Technical Implementation
- **Pure HTML/CSS/JS**: No frameworks, fast loading times
- **Consistent Design**: Glass morphism cards with backdrop blur effects
- **Responsive Grid Layouts**: CSS Grid and Flexbox for all screen sizes
- **Interactive Animations**: Hover effects, transforms, and smooth transitions
- **AWS Integration**: Serverless contact form with Lambda and SES

### User Experience
- **Rotating Job Titles**: 4 roles cycling every 3 seconds on landing page
- **Professional Timeline**: Alternating left/right layout with hover animations
- **Skill Cards**: Organized tools with category-based sections
- **Download Features**: Direct PDF downloads for resume and recommendations
- **Status Indicators**: Live availability status with pulsing animation

---

## Old 📸 Preview [New-below]

https://github.com/user-attachments/assets/036113ef-e119-4c1f-88e8-602a68aeb513

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

### Development Setup
- **No Build Process**: Direct file editing and browser refresh
- **Local Testing**: Use Python HTTP server or Live Server extension
- **AWS Integration**: Contact form requires valid AWS endpoint
- **File Structure**: Each page has consistent styling and navigation
- **Testing**: Responsive design testing across multiple devices

---

## 🏗️ AWS Infrastructure

### Serverless Architecture
```
User Form → API Gateway → Lambda Function → Amazon SES → Email Delivery
     ↓
  Amplify Hosting ← GitHub Repository
     ↓
  S3 Storage (Resume & Recommendations)
```

### AWS Services Used
- **AWS Amplify**: Static web hosting with continuous deployment
- **API Gateway**: RESTful endpoint for contact form submissions
- **AWS Lambda**: Serverless function processing form data
- **Amazon SES**: Email service for contact form delivery
- **S3 Bucket**: File storage for resume and recommendation PDFs

### Deployment Pipeline
1. Code push to GitHub repository
2. Amplify automatically detects changes
3. Builds and deploys static site
4. Updates live website instantly

---

## 📱 Responsive Design

### Breakpoints
- **Desktop**: 1024px and above (full layout)
- **Tablet**: 768px - 1023px (adjusted grids)
- **Mobile**: Below 768px (single column, stacked layout)
- **Small Mobile**: Below 480px (compact spacing)

### Responsive Features
- **Timeline**: Switches from alternating to single-column on mobile
- **Navigation**: Maintains horizontal layout with adjusted spacing
- **Cards**: Grid layouts adapt from multi-column to single-column
- **Typography**: Font sizes scale down appropriately for smaller screens

---

## 🎨 Design System

### Visual Identity
- **Theme**: Dark gradient with glass morphism effects
- **Primary Colors**: Cyan (`#00fff7`) and Green (`#00ff7f`)
- **Background**: Multi-layer gradient (`#0f0f23` → `#1a1a2e` → `#16213e`)
- **Cards**: Semi-transparent with backdrop blur (`rgba(24, 24, 24, 0.9)`)
- **Borders**: Subtle cyan glow effects (`rgba(0, 255, 247, 0.2)`)

### Typography & Icons
- **Font Family**: Poppins (300, 400, 500, 600, 700 weights)
- **Headings**: Gradient text effects with background-clip
- **Icons**: Font Awesome 6.4.2 for consistent iconography
- **Text Colors**: White primary, light gray (`#ccc`) secondary

### Interactive Elements
- **Hover Effects**: Transform scale, translateY, and glow animations
- **Transitions**: 0.3s ease for smooth interactions
- **Button Styles**: Gradient backgrounds with hover transforms
- **Card Animations**: Backdrop blur with border color changes

---

## 🔧 Technical Implementation

### Contact Form Integration
Serverless contact form with AWS services:

```javascript
// Enhanced form submission with loading states
document.getElementById('contactForm').addEventListener('submit', async function(e) {
  e.preventDefault();
  
  const payload = { name, email, message };
  
  try {
    const response = await fetch(apiEndpoint, {
      method: 'POST',
      headers: { 'Content-Type': 'application/json' },
      body: JSON.stringify(payload)
    });
    
    if (response.ok) {
      // Show success message and redirect
    }
  } catch (error) {
    // Handle errors with user feedback
  }
});
```

### JavaScript Features
- **Rotating Titles**: DOM manipulation with setInterval for title cycling
- **Form Validation**: Client-side validation with error handling
- **Loading States**: Button disable/enable with visual feedback
- **Responsive Navigation**: Event listeners for mobile menu interactions

### Architecture & Performance
- **Static Site**: No build process required, direct file serving
- **Minimal Dependencies**: Font Awesome (icons) and Google Fonts (typography)
- **Optimized Assets**: Compressed images and efficient CSS
- **Modern CSS**: Grid layouts, Flexbox, and backdrop-filter effects
- **Cross-browser**: Compatible with all modern browsers
- **Mobile-first**: Responsive breakpoints at 768px and 480px

---

## 🤝 Contributing

Contributions and suggestions are welcome! Please feel free to:

- Suggest new features or improvements
- Submit pull requests for enhancements
- Provide feedback on design or functionality

### Development Guidelines
- **Consistency**: Maintain unified design system across all pages
- **Performance**: Keep dependencies minimal and optimize assets
- **Accessibility**: Include proper ARIA labels and semantic HTML
- **Responsive**: Test on multiple screen sizes and devices
- **Browser Support**: Ensure compatibility with modern browsers
- **Code Quality**: Use semantic HTML and organized CSS structure

---

## 📬 Contact & Connect

- **📧 Email**: [gustav.kiewiets@hotmail.com](mailto:gustav.kiewiets@hotmail.com)
- **💼 LinkedIn**: [linkedin.com/in/gus88](https://www.linkedin.com/in/gus88)
- **🐙 GitHub**: [github.com/gus-hub-tech](https://github.com/gus-hub-tech)
- **📝 Medium**: [medium.com/@gustav.kiewiets](https://medium.com/@gustav.kiewiets)

---

## 🌐 Live Demo
<img width="1343" height="307" alt="image" src="https://github.com/user-attachments/assets/d9a3910c-f83d-4117-a31a-a519b3290a80" />

https://github.com/user-attachments/assets/600bc41e-ad18-482c-a3cb-e1ba189b3dea



---

**Thank you for exploring my portfolio! 🚀**

