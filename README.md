# LA Art & Activism Calendar 2026

A calendar highlighting art exhibitions and events focused on activism, human rights, intersectionality, and immigrant experiences in the Los Angeles area.

## 🎨 Features

- **Black & white minimalist design** with pattern-based category markers
- **Community submissions** via GitHub Issues
- **Easy to maintain** with a simple JSON file
- **Mobile responsive**
- **Free to host** on GitHub Pages

## 🚀 Setup Instructions

### 1. Fork or Clone This Repository

```bash
git clone https://github.com/melanni3h/la-artivist.git
cd la-artivist
```

### 2. Update Configuration

Edit `index.html` and update these variables (around line 454):

```javascript
const GITHUB_USERNAME = 'melanni3h';  // Your GitHub username
const REPO_NAME = 'la-artivist';  // Your repository name
```

Also update the GitHub link in the sidebar (around line 407):

```html
<a href="https://github.com/melanni3h/la-artivist" target="_blank" class="btn-primary">VIEW ON GITHUB</a>
```

### 3. Enable GitHub Pages

1. Go to your repository Settings
2. Navigate to "Pages" in the left sidebar
3. Under "Source", select `main` branch
4. Click Savela-artivist
5. Your site will be live at `https://melanni3h.github.io//`

### 4. Set Up Issue Labels (Optional but Recommended)

Create a label called `event-submission` for organizing event submissions:

1. Go to Issues → Labels
2. Click "New label"
3. Name: `event-submission`
4. Color: Pick any color
5. Click "Create label"

## 📝 How to Add Events

### Method 1: Edit JSON Directly (Recommended for Maintainers)

Edit `events.json` and add your event:

```json
{
  "id": 15,
  "title": "Your Event Title",
  "startDate": "2026-03-15",
  "endDate": "2026-03-20",
  "venue": "Event Venue Name",
  "category": "chicano",
  "description": "Event description highlighting activism/human rights themes.",
  "eventUrl": "https://example.com/event",
  "mapQuery": "Venue Name Los Angeles",
  "tags": ["FREE", "MULTI-DAY"]
}
```

**Categories:**
- `immigration` - Immigration & Border Justice
- `chicano` - Chicano/Latinx Activism
- `aapi` - AAPI Rights & History
- `environmental` - Environmental Justice
- `social-justice` - Social Justice & Human Rights
- `intersectional` - Intersectional/Multiple Themes

**Commit and push:**
```bash
git add events.json
git commit -m "Add [Event Name]"
git push
```

Your changes will appear live in a few minutes!

### Method 2: Via GitHub Issues (For Community Members)

1. Click "SUBMIT EVENT" button on the calendar
2. Fill out the pre-formatted GitHub issue template
3. Submit the issue
4. A maintainer will review and add to `events.json`

## 🛠️ Maintaining the Calendar

### Reviewing Submissions

1. Check the [Issues](../../issues?q=is%3Aissue+is%3Aopen+label%3Aevent-submission) tab
2. Review event submissions
3. If approved:
   - Copy the event details
   - Add to `events.json`
   - Commit and push
   - Close the issue with a comment: "Added! Thanks for contributing."
4. If rejected:
   - Close the issue with a polite explanation

### Removing Past Events

Periodically clean up old events:

```bash
# Edit events.json to remove events that have ended
git add events.json
git commit -m "Remove past events"
git push
```

### Updating Event Information

Simply edit the event in `events.json`, commit, and push.

## 📂 File Structure

```
la-artivist/
├── index.html          # Main calendar page
├── events.json         # All events data
└── README.md           # This file
```

## 🎨 Customization

### Design
- All styles are in `<style>` tag in `index.html`
- Uses IBM Plex Mono and Space Mono fonts
- Pattern-based markers for accessibility

### Adding New Categories

1. Add category to `events.json`
2. Add filter button in HTML
3. Add legend item with pattern
4. Add pattern CSS for the marker

## 🤝 Contributing

Contributions are welcome! Please:
1. Submit events via GitHub Issues
2. Report bugs via GitHub Issues
3. Suggest features via GitHub Issues

## 📄 License

Free to use and modify. Attribution appreciated but not required.

## 📧 Contact

For questions or suggestions, [open an issue](../../issues/new).

---

**Last Updated:** January 2026  
**Maintained by:** [Your Name/Organization]
