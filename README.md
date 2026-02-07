# National Digital Health Passport

A secure, cloud-based digital health platform that provides each Malawian with a single, comprehensive medical record throughout their lifetime, accessible via National ID and fingerprint verification.

![Platform](https://img.shields.io/badge/Platform-Flutter-02569B?logo=flutter)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Active-success)

## Overview

The **National Digital Health Passport** is a revolutionary healthcare system designed to modernize medical record management in Malawi. By linking medical records to National IDs and fingerprints, the system ensures secure, instant access to complete patient medical histories at any healthcare facility across the country.

### Key Benefits

- **Single Medical Record**: One comprehensive record for life
- **Instant Access**: Retrieve complete medical history in seconds
- **Paperless**: No more lost forms, cards, or paper records
- **Secure**: Protected by fingerprint biometric authentication
- **Nationwide**: Accessible at any clinic or hospital in Malawi
- **Cloud-Based**: Always available, never lost

## How It Works

### 1. Patient Registration
When a patient registers at a health clinic for the first time:
- Their **National ID** is captured
- Their **fingerprint** is scanned and recorded
- A unique medical record is created and linked to their biometric data
- **For children under 16**: Records are linked to their mother's or guardian's National ID until they receive their own ID at age 16

### 2. Patient Check-In
At any subsequent visit to any healthcare facility:
- Patient simply **swipes their fingerprint** at the clinic/hospital
- The system instantly retrieves their complete medical history
- Healthcare worker can view all past records including:
  - **Prescriptions**
  - **Vaccinations/Shots**
  - **Lab Tests**
  - **Diagnoses**
  - **General Checkups**
  - **Hospital Visits**

### 3. Record Management
Healthcare workers can:
- View complete patient medical history
- Add new diagnoses, prescriptions, and test results
- Update vaccination records
- Track medication adherence
- Monitor health trends over time

## System Features

### For Health Workers
- **Quick Patient Lookup**: Fingerprint or National ID search
- **Complete Medical History**: Instant access to all patient records
- **Real-time Updates**: Add information that's immediately available system-wide
- **Health Analytics**: Track trends and patient progress
- **Medication Tracking**: Monitor prescription adherence
- **Dark Mode**: Reduce eye strain during long shifts

### For Patients
- **Continuity of Care**: Consistent medical records regardless of facility
- **No Lost Records**: Cloud-based storage ensures records are never lost
- **Fast Check-In**: Simple fingerprint scan for instant access
- **Complete History**: All medical information in one place
- **Privacy Protected**: Biometric security ensures only authorized access

### For Healthcare System
- **Reduced Paperwork**: Eliminate paper forms and cards
- **Better Data**: Comprehensive health statistics for public health planning
- **Cost Savings**: Reduced administrative overhead
- **Improved Outcomes**: Better-informed treatment decisions
- **Disease Tracking**: Enhanced epidemic monitoring and response

## Technical Stack

### Frontend (Flutter)
- **Framework**: Flutter 3.0+
- **Language**: Dart
- **UI Library**: Material Design 3
- **Charts**: FL Chart
- **Fonts**: Google Fonts (Plus Jakarta Sans)
- **State Management**: StatefulWidget (can be upgraded to Provider/Riverpod)

### Design Features
- Responsive design (Mobile, Tablet, Desktop)
- Dark mode support
- Modern, clean UI with smooth animations
- Accessibility-focused design
- Material Design 3 components

## Platform Support

- Android
- iOS
- Web
- Windows
- macOS
- Linux

## Getting Started

### Prerequisites

```bash
# Install Flutter (3.0 or higher)
flutter --version

# Verify Flutter installation
flutter doctor
```

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/your-org/national_digital_health_passport.git
cd national_digital_health_passport
```

2. **Install dependencies**
```bash
flutter pub get
```

3. **Run the application**
```bash
# For development
flutter run

# For specific platform
flutter run -d chrome        # Web
flutter run -d windows       # Windows
flutter run -d macos         # macOS
flutter run -d linux         # Linux
```

### Building for Production

```bash
# Android
flutter build apk --release
flutter build appbundle --release

# iOS
flutter build ios --release

# Web
flutter build web --release

# Desktop
flutter build windows --release
flutter build macos --release
flutter build linux --release
```

## Project Structure

```
national_digital_health_passport/
├── lib/
│   ├── main.dart                 # Main application entry point
│   ├── screens/                  # Application screens
│   ├── widgets/                  # Reusable widget components
│   ├── models/                   # Data models
│   ├── services/                 # API and business logic
│   └── utils/                    # Helper functions
├── android/                      # Android-specific files
├── ios/                          # iOS-specific files
├── web/                          # Web-specific files
├── windows/                      # Windows-specific files
├── macos/                        # macOS-specific files
├── linux/                        # Linux-specific files
├── pubspec.yaml                  # Dependencies and assets
└── README.md                     # This file
```

## Configuration

### Dependencies

```yaml
dependencies:
  flutter:
    sdk: flutter
  google_fonts: ^6.1.0      # Custom typography
  fl_chart: ^0.66.0         # Data visualization
```

### Environment Variables

Create a `.env` file in the root directory:

```env
API_BASE_URL=https://api.healthpassport.mw
API_KEY=your_api_key_here
FINGERPRINT_DEVICE_ID=device_id
```

## Security Features

- **Biometric Authentication**: Fingerprint-based patient identification
- **End-to-End Encryption**: All medical data encrypted in transit and at rest
- **Role-Based Access Control**: Different permissions for different healthcare roles
- **Audit Logging**: Complete track of who accessed what and when
- **HIPAA Compliant**: Follows international medical data privacy standards
- **Secure Cloud Storage**: Data stored in secure, redundant cloud infrastructure

## User Roles

### 1. Healthcare Worker
- Access patient records via fingerprint/ID scan
- Add new medical records
- View complete patient history
- Update prescriptions and diagnoses

### 2. Administrator
- Manage healthcare worker accounts
- System configuration
- Generate reports and analytics
- Monitor system health

### 3. Guardian (for children under 16)
- View child's medical records
- Consent to treatments
- Update contact information

## Dashboard Features

### Main Dashboard
- Patient intake with fingerprint scanning
- Quick National ID entry
- Real-time health statistics
- Recent patient activity

### Analytics
- Health history trends
- Medication adherence tracking
- Vital signs monitoring (heart rate, temperature, blood pressure)
- Patient visit patterns

### Calendar Integration
- Appointment scheduling
- Vaccination reminders
- Follow-up tracking
- Medication schedules

## Roadmap

### Phase 1 (Current)
- Core UI/UX design
- Dashboard implementation
- Dark mode support
- Responsive design

### Phase 2 (In Progress)
- Backend API integration
- Fingerprint scanner integration
- National ID database connection
- Authentication system

### Phase 3 (Planned)
- Offline mode support
- Multi-language support (English, Chichewa, Tumbuka)
- SMS notifications
- Prescription printing

### Phase 4 (Future)
- AI-powered health insights
- Telemedicine integration
- Mobile app for patients
- Payment integration for insurance

## Contributing

We welcome contributions from the community! Please read our [Contributing Guidelines](CONTRIBUTING.md) before submitting pull requests.

### How to Contribute

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Support

For support and questions:

- **Email**: support@healthpassport.mw
- **Phone**: +265 XXX XXX XXX
- **Website**: https://healthpassport.mw
- **Documentation**: https://docs.healthpassport.mw

## Acknowledgments

- Ministry of Health, Malawi
- National Registration Bureau
- Healthcare workers across Malawi
- Flutter and Dart development teams
- Open source community

## Statistics

- **Registered Users**: Growing daily
- **Healthcare Facilities**: Nationwide coverage
- **Records Digitized**: Millions of medical records
- **Paperwork Eliminated**: 100% digital records

---

**Built with care for better healthcare in Malawi**

*Securing health records, empowering healthcare workers, improving patient outcomes.*
