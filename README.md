# VIT-AP WiFi Login Manager (Offline Mode)

A modern, **offline-capable** WiFi login manager for VIT-AP students that stores your login profiles locally on your device.

## ✨ Features

- **🔌 Completely Offline**: Works without internet connection
- **💾 Local Storage**: Your WiFi profiles are saved locally on your device
- **📱 Multiple Profiles**: Store up to 5 different login profiles (phone, laptop, tablet, etc.)
- **⚡ One-Click Login/Logout**: Quick access to VIT-AP WiFi with saved credentials
- **📊 Real-time Status**: Visual indicators for connection status
- **🔒 Secure Storage**: Credentials are stored securely in browser's local storage
- **🎨 Modern UI**: Clean, responsive design with smooth animations
- **📤 Backup/Restore**: Export and import your profiles as JSON files

## 🚀 Quick Start

### **Step 1: Download the Files**
1. Download `wifi.html` to your computer
2. Save it in a folder of your choice

### **Step 2: Open the App**
1. Double-click `wifi.html` to open it in your browser
2. Or drag and drop the file into your browser window
3. The app will work immediately - no setup required!

### **Step 3: Add Your Profiles**
1. Click the **+** button to add a new profile
2. Enter your VIT-AP registration number and password
3. Your profiles are automatically saved locally

## 📱 Usage

### **Adding Profiles**
1. Click the **+** button to add a new profile
2. Enter a profile name (e.g., "My Phone", "Laptop")
3. Enter your VIT-AP registration number as username
4. Enter your password
5. Click **Save**

### **Logging In/Out**
1. Select a profile from the list
2. Click **Login with Selected Profile** to connect
3. Click **Logout Selected Profile** to disconnect
4. Check the status indicator for connection confirmation

### **Offline Status**
- **💾✅ Offline Mode**: App is working normally
- **💾⏳ Saving**: Data is being saved locally
- **💾❌ Error**: There was an error saving data

## 🔧 Configuration

### **Customizing the App**

You can edit the configuration section in `wifi.html`:

```javascript
const LOGIN_URL = 'https://hfw.vitap.ac.in:8090/httpclient.html'; // WiFi portal URL
const MAX_PROFILES = 5; // Maximum number of profiles allowed
const STORAGE_KEY = 'vitap-wifi-profiles'; // Local storage key
```

## 🛡️ Security Features

- **Local Storage Only**: Your credentials never leave your device
- **No Internet Required**: Works completely offline
- **Browser Security**: Uses browser's built-in security features
- **No Server Storage**: No external servers involved

## 📤 Backup & Restore

### **Exporting Profiles**
Your profiles are automatically saved in your browser's local storage. To backup:

1. Open browser developer tools (F12)
2. Go to Console tab
3. Type: `exportProfiles()` and press Enter
4. A JSON file will be downloaded with your profiles

### **Importing Profiles**
1. Open browser developer tools (F12)
2. Go to Console tab
3. Type: `importProfiles(file)` where `file` is your JSON backup
4. Your profiles will be restored

## 🔄 Data Storage

Your data is stored in your browser's local storage with this structure:

```json
{
  "profiles": [
    {
      "name": "Profile Name",
      "username": "reg_number",
      "password": "password"
    }
  ],
  "lastSelectedProfileIndex": 0
}
```

## 🐛 Troubleshooting

### **Profiles Not Saving**
- Check if your browser supports local storage
- Try clearing browser cache and cookies
- Check browser console for error messages

### **Login Issues**
- Verify your VIT-AP credentials
- Check if the WiFi portal URL is correct
- Try logging out first, then logging in again

### **App Not Working**
- Make sure you're using a modern browser (Chrome, Firefox, Safari, Edge)
- Check if JavaScript is enabled
- Try refreshing the page

## 📋 Requirements

- **Modern web browser** (Chrome, Firefox, Safari, Edge)
- **JavaScript enabled**
- **VIT-AP student credentials**
- **No internet connection required!**

## 🌟 Advantages of Offline Mode

- **⚡ Instant Loading**: No waiting for cloud connections
- **🔒 Privacy**: Your data never leaves your device
- **🌐 No Internet Required**: Works anywhere, anytime
- **💰 No Costs**: No cloud storage fees
- **🛡️ Security**: No external servers involved
- **📱 Portable**: Just one HTML file, works on any device

## 🤝 Contributing

Feel free to submit issues and enhancement requests!

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## ⚠️ Disclaimer

This tool is for educational purposes. Always follow your institution's IT policies and guidelines. The developers are not responsible for any misuse of this application.

---

**Made with ❤️ for VIT-AP Students**

*Works completely offline - no internet required!* 🌟
