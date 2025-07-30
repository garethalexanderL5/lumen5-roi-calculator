# Lumen5 ROI Calculator

A comprehensive ROI calculator that helps businesses understand the cost and time savings from using Lumen5's AI-powered video creation platform compared to traditional post-production workflows.

## Features

- **Real-time ROI Calculations**: Calculate savings based on video count, time frame, and production costs
- **Flexible Cost Models**: Support for both direct cost per video and hourly rate calculations
- **Comprehensive Metrics**: Track time savings, cost savings, productivity gains, and break-even analysis
- **Interactive Visualizations**: Charts showing 12-month savings projections
- **Detailed Breakdowns**: Modal popups explaining each calculation with examples
- **Export Functionality**: Generate and export detailed ROI reports

## Live Demo

[View the live calculator](https://your-vercel-url.vercel.app)

## Screenshots

![ROI Calculator Interface](./screenshots/calculator-interface.png)
*Main calculator interface with input form and results dashboard*

## Technology Stack

- **Frontend**: Vanilla HTML5, CSS3, JavaScript (ES6+)
- **Charts**: Chart.js 3.9.1
- **Styling**: Custom CSS with modern gradients and responsive design
- **Deployment**: Vercel

## Getting Started

### Prerequisites

No build tools or dependencies required! This is a static HTML application.

### Local Development

1. Clone the repository:
```bash
git clone https://github.com/yourusername/lumen5-roi-calculator.git
cd lumen5-roi-calculator
```

2. Open `index.html` in your browser or serve it locally:
```bash
# Using Python
python -m http.server 8000

# Using Node.js (if you have http-server installed)
npx http-server

# Or simply open index.html in your browser
```

3. Navigate to `http://localhost:8000` (if using a local server)

### Deployment

#### Vercel (Recommended)

1. Push your code to GitHub
2. Connect your GitHub repository to Vercel
3. Deploy automatically - no build configuration needed!

#### Alternative Deployments

This static site can be deployed to any static hosting service:
- Netlify
- GitHub Pages  
- AWS S3 + CloudFront
- Firebase Hosting

## Usage

1. **Enter Video Details**: Specify the number of videos and time period
2. **Configure Costs**: Choose between direct cost per video or hourly rate calculations
3. **Set Time Parameters**: Input traditional vs. Lumen5 production times
4. **View Results**: See comprehensive ROI analysis with interactive charts
5. **Export Report**: Generate detailed reports for stakeholders

## Calculator Methodology

### Cost Savings Calculation
```
Traditional Cost = Videos × (Direct Cost OR Hourly Rate × Hours)
Lumen5 Cost = (Annual Enterprise Cost ÷ 12) × Months
Cost Savings = Traditional Cost - Lumen5 Cost
```

### Time Value Calculation
```
Coordination Time Saved = (Traditional Time × 0.6) - (Lumen5 Time × 0.67)
Time Value = Coordination Time Saved × Coordination Wage
```

### ROI Calculation
```
Total Value = Cost Savings + Time Value Saved
ROI = (Total Value ÷ Lumen5 Cost) × 100
```

## Customization

### Modifying Default Values

Edit the default values in the HTML input elements or JavaScript initialization:

```javascript
// In the DOMContentLoaded event listener
value="20"     // Default video count
value="1"      // Default time frame
value="12000"  // Default enterprise cost
```

### Adding New Metrics

1. Add new input fields in the HTML
2. Update the `calculate()` function to include new calculations  
3. Add corresponding result displays and modal explanations

### Styling Changes

The CSS uses CSS custom properties for easy theming. Key variables:
- Primary colors: `#4f46e5`, `#7c3aed`
- Success color: `#10b981`
- Error color: `#ef4444`

## File Structure

```
lumen5-roi-calculator/
├── index.html          # Main application file
├── README.md           # This file
├── screenshots/        # Application screenshots
├── .gitignore         # Git ignore rules
└── vercel.json        # Vercel configuration (optional)
```

## Browser Support

- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Support

For questions or support, please open an issue on GitHub or contact [your-email@company.com].

## Roadmap

- [ ] Add CSV export functionality
- [ ] Implement multiple currency support
- [ ] Add team collaboration features
- [ ] Mobile app version
- [ ] Integration with CRM systems

---

**Note**: This calculator is designed for Lumen5 Enterprise customers. For other plan tiers or custom configurations, please contact Lumen5 sales.