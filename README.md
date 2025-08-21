# Location App Mobile

React Native mobile application for location-based services with MapmyIndia and Google Maps integration, supporting both iOS and Android platforms.

## 🚀 Technology Stack

- **Framework**: React Native
- **Platform**: iOS & Android
- **Maps**: MapmyIndia & Google Maps Platform
- **Navigation**: React Navigation
- **State Management**: Redux/Context API
- **Location Services**: React Native Geolocation
- **Real-time**: WebSocket integration
- **UI Components**: Custom components with native feel

## 🏗️ Project Structure

```
mobile-app/
├── src/
│   ├── assets/          # Images, fonts, icons
│   │   ├── fonts/       # Custom fonts
│   │   ├── icons/       # App icons
│   │   └── images/      # Image assets
│   ├── components/      # Reusable UI components
│   ├── contexts/        # React contexts
│   ├── hooks/           # Custom React hooks
│   ├── navigation/      # Navigation configuration
│   ├── screens/         # App screens/pages
│   ├── services/        # API and external services
│   └── utils/           # Utility functions
├── android/             # Android-specific code
├── ios/                 # iOS-specific code
└── __tests__/           # Test files
```

## 🔧 Features

- **Cross-platform**: Single codebase for iOS and Android
- **Location Services**: Real-time location tracking and geofencing
- **Interactive Maps**: MapmyIndia and Google Maps integration
- **Offline Support**: Offline map capabilities
- **Push Notifications**: Real-time notifications
- **User Authentication**: Secure login and registration
- **Performance Optimized**: Smooth animations and fast loading
- **Responsive Design**: Adaptive UI for different screen sizes

## 🛠️ Development Setup

### Prerequisites

- Node.js (v16 or higher)
- React Native CLI
- Android Studio (for Android development)
- Xcode (for iOS development, macOS only)
- CocoaPods (for iOS dependencies)

### Installation

1. Clone the repository
```bash
git clone https://github.com/pranjal255/location-app-mobile.git
cd location-app-mobile
```

2. Install dependencies
```bash
npm install
```

3. Install iOS dependencies (macOS only)
```bash
cd ios && pod install && cd ..
```

4. Set up environment variables
```bash
cp .env.example .env
# Add your API keys for MapmyIndia and Google Maps
```

### Running the App

#### Android
```bash
# Start Metro bundler
npm start

# Run on Android (in another terminal)
npm run android
```

#### iOS (macOS only)
```bash
# Start Metro bundler
npm start

# Run on iOS (in another terminal)
npm run ios
```

## 🗺️ Maps Integration

### MapmyIndia Setup
1. Get API key from MapmyIndia developer console
2. Add to `.env` file: `MAPMYINDIA_API_KEY=your_key_here`

### Google Maps Setup
1. Get API key from Google Cloud Console
2. Enable Maps SDK for Android/iOS
3. Add to `.env` file: `GOOGLE_MAPS_API_KEY=your_key_here`

## 🧪 Testing

```bash
# Run unit tests
npm test

# Run tests with coverage
npm run test:coverage

# Run E2E tests (requires setup)
npm run test:e2e
```

## 📱 Building for Production

### Android
```bash
# Generate signed APK
npm run build:android

# Generate AAB for Play Store
npm run build:android:bundle
```

### iOS
```bash
# Build for iOS
npm run build:ios
```

## 🚀 Deployment

### Android (Google Play Store)
1. Build signed AAB
2. Upload to Google Play Console
3. Follow Play Store review process

### iOS (App Store)
1. Build archive in Xcode
2. Upload to App Store Connect
3. Submit for App Store review

## 📚 API Integration

The mobile app connects to the backend API for:
- User authentication
- Location data synchronization
- Real-time updates
- File uploads

Backend API: [location-app-backend](https://github.com/pranjal255/location-app-backend)

## 🔧 Configuration

### Environment Variables
```
BACKEND_API_URL=https://your-backend-api.com
MAPMYINDIA_API_KEY=your_mapmyindia_key
GOOGLE_MAPS_API_KEY=your_google_maps_key
```

## 📄 License

This project is licensed under the MIT License.

## 🔗 Related Repositories

- [Backend API](https://github.com/pranjal255/location-app-backend) - Node.js backend server
- [Main Project](https://github.com/pranjal255/location-app-project) - Project overview and documentation

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## 📞 Support

For support and questions, please open an issue in the GitHub repository.
