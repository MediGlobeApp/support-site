# MediGlobe Troubleshooting Guide

Having issues with MediGlobe? This guide will help you resolve common problems quickly.

---

## 🔍 Search Issues

### Search Returns No Results

**Symptoms:**
- Searching for a medication returns empty results
- "No medications found" message appears

**Solutions:**

1. **Try the generic name**
   - Instead of "Advil" → try "ibuprofen"
   - Instead of "Tylenol" → try "acetaminophen" or "paracetamol"
   - Instead of "Zantac" → try "ranitidine"

2. **Check your spelling**
   - Common medications may have different spellings
   - Try alternative spellings (e.g., "paracetamol" vs "acetaminophen")
   - Use the suggestions that appear as you type

3. **Verify internet connection**
   - Check if you're connected to Wi-Fi or cellular data
   - Try opening Safari to test connectivity
   - Some medications require internet access for first search

4. **Check country selection**
   - Some medications are only available in certain countries
   - Try selecting a different country (e.g., United States)
   - Use "All Countries" if available

5. **Request the medication**
   - The medication might not be in our database yet
   - Email us at [mediglobeapp@gmail.com](mailto:mediglobeapp@gmail.com)
   - We prioritize user requests

**Still not working?**
- Clear the app cache (see below)
- Restart the app
- Update to the latest version

---

### Search is Very Slow

**Symptoms:**
- Search takes longer than 10 seconds
- App appears to hang during search
- Loading indicator spins indefinitely

**Solutions:**

1. **Check internet speed**
   - Test your connection in Safari
   - Switch between Wi-Fi and cellular data
   - Move to an area with better signal

2. **API rate limiting**
   - If you've searched many times rapidly, wait 1-2 minutes
   - The API has rate limits to prevent abuse
   - Use favorites to avoid re-searching

3. **Clear search cache**
   - Go to app Settings
   - Tap "Clear Search History"
   - Restart the app

4. **Use offline mode**
   - Search for medications you've previously found
   - Use the local database (150+ medications)
   - Save favorites before traveling

5. **Update the app**
   - Check App Store for updates
   - New versions may have performance improvements

**Technical details:**
- Network timeout is set to 30 seconds
- After timeout, app falls back to local database
- Rate limit: ~20 searches per minute

---

### Suggestions Not Appearing

**Symptoms:**
- No suggestions appear while typing
- Dropdown is empty
- Have to type full medication name

**Solutions:**

1. **Type at least 2 characters**
   - Suggestions appear after 2+ characters
   - Try typing more of the medication name

2. **Check internet connection**
   - Suggestions require internet for new medications
   - Previously searched medications work offline

3. **Restart the app**
   - Close MediGlobe completely
   - Swipe up from home screen (or double-click home button)
   - Swipe up on MediGlobe to close
   - Reopen the app

4. **Clear keyboard cache**
   - iOS Settings → General → Keyboard
   - Tap "Reset Keyboard Dictionary"
   - Note: This affects all apps, not just MediGlobe

---

## 📸 Camera Scanner Issues

### Camera Won't Open

**Symptoms:**
- Tapping camera button does nothing
- Black screen appears
- Permission denied message

**Solutions:**

1. **Grant camera permission**
   - Go to iOS Settings → MediGlobe
   - Tap "Camera"
   - Select "Allow"
   - Return to app and try again

2. **Check camera availability**
   - Try opening the iOS Camera app
   - If iOS Camera doesn't work, restart device
   - Clean camera lens with soft cloth

3. **Update iOS**
   - Go to Settings → General → Software Update
   - Install any available updates
   - Camera permissions sometimes require updates

4. **Reinstall the app**
   - Delete MediGlobe
   - Restart your device
   - Reinstall from App Store
   - Grant camera permission when prompted

---

### Camera Can't Read Text

**Symptoms:**
- Camera opens but doesn't recognize text
- OCR fails to extract medication name
- Wrong text is extracted

**Solutions:**

1. **Improve lighting**
   - Use in well-lit area
   - Avoid shadows on the label
   - Use flash if needed
   - Natural daylight works best

2. **Hold steady and close**
   - Hold device 4-6 inches from label
   - Keep camera parallel to text
   - Hold steady for 2-3 seconds
   - Avoid motion blur

3. **Clean and clear label**
   - Wipe label with dry cloth
   - Remove plastic wrapping if present
   - Flatten curved labels if possible
   - Avoid glossy reflections

4. **Text quality issues**
   - Very small text may not scan well
   - Faded or damaged labels are harder to read
   - Handwritten text won't work
   - Non-English characters may not scan correctly

5. **Manual entry fallback**
   - If scanner fails, tap "Cancel"
   - Type the medication name manually
   - Use the regular search feature

**Supported text:**
- Latin alphabet (English characters)
- Printed text (not handwritten)
- Minimum text height: 5mm
- High contrast (dark text on light background)

---

## 📍 Location Issues

### Location Not Detecting Country

**Symptoms:**
- "Unable to detect location" message
- Wrong country is detected
- Location button doesn't work

**Solutions:**

1. **Grant location permission**
   - Go to iOS Settings → MediGlobe
   - Tap "Location"
   - Select "While Using the App"
   - Return to app and try again

2. **Enable Location Services**
   - Go to Settings → Privacy & Security → Location Services
   - Toggle on "Location Services" at top
   - Scroll to MediGlobe and enable

3. **Check GPS signal**
   - Go outdoors if you're inside a building
   - Move away from metal structures
   - Wait 30 seconds for GPS to acquire signal
   - Try again

4. **Verify you're in a supported country**
   - MediGlobe supports 50+ countries
   - Some regions may not be recognized
   - Manually select your country if auto-detect fails

5. **Reset location settings**
   - iOS Settings → General → Transfer or Reset iPhone
   - Tap "Reset"
   - Choose "Reset Location & Privacy"
   - Reopen MediGlobe and grant permission

**Manual selection:**
- You can always manually select your country
- Tap the country dropdown
- Scroll or search for your country
- Location detection is optional

---

### Wrong Location Detected

**Symptoms:**
- App thinks you're in a different country
- GPS shows incorrect location
- Country automatically changes to wrong one

**Solutions:**

1. **Wait for GPS accuracy**
   - Initial GPS fix can be inaccurate
   - Wait 30-60 seconds
   - Check if location improves

2. **Disable VPN**
   - VPNs can make you appear in different countries
   - Disable VPN temporarily
   - Try location detection again

3. **Use Wi-Fi**
   - Wi-Fi improves location accuracy
   - Connect to Wi-Fi network
   - Try location detection again

4. **Manual override**
   - Always verify auto-detected country
   - Manually select correct country from dropdown
   - Auto-detection is a convenience, not required

---

## 💊 Drug Interactions Issues

### Interactions Not Showing

**Symptoms:**
- No interactions shown for medications known to interact
- "No interactions found" message
- Interaction checker seems broken

**Solutions:**

1. **Add multiple medications**
   - Interactions only show when 2+ medications are added
   - Tap "Add Medication" to add more
   - Minimum 2 medications required

2. **Use generic names**
   - Interactions database uses generic names
   - "Ibuprofen" and "Acetaminophen" (not "Advil" and "Tylenol")
   - Try searching by active ingredient

3. **Check internet connection**
   - Interactions require internet access
   - Previously checked combinations are cached
   - Reconnect and try again

4. **Understand limitations**
   - Not all interactions are in the database
   - Rare interactions may not be included
   - Food interactions not included
   - Herbal supplement interactions limited

**⚠️ IMPORTANT:** Always consult your doctor or pharmacist. The interactions checker is informational only and may not include all interactions.

---

## ⭐ Favorites Issues

### Can't Add to Favorites

**Symptoms:**
- Star button doesn't work
- Medication not appearing in favorites
- Favorites list is empty

**Solutions:**

1. **Tap the star icon**
   - Look for the star icon on medication card
   - Tap once to add (star fills)
   - Tap again to remove (star empties)

2. **Check if already added**
   - Go to Favorites tab
   - Medication might already be there
   - Search within favorites if list is long

3. **Storage space**
   - Ensure device has available storage
   - Go to Settings → General → iPhone Storage
   - Free up space if needed
   - Try adding to favorites again

4. **App permissions**
   - Check Settings → MediGlobe
   - Ensure app has storage permissions
   - Restart app after changing permissions

---

### Favorites Disappeared

**Symptoms:**
- Previously saved favorites are gone
- Favorites list is empty
- Lost all saved medications

**Solutions:**

1. **Check if logged out/reset**
   - Did you delete and reinstall the app?
   - Data is stored locally and deleted with app
   - Cannot be recovered if app was deleted

2. **Update app**
   - Old versions may have sync issues
   - Update to latest version from App Store
   - Check if favorites reappear

3. **iCloud backup (doesn't apply)**
   - MediGlobe doesn't use iCloud
   - Favorites are local only
   - Cannot restore from backup

**Prevention:**
- Screenshot your favorites list periodically
- Keep a note of your medications
- Export list (coming in future update)

---

## 🔄 App Performance Issues

### App Crashes on Launch

**Symptoms:**
- App closes immediately after opening
- Black screen then returns to home screen
- Can't get past loading screen

**Solutions:**

1. **Force close and reopen**
   - Swipe up from bottom (or double-click home)
   - Find MediGlobe
   - Swipe up to close completely
   - Wait 10 seconds
   - Reopen app

2. **Restart device**
   - Press and hold power button
   - Slide to power off
   - Wait 30 seconds
   - Power back on
   - Try app again

3. **Update app**
   - Open App Store
   - Go to Updates tab
   - Check for MediGlobe update
   - Install if available

4. **Update iOS**
   - Settings → General → Software Update
   - Install any available updates
   - Restart device
   - Try app again

5. **Reinstall app**
   - Press and hold MediGlobe icon
   - Tap "Remove App" → "Delete App"
   - Restart device
   - Reinstall from App Store
   - Note: This deletes all local data (favorites, history)

---

### App Freezes or Hangs

**Symptoms:**
- App stops responding to taps
- Screen is frozen
- Can't navigate or close sheets

**Solutions:**

1. **Wait 30 seconds**
   - May be loading data
   - Network timeout is 30 seconds
   - App should recover automatically

2. **Force close app**
   - See "App Crashes on Launch" above
   - Force close and reopen

3. **Clear cache**
   - Open MediGlobe (if possible)
   - Go to Settings
   - Tap "Clear Search History"
   - Restart app

4. **Check available memory**
   - Close other apps running in background
   - Restart device to free memory
   - Delete unused apps if storage is low

---

### Slow Performance

**Symptoms:**
- App is laggy or sluggish
- Scrolling is choppy
- Animations are slow

**Solutions:**

1. **Close background apps**
   - Swipe up from bottom (or double-click home)
   - Swipe up on all apps to close
   - Reopen MediGlobe

2. **Restart device**
   - Full device restart often helps
   - Press and hold power button
   - Slide to power off, wait, power on

3. **Free up storage**
   - Settings → General → iPhone Storage
   - Need at least 1GB free
   - Delete unused apps, photos, etc.

4. **Disable animations** (iOS setting)
   - Settings → Accessibility → Motion
   - Toggle on "Reduce Motion"
   - Helps on older devices

5. **Update everything**
   - Update MediGlobe (App Store)
   - Update iOS (Settings → General → Software Update)

---

## 📱 Device-Specific Issues

### Older iPhone Issues

**Devices:** iPhone 8, iPhone X, iPhone XR, etc.

**Common issues:**
- Slower search performance
- Camera scanner slower
- Occasional freezing

**Solutions:**
- Close all background apps
- Use offline mode when possible
- Update to latest iOS compatible with your device
- Free up storage space
- Consider upgrading device if issues persist

---

### iPad-Specific Issues

**Symptoms:**
- Layout looks stretched or odd
- Buttons are in wrong places
- Text is too large or small

**Solutions:**
- MediGlobe is optimized for iPhone but works on iPad
- Rotate to portrait mode for best experience
- Use Split View or Slide Over if preferred
- Some UI elements may appear larger on iPad (normal)

---

## 🌐 Network & Connectivity Issues

### "No Internet Connection" Error

**Symptoms:**
- Error message about no internet
- Can't search new medications
- Only cached results appear

**Solutions:**

1. **Check internet connection**
   - Open Safari and visit a website
   - Toggle Airplane Mode off
   - Check Wi-Fi or cellular data is on

2. **Switch networks**
   - Switch from Wi-Fi to cellular (or vice versa)
   - Disconnect and reconnect to Wi-Fi
   - Forget and rejoin Wi-Fi network

3. **Check data restrictions**
   - Settings → Cellular
   - Scroll to MediGlobe
   - Ensure toggle is ON
   - Check "Low Data Mode" is OFF

4. **Use offline mode**
   - Search previously viewed medications
   - Use local database (150+ medications)
   - Check favorites

---

### "Rate Limit Exceeded" Error

**Symptoms:**
- Error saying "too many requests"
- "Please wait a moment and try again"
- Search temporarily blocked

**Solutions:**

1. **Wait 1-2 minutes**
   - APIs have rate limits
   - Limit: ~20 searches per minute
   - Brief wait resolves this

2. **Use cache**
   - Search previously searched medications
   - They load from cache (no API call)

3. **Use local database**
   - Common medications work without API
   - Offline mode available

4. **Save to favorites**
   - Favorite medications you search often
   - Avoid repeated searches

**This is normal if:**
- You're testing the app
- You searched many times rapidly
- Multiple users on same network

---

### "Server Error" Message

**Symptoms:**
- "Unable to connect to server"
- "Request failed"
- "Server returned an error"

**Solutions:**

1. **Check if APIs are down**
   - RxNorm: https://rxnav.nlm.nih.gov/
   - OpenFDA: https://open.fda.gov/
   - Visit websites to check status

2. **Wait and retry**
   - Temporary server issues
   - Usually resolve within minutes
   - Try again in 5-10 minutes

3. **Use offline mode**
   - Falls back to local database automatically
   - Should work even if servers are down

4. **Check your internet**
   - Some "server errors" are actually network issues
   - See "No Internet Connection" section above

---

## 🔧 General Troubleshooting Steps

### The Universal Fix (Try This First!)

1. **Force close the app**
   - Swipe up from bottom (or double-click home)
   - Swipe up on MediGlobe
   - Wait 10 seconds

2. **Restart your device**
   - Press and hold power button
   - Slide to power off
   - Wait 30 seconds
   - Power back on

3. **Update the app**
   - Open App Store
   - Tap your profile icon (top right)
   - Scroll to find MediGlobe
   - Tap "Update" if available

4. **Update iOS**
   - Settings → General → Software Update
   - Install any available updates

5. **Reinstall the app** (last resort)
   - Delete MediGlobe
   - Restart device
   - Reinstall from App Store
   - ⚠️ Warning: This deletes all local data

---

## 📊 Data & Accuracy Issues

### Medication Information Seems Wrong

**What to do:**

1. **Verify with pharmacist**
   - Always verify medication information
   - Show MediGlobe results to pharmacist
   - Ask for confirmation

2. **Report the issue**
   - Email: [mediglobeapp@gmail.com](mailto:mediglobeapp@gmail.com)
   - Include:
     - Medication name
     - Country
     - What seems incorrect
     - Source of correct information (if known)

3. **Understand limitations**
   - Brand names vary by region
   - Databases may not be current
   - Formulations differ between countries
   - Some information may be incomplete

**We appreciate reports!** User feedback helps us improve the database for everyone.

---

## 🆘 Still Need Help?

### Issue Not Listed Here?

1. **Check the FAQ**
   - [Frequently Asked Questions](faq.md)
   - May have additional information

2. **Contact Support**
   - Email: [mediglobeapp@gmail.com](mailto:mediglobeapp@gmail.com)
   - Include:
     - Device model (e.g., "iPhone 14 Pro")
     - iOS version (Settings → General → About)
     - App version (MediGlobe Settings → About)
     - Detailed description of issue
     - Steps to reproduce
     - Screenshots (if applicable)

3. **Expected Response Time**
   - 24-48 hours during business days
   - May be longer on weekends/holidays

---

## 📋 Bug Report Template

Copy and paste this when emailing support:

Subject: MediGlobe Issue - [Brief Description]

Device Information:
• Device Model: [e.g., iPhone 14 Pro]
• iOS Version: [e.g., iOS 17.2]
• App Version: [Found in app Settings]

Issue Description:
[Describe what's happening]

Steps to Reproduce:
1. [First step]
2. [Second step]
3. [What happened]

Expected Behavior:
[What should happen]

Actual Behavior:
[What actually happened]

Frequency:
[ ] Happens every time
[ ] Happens sometimes
[ ] Happened once

Screenshots:
[Attach if helpful]

Additional Information:
[Anything else relevant]

---

## 🔍 Diagnostic Information

### How to Find App Version

1. Open MediGlobe
2. Tap settings or info icon
3. Scroll to bottom
4. Look for "Version 1.0" or similar

### How to Find iOS Version

1. Open Settings app
2. Go to General → About
3. Look for "iOS Version"
4. Example: iOS 17.2.1

### How to Check Storage

1. Settings → General → iPhone Storage
2. Wait for it to load
3. Check available space
4. Need at least 1GB free

### How to Check Network Speed

1. Open Safari
2. Search "speed test"
3. Run a test
4. MediGlobe needs at least 1 Mbps

---

## 💡 Pro Tips to Avoid Issues

### Before Traveling

- [ ] Search and favorite all your medications
- [ ] Test the app with your medications
- [ ] Screenshot important results
- [ ] Update app to latest version
- [ ] Update iOS to latest version
- [ ] Verify internet works on your plan abroad

### While Traveling

- [ ] Use offline mode when internet is unreliable
- [ ] Save important results to favorites
- [ ] Keep prescriptions with you
- [ ] Verify information with local pharmacists
- [ ] Take photos of local medication packaging

### General Maintenance

- [ ] Update app regularly
- [ ] Clear search history monthly
- [ ] Restart app if it becomes slow
- [ ] Report inaccurate information
- [ ] Back up your favorites (screenshot)

---

## 🎓 Common Mistakes

### Mistake 1: Using Brand Names Only
**Problem:** "Can't find Advil"
**Solution:** Try generic name "ibuprofen"

### Mistake 2: Expecting 100% Accuracy
**Problem:** "Brand name isn't available"
**Solution:** Verify with local pharmacist, brands vary

### Mistake 3: Relying on Interactions Only
**Problem:** "App says no interactions, so I combined medications"
**Solution:** **Always consult your doctor!** App is informational only

### Mistake 4: Not Granting Permissions
**Problem:** "Camera doesn't work"
**Solution:** Grant camera permission in Settings

### Mistake 5: Searching Without Internet
**Problem:** "Nothing found"
**Solution:** Connect to internet or use local database

---

**Safe travels and stay healthy! 🌍✈️💊**

*For informational purposes only. Not a substitute for professional medical advice.*

---

**Last Updated**: November 2025  
**Version**: 0.1

**Found a solution not listed here?** Email us so we can add it: [mediglobeapp@gmail.com](mailto:mediglobeapp@gmail.com)
