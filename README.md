# Quarterly Objectives Dashboard

A professional web-based dashboard for tracking and managing quarterly objectives across financial years. Built with clean HTML, CSS, and JavaScript for easy deployment and maintenance.

## 🎯 Features

- **Interactive Dashboard**: Overview of all quarterly objectives with progress tracking
- **Priority Matrix**: Detailed objective management with filtering and search capabilities
- **Professional Design**: Corporate-style interface inspired by modern financial services
- **Responsive Layout**: Works seamlessly on desktop, tablet, and mobile devices
- **Easy Configuration**: Simple JavaScript-based configuration for adding new quarters
- **Financial Year Support**: Designed for April-March financial year cycles

## 📁 File Structure

```
quarterly-objectives/
├── index.html              # Main dashboard page
├── 2025-26-q2.html        # Q2 objectives (current quarter)
├── 2025-26-q3.html        # Q3 objectives (future)
├── 2025-26-q4.html        # Q4 objectives (future)
├── 2026-27-q1.html        # Q1 objectives (future)
├── README.md               # Documentation
└── assets/                 # (Optional) For any additional resources
```

## 🚀 Quick Start

### 1. Download Files
Save the dashboard files to your desired location:
- `index.html` - Main dashboard
- `2025-26-q2.html` - Current quarter objectives
- `README.md` - This documentation

### 2. Configure Current Quarter
Edit the `quarters` array in `index.html` to match your current objectives:

```javascript
const quarters = [
    {
        id: '2025-26-q2',
        title: 'Q2 2025-26',
        period: 'July - September 2025',
        status: 'current',
        fileName: '2025-26-q2.html',
        stats: {
            total: 28,
            completed: 0,
            inProgress: 28
        },
        priorities: {
            high: 17,
            medium: 6,
            low: 5
        }
    }
    // ... add more quarters
];
```

### 3. Deploy
Choose your preferred hosting method:

#### GitHub Pages (Recommended)
1. Create a new GitHub repository
2. Upload all files to the repository
3. Go to Settings → Pages
4. Select "Deploy from a branch" and choose `main`
5. Your dashboard will be available at `https://yourusername.github.io/repository-name`

#### Other Options
- **Netlify**: Drag and drop files for instant deployment
- **Vercel**: Upload files for automatic deployment
- **Internal Server**: Copy files to your company's web server

## 📊 Managing Objectives

### Priority Levels
- **High**: Critical objectives that must be completed this quarter
- **Medium**: Important objectives that should be completed if possible
- **Low**: Nice-to-have objectives that can be deferred if needed

### Categories
- **Business Delivery**: Core business functionality and features
- **Quality & Stability**: Testing, QA, and system reliability
- **Team Development**: Training, mentoring, and skill building
- **Automation**: Process improvements and automated workflows
- **Innovation**: New technologies and experimental features
- **Experimental**: Research projects and proof-of-concepts

### Adding New Objectives
Edit the `objectives` array in your quarter file:

```javascript
const objectives = [
    {
        priority: 'high',
        category: 'delivery',
        objective: 'Description of the objective',
        assignees: ['AB', 'MS', 'LR'],
        notes: 'Additional context or notes'
    }
    // ... add more objectives
];
```

## 🗓️ Financial Year Structure

The dashboard is designed for companies with April-March financial years:

- **Q1**: April - June
- **Q2**: July - September  
- **Q3**: October - December
- **Q4**: January - March

### File Naming Convention
- Format: `YYYY-YY-qN.html`
- Example: `2025-26-q2.html` for Q2 of financial year 2025-26

## 🔧 Customization

### Adding New Quarters

1. **Create New File**: Copy an existing quarter file (e.g., `2025-26-q2.html`) and rename it
2. **Update Objectives**: Edit the `objectives` array with new quarter's objectives
3. **Update Dashboard**: Add the new quarter to the `quarters` array in `index.html`
4. **Deploy**: Upload the new file to your hosting platform

### Updating Progress

To track progress throughout the quarter:

1. **Mark Completed**: Update the `completed` count in the quarter configuration
2. **Update Status**: Change objective status or add completion notes
3. **Refresh Stats**: The dashboard will automatically calculate completion percentages

### Team Members

Update the assignee filter options in both dashboard and objectives files:

```javascript
// In the assignee filter dropdown
<option value="AB">AB</option>
<option value="MS">MS</option>
// ... add new team members
```

## 🎨 Design System

The dashboard uses a professional color scheme and typography:

- **Primary Blue**: `#1a365d` - Headers and key elements
- **Secondary Blue**: `#2d5a87` - Accents and hover states
- **Typography**: Segoe UI for clean, modern appearance
- **Spacing**: Consistent 8px grid system
- **Shadows**: Subtle shadows for depth and hierarchy

## 📱 Browser Support

- **Chrome**: Full support
- **Firefox**: Full support
- **Safari**: Full support
- **Edge**: Full support
- **Mobile**: Responsive design works on all modern mobile browsers

## 🔒 Security & Privacy

- **No External Dependencies**: All code runs locally, no external API calls
- **No Data Storage**: No cookies or local storage used
- **Static Files**: Pure HTML/CSS/JS - no server-side processing required

## 🛠️ Troubleshooting

### Common Issues

**Dashboard not loading properly**
- Check that all file paths are correct
- Ensure JavaScript is enabled in browser
- Verify file names match the configuration

**Objectives not displaying**
- Check the `objectives` array syntax
- Verify all required fields are present
- Look for JavaScript console errors

**Styling issues**
- Clear browser cache
- Check for missing CSS files
- Verify responsive viewport meta tag

### Getting Help

If you encounter issues:

1. Check the browser console for error messages
2. Verify file names and paths match configuration
3. Ensure all required fields are present in data arrays
4. Test with a simple configuration first

## 📈 Best Practices

### Objective Management
- **Be Specific**: Write clear, actionable objectives
- **Set Realistic Goals**: Don't overcommit team members
- **Regular Updates**: Review and update progress weekly
- **Priority Balance**: Aim for 60% High, 30% Medium, 10% Low priorities

### Team Allocation
- **Balanced Workload**: Avoid overloading specific team members
- **Skill Matching**: Assign objectives based on expertise
- **Dependencies**: Consider objective dependencies when planning
- **Backup Plans**: Have contingency plans for high-priority objectives

### Documentation
- **Clear Notes**: Add context and requirements to objectives
- **Progress Tracking**: Update completion status regularly
- **Lessons Learned**: Document what worked and what didn't
- **Future Planning**: Use insights for next quarter planning

## 🔄 Version History

- **v1.0**: Initial release with basic dashboard and objectives tracking
- **v1.1**: Added Downing-inspired professional design
- **v1.2**: Improved responsive design and mobile support
- **v1.3**: Enhanced filtering and search capabilities

## 📞 Support

For questions or issues with the dashboard:
- Check this README for common solutions
- Review the code comments for technical details
- Test with simplified configurations to isolate issues

---

*This dashboard is designed for internal use and can be customized to fit your team's specific needs and branding requirements.*
