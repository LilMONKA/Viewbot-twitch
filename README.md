# Quick Start Guide

Get up and running with the Advanced Twitch ViewBot in 5 minutes!

## Prerequisites

Before you begin, make sure you have:
- ✅ Python 3.6 or higher installed
- ✅ Google Chrome browser (latest version)
- ✅ Internet connection
- ✅ At least 4GB of RAM

## Installation

### Step 1: Install Dependencies

Open your terminal and run:

```bash
pip install -r requirements.txt
```

This will install:
- selenium (browser automation)
- webdriver-manager (Chrome driver management)
- requests (HTTP library)

### Step 2: Verify Installation

Run the test script to make sure everything works:

```bash
python test_viewbot.py
```

If you see "✅ Test completed successfully", you're ready to go!

## Basic Usage

### Option 1: Interactive Mode (Easiest)

Simply run:

```bash
python run_viewbot.py
```

Then follow the prompts:
1. Enter the Twitch channel URL (e.g., https://www.twitch.tv/shroud)
2. Enter the number of bots (start with 5-10)
3. Enter the duration in minutes (start with 30)
4. Confirm to start

### Option 2: Command Line

For direct execution:

```bash
python twitch_viewbot.py https://www.twitch.tv/CHANNEL_NAME NUMBER_OF_BOTS --duration MINUTES
```

**Example:**
```bash
python twitch_viewbot.py https://www.twitch.tv/shroud 10 --duration 30
```

This sends 10 bots to shroud's channel for 30 minutes.

## Your First Run

Let's do a test run with minimal bots:

```bash
python twitch_viewbot.py https://www.twitch.tv/shroud 5 --duration 15
```

This will:
- Send 5 bot viewers to shroud's channel
- Keep them active for 15 minutes
- Use advanced anti-detection features
- Simulate realistic human behavior

## What to Expect

When you run the viewbot, you'll see:

```
Starting 5 advanced viewer bots for channel: shroud
Viewers will run for 15 minutes
Using mixed viewing methods for better realism...
Bot 1 started (waiting 5.3s before next bot)
Bot 2 started (waiting 3.7s before next bot)
...
All bots are now active and watching...
```

The bots will:
- Start with random delays (2-8 seconds apart)
- Alternate between direct page and embed viewing
- Simulate mouse movements and scrolling
- Maintain sessions with periodic refreshes
- Run for the specified duration

## Stopping Early

To stop the bots before the duration expires:

Press `Ctrl+C` in the terminal

All browser instances will close gracefully.

## Recommended Settings

### For Testing
- **Bots**: 3-5
- **Duration**: 5-10 minutes
- **Purpose**: Verify everything works

### For Light Use
- **Bots**: 5-15
- **Duration**: 30-60 minutes
- **System**: Any modern computer

### For Moderate Use
- **Bots**: 15-30
- **Duration**: 30-90 minutes
- **System**: 8GB+ RAM, quad-core CPU

### For Heavy Use
- **Bots**: 30-50
- **Duration**: 60+ minutes
- **System**: 16GB+ RAM, 6+ core CPU

## Common Issues & Solutions

### Issue: "Chrome driver not found"
**Solution:** Run `pip install --upgrade webdriver-manager`

### Issue: High CPU/RAM usage
**Solution:** Reduce the number of bots or close other applications

### Issue: Bots stop quickly
**Solution:** Increase the duration parameter

### Issue: "Module not found" error
**Solution:** Run `pip install -r requirements.txt` again

## Tips for Best Results

1. **Start Small**: Begin with 5-10 bots to test
2. **Monitor Resources**: Watch CPU and RAM usage
3. **Stable Internet**: Ensure good connection
4. **Close Apps**: Free up system resources
5. **Realistic Duration**: Use 30+ minutes for better effect

## Advanced Usage

For more advanced features and customization, see:
- [README.md](README.md) - Full documentation
- [ADVANCED_FEATURES.md](ADVANCED_FEATURES.md) - Technical details

## Safety Reminders

⚠️ **Important:**
- This tool is for educational purposes only
- Using bots violates Twitch's Terms of Service
- May result in channel suspension or ban
- Use at your own risk

## Next Steps

Once you're comfortable with basic usage:

1. Read [ADVANCED_FEATURES.md](ADVANCED_FEATURES.md) for customization options
2. Experiment with different bot counts and durations
3. Monitor system performance and adjust accordingly
4. Explore the code to understand how it works

## Getting Help

If you encounter issues:

1. Check the [README.md](README.md) troubleshooting section
2. Review [ADVANCED_FEATURES.md](ADVANCED_FEATURES.md) for technical details
3. Verify all prerequisites are met
4. Try running with fewer bots first

## Example Commands

### Test Run (5 bots, 10 minutes)
```bash
python twitch_viewbot.py https://www.twitch.tv/shroud 5 --duration 10
```

### Light Run (10 bots, 30 minutes)
```bash
python twitch_viewbot.py https://www.twitch.tv/ninja 10 --duration 30
```

### Moderate Run (20 bots, 45 minutes)
```bash
python twitch_viewbot.py https://www.twitch.tv/xqc 20 --duration 45
```

### Heavy Run (40 bots, 60 minutes)
```bash
python twitch_viewbot.py https://www.twitch.tv/pokimane 40 --duration 60
```

---

**You're all set!** Start with a small test run and gradually increase as you get comfortable with the tool.

Happy streaming! 🎮📺
