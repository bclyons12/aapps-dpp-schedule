# AAPPS-DPP 2025 Conference Schedule

Interactive web-based conference schedule for the Asia-Pacific Plasma Science (AAPPS) Division of Plasma Physics (DPP) 2025 conference.

## 🌐 Live Schedule

**Access the schedule at:** https://bclyons12.github.io/aapps-dpp-schedule/

## ✨ Features

- **📅 Multi-day navigation** - Browse schedule across all conference days (Sep 21-26, 2025)
- **⏰ Real-time updates** - Talks are automatically grayed out when started, hidden when past (30-min grace period)
- **✅ Personal tracking** - Check off talks you want to attend
- **🔍 Smart filtering** - Show only checked talks, hide past talks
- **💾 Persistent state** - Your selections and preferences are saved locally
- **⏱️ Duration display** - See talk duration in minutes
- **🔗 Shareable selections** - URL updates with your checked talks for easy sharing
- **📱 Mobile responsive** - Works perfectly on phones, tablets, and desktop

## 🚀 Usage

### Navigation
- Click day tabs to switch between conference days
- Current day is highlighted with your local time display

### Talk Management  
- **Check talks** you plan to attend using the checkboxes
- **View details** including speaker, affiliation, room, and duration
- **Track time** with automatic graying of started talks

### Filtering Options
- **"Show only checked talks"** - Focus on your selected sessions
- **"Hide past talks"** - Clean view of upcoming sessions (30-minute grace period)
- **Time-based display** - Past talks are grayed out automatically

### Sharing & Persistence
- **Bookmarks work** - URL includes your selections for easy sharing
- **Auto-save** - Your preferences persist across browser sessions
- **Device-specific** - Each device maintains its own selections

## 🛠️ Technical Details

### Architecture
- **Single HTML file** with embedded CSS/JavaScript
- **CSV data source** - Easy to update conference information
- **Local storage** - Base64-encoded bitmap for efficient selection storage
- **No server required** - Runs entirely in the browser

### Data Format
CSV files contain: `Session,Time,Duration,Room,Speaker,Affiliation,Title`

### Cache Management
- **Fresh data** - CSV files are fetched fresh on each load
- **No caching** - Ensures users always see latest schedule updates

## 📂 File Structure

```
aapps-dpp-schedule/
├── index.html          # Redirect to main schedule
├── agenda.html         # Main conference schedule application  
├── csv/                # Conference data files
│   ├── Agenda_2025-09-21.csv
│   ├── Agenda_2025-09-22.csv
│   ├── Agenda_2025-09-23.csv
│   ├── Agenda_2025-09-24.csv
│   ├── Agenda_2025-09-25.csv
│   └── Agenda_2025-09-26.csv
├── server.py           # Local development server (not used in production)
└── README.md           # This file
```

## 🔧 Local Development

For local testing and development:

```bash
# Clone the repository
git clone https://github.com/bclyons12/aapps-dpp-schedule.git
cd aapps-dpp-schedule

# Start local server
python3 server.py

# Open browser to http://localhost:8000
```

## 📊 Conference Data

This schedule contains **729 talks** across **6 days** of the AAPPS-DPP 2025 conference.

Conference dates: **September 21-26, 2025**  
Time zone: **Japan Standard Time (JST)**

## 🤝 Contributing

To update the schedule:

1. Edit the CSV files in the `csv/` directory
2. Commit and push changes to GitHub
3. GitHub Pages will automatically deploy updates

CSV format: `Session,Time,Duration,Room,Speaker,Affiliation,Title`

## 📱 Browser Compatibility

- ✅ Chrome/Chromium (recommended)
- ✅ Firefox  
- ✅ Safari
- ✅ Edge
- ✅ Mobile browsers

## 🔒 Privacy

- **No data collection** - All data stays on your device
- **Local storage only** - Selections stored in browser localStorage
- **No tracking** - No analytics or external services
- **Offline capable** - Works without internet after initial load

---

*Generated for AAPPS-DPP 2025 Conference*