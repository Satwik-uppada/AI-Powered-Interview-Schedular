# User Manual: AI Interview Scheduler 📅

This guide will help you set up and use the AI Interview Scheduler as a recruiter.

## Initial Setup Requirements 🛠️

Before you can start using the scheduler, you need to:

1. Have a Google Calendar account (corporate or personal)
2. Grant necessary calendar permissions
3. Add the service account to your calendar settings

## Calendar Permission Setup 🔐

### Step 1: Add Service Account to Your Calendar

1. Copy the service account email: `calendar-scheduler-bot@scheduling-bot-453903.iam.gserviceaccount.com`

2. Open [Google Calendar](https://calendar.google.com/)

3. Find your calendar settings:
   - Click on the gear icon (⚙️) in the top right
   - Select "Settings & Sharing" from the dropdown menu

4. Share your calendar with the service account:
   - In the left sidebar, click on your calendar name under "Settings for my calendars"
   - Scroll to "Share with specific people or groups"
   - Click "+ Add people"
   - Paste the service account email
   - Set permission to "Make changes and manage sharing"
   - Click "Send"

### Step 2: Calendar Visibility Settings

1. Still in calendar settings, ensure:
   - "Make available to public" is OFF for privacy
   - "See all event details" is selected under "Access permissions"

## Using the Scheduler 📋

### Before Scheduling

1. Inform candidates that:
   - They need to share their Google Calendar availability
   - They should mark personal appointments as "private"
   - They need to share their calendar with the service account email

2. Collect from candidates:
   - Their preferred email address
   - Confirmation that they've shared their calendar

### Scheduling Process

1. Launch the application:
   - Open your browser
   - Go to the provided application URL or localhost:8501

2. Follow the chat interface prompts:

   a. Enter your email (recruiter email)
   ```
   Example: recruiter@company.com
   ```

   b. Enter candidate's email
   ```
   Example: candidate@email.com
   ```

   c. Specify interview duration
   ```
   Example: "1 hour" or "45 minutes" or "1 hr 30 min"
   ```

   d. Enter preferred date
   ```
   Example: "next Monday" or "March 25th" or "2025-04-01"
   ```

3. Select time slot:
   - View available time slots
   - Choose a slot by entering its number
   - Confirm the selection

## Troubleshooting Guide 🔧

### Common Issues and Solutions

1. **"Cannot access calendar" error**
   - Verify service account email is added to calendar
   - Check permission level (should be "Make changes and manage sharing")
   - Try removing and re-adding the service account

2. **No available slots shown**
   - Confirm candidate has shared their calendar
   - Check if the selected date is a holiday/weekend
   - Try a different date

3. **Calendar sync delays**
   - Allow up to 5 minutes for calendar changes to reflect
   - Refresh the application

### Best Practices 💡

1. **Before Each Interview:**
   - Verify calendar sharing is set up properly
   - Ensure both parties have granted permissions
   - Check your calendar is up to date

2. **Privacy Considerations:**
   - Mark sensitive meetings as "private"
   - Only share required calendar details
   - Inform candidates about data usage

3. **Schedule Management:**
   - Keep your calendar updated
   - Remove calendar access after scheduling if desired
   - Double-check time zones (system uses IST)

## Data Privacy Notice 🔒

The system:
- Only accesses free/busy information
- Does not store personal calendar data
- Uses secure service account authentication
- Respects calendar privacy settings

## Support and Help 💁‍♂️

If you encounter issues:
1. Check this manual's troubleshooting section
2. Verify all setup steps are completed
3. Contact your system administrator
4. Raise an issue in the project repository

## Quick Reference Card 📝

### Essential Emails to Save:
```
Service Account: calendar-scheduler-bot@scheduling-bot-453903.iam.gserviceaccount.com
```

### Key Steps Summary:
1. Share calendar with service account
2. Verify candidate has shared their calendar
3. Use the application to find common slots
4. Confirm and schedule

### Remember:
- Keep calendars updated
- Check permissions before scheduling
- Use clear meeting titles
- Verify time zones
