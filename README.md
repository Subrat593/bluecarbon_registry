# BlueCarbon Registry

A comprehensive carbon credit management platform with real-time IoT monitoring, blockchain integration, and environmental data tracking for blue carbon ecosystems.

## Progress

### Step 1: Dedicated Pages Creation ✅
**Status**: Completed  
**Summary**: Created three new dedicated pages with full functionality and updated navigation.

**What was done**:
- Created `/blockchain` page with wallet connection, contract information, and token management
- Created `/settings` page with user profile, notifications, preferences, and security options  
- Created `/help` page with FAQ, tutorials, and contact support
- Updated routing to include all new pages
- Enhanced 404 page with navigation to new pages

**Files created/modified**:
- `src/pages/blockchain/index.jsx` - Blockchain integration page
- `src/pages/settings/index.jsx` - User settings and preferences
- `src/pages/help/index.jsx` - Help and support center
- `src/Routes.jsx` - Added new routes
- `src/pages/NotFound.jsx` - Enhanced with navigation links

**How to test**:
```bash
npm start
# Navigate to:
# http://localhost:4028/blockchain
# http://localhost:4028/settings  
# http://localhost:4028/help
```

**Expected results**: All pages load correctly with proper styling, interactive elements, and navigation.

### Step 2: User Profile Page ✅
**Status**: Completed  
**Summary**: Created a comprehensive user profile page with detailed user information, statistics, and activity history.

**What was done**:
- Created `/profile` page with complete user profile management
- Added user statistics (projects, carbon credits, verification score)
- Implemented profile editing functionality with form controls
- Added recent activity feed with timestamps
- Included social media links and wallet address
- Updated settings page to link to the dedicated profile page
- Added profile route to navigation system

**Files created/modified**:
- `src/pages/profile/index.jsx` - Comprehensive user profile page
- `src/Routes.jsx` - Added profile route
- `src/pages/settings/index.jsx` - Updated to link to profile page

**How to test**:
```bash
npm start
# Navigate to:
# http://localhost:4028/profile
# Or go to Settings and click "View Full Profile"
```

**Expected results**: Profile page displays user information, statistics, recent activity, and allows editing of profile details.

## 🚀 Features

- **React 18** - React version with improved rendering and concurrent features
- **Vite** - Lightning-fast build tool and development server
- **Redux Toolkit** - State management with simplified Redux setup
- **TailwindCSS** - Utility-first CSS framework with extensive customization
- **React Router v6** - Declarative routing for React applications
- **Data Visualization** - Integrated D3.js and Recharts for powerful data visualization
- **Form Management** - React Hook Form for efficient form handling
- **Animation** - Framer Motion for smooth UI animations
- **Testing** - Jest and React Testing Library setup

## 📋 Prerequisites

- Node.js (v14.x or higher)
- npm or yarn

## 🛠️ Installation

1. Install dependencies:
   ```bash
   npm install
   # or
   yarn install
   ```
   
2. Start the development server:
   ```bash
   npm start
   # or
   yarn start
   ```

## 📁 Project Structure

```
react_app/
├── public/             # Static assets
├── src/
│   ├── components/     # Reusable UI components
│   ├── pages/          # Page components
│   ├── styles/         # Global styles and Tailwind configuration
│   ├── App.jsx         # Main application component
│   ├── Routes.jsx      # Application routes
│   └── index.jsx       # Application entry point
├── .env                # Environment variables
├── index.html          # HTML template
├── package.json        # Project dependencies and scripts
├── tailwind.config.js  # Tailwind CSS configuration
└── vite.config.js      # Vite configuration
```

## 🧩 Adding Routes

To add new routes to the application, update the `Routes.jsx` file:

```jsx
import { useRoutes } from "react-router-dom";
import HomePage from "pages/HomePage";
import AboutPage from "pages/AboutPage";

const ProjectRoutes = () => {
  let element = useRoutes([
    { path: "/", element: <HomePage /> },
    { path: "/about", element: <AboutPage /> },
    // Add more routes as needed
  ]);

  return element;
};
```

## 🎨 Styling

This project uses Tailwind CSS for styling. The configuration includes:

- Forms plugin for form styling
- Typography plugin for text styling
- Aspect ratio plugin for responsive elements
- Container queries for component-specific responsive design
- Fluid typography for responsive text
- Animation utilities

## 📱 Responsive Design

The app is built with responsive design using Tailwind CSS breakpoints.


## 📦 Deployment

Build the application for production:

```bash
npm run build
```

## 🙏 Acknowledgments

- Powered by React and Vite
- Styled with Tailwind CSS
