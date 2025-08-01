# Cybersecurity Incident Response Automation Tool

A comprehensive cybersecurity dashboard for real-time threat monitoring, incident response automation, and security operations center (SOC) management.

## Features

- **Real-time Threat Detection**: Live monitoring of security incidents with automated classification
- **Network Traffic Analysis**: Continuous monitoring of network activity with suspicious behavior detection
- **Incident Management**: Comprehensive incident tracking with automated response actions
- **Alert System**: Real-time alerts with acknowledgment and escalation capabilities
- **System Status Monitoring**: Health monitoring of critical security infrastructure
- **Interactive Threat Map**: Visual representation of global threat landscape
- **Automated Response**: Configurable response playbooks for different incident types

## Tech Stack

- **Frontend**: React 18 + TypeScript
- **Styling**: Tailwind CSS
- **Icons**: Lucide React
- **Build Tool**: Vite
- **Linting**: ESLint + TypeScript ESLint

## Getting Started

### Prerequisites

- Node.js 18+ 
- npm or yarn
- VS Code (recommended)

### Installation

1. Clone the repository
2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm run dev
   ```

4. Open your browser and navigate to `http://localhost:5173`

### VS Code Setup

This project includes VS Code configuration for optimal development experience:

- **Recommended Extensions**: Automatically suggests useful extensions
- **Settings**: Pre-configured for TypeScript, Tailwind CSS, and React development
- **Tasks**: Quick access to npm scripts via Command Palette
- **Debugging**: Chrome debugging configuration included

#### Recommended VS Code Extensions

- Tailwind CSS IntelliSense
- Prettier - Code formatter
- ESLint
- TypeScript and JavaScript Language Features
- Auto Rename Tag
- Path Intellisense

### Development Commands

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run lint` - Run ESLint
- `npm run preview` - Preview production build

### VS Code Usage

1. **Running the Development Server**:
   - Press `Ctrl+Shift+P` (or `Cmd+Shift+P` on Mac)
   - Type "Tasks: Run Task"
   - Select "npm: dev"

2. **Debugging**:
   - Set breakpoints in your TypeScript/React code
   - Press `F5` or go to Run and Debug panel
   - Select "Launch Chrome" configuration

3. **Code Formatting**:
   - Files are automatically formatted on save
   - Manual format: `Shift+Alt+F` (or `Shift+Option+F` on Mac)

## Project Structure

```
src/
├── components/          # React components
│   ├── Dashboard.tsx    # Main dashboard component
│   ├── ThreatMap.tsx    # Interactive threat visualization
│   ├── NetworkMonitor.tsx # Network traffic monitoring
│   ├── SystemStatus.tsx # System health monitoring
│   ├── AlertPanel.tsx   # Alert management
│   └── IncidentList.tsx # Incident tracking
├── hooks/              # Custom React hooks
│   └── useIncidentData.ts # Data management hook
├── types/              # TypeScript type definitions
│   └── incident.ts     # Core data types
├── utils/              # Utility functions
│   └── dataSimulator.ts # Mock data generation
├── App.tsx             # Root component
└── main.tsx           # Application entry point
```

## Features Overview

### Dashboard Components

1. **Threat Map**: Visual representation of global security threats with real-time updates
2. **Network Monitor**: Live network traffic analysis with suspicious activity detection
3. **System Status**: Health monitoring of critical security infrastructure
4. **Alert Panel**: Real-time security alerts with acknowledgment capabilities
5. **Incident List**: Comprehensive incident tracking and management

### Data Simulation

The application includes a sophisticated data simulation system that generates:
- Realistic security incidents with various threat types
- Network traffic patterns with suspicious activity indicators
- System health metrics and status updates
- Security alerts and notifications

### Responsive Design

- Mobile-first responsive design
- Optimized for various screen sizes
- Touch-friendly interface elements
- Accessible color schemes and typography

## Customization

### Adding New Incident Types

1. Update the `incidentTypes` array in `src/utils/dataSimulator.ts`
2. Add corresponding response actions and descriptions
3. Update type definitions in `src/types/incident.ts`

### Modifying Alert Thresholds

Adjust alert generation logic in `src/hooks/useIncidentData.ts`:
- Change probability thresholds for incident generation
- Modify alert criteria for suspicious network traffic
- Customize system status monitoring intervals

### Styling Customization

The application uses Tailwind CSS for styling:
- Modify color schemes in component files
- Adjust spacing and layout in grid configurations
- Customize animations and transitions

## Production Deployment

1. Build the application:
   ```bash
   npm run build
   ```

2. The `dist` folder contains the production-ready files
3. Deploy to your preferred hosting platform (Netlify, Vercel, etc.)

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Run linting and ensure code quality
5. Submit a pull request

## License

This project is licensed under the MIT License.