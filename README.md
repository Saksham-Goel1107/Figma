<div align="center">
  <br />
  <a href="https://github.com/Saksham-goel1107/Figma" target="_blank">
    <img src="https://github.com/Saksham-goel1107/Figma/assets/raw/main/public/assets/logo.svg" alt="Figma Clone Logo" width="150">
  </a>
  <h1 align="center">Figma Clone</h1>
  <p align="center">
    A real-time collaborative design platform with features like multi-cursor support, live collaboration, and design tools
  </p>

  <p align="center">
    <img src="https://img.shields.io/badge/Created%20By-Saksham%20Goel-blue?style=for-the-badge" alt="Created By Saksham Goel" />
    <img src="https://img.shields.io/github/license/Saksham-goel1107/Figma?style=for-the-badge&color=green" alt="License" />
    <img src="https://img.shields.io/github/stars/Saksham-goel1107/Figma?style=for-the-badge&color=yellow" alt="Stars" />
    <img src="https://img.shields.io/github/forks/Saksham-goel1107/Figma?style=for-the-badge&color=orange" alt="Forks" />
  </p>

  <p align="center">
    <img src="https://img.shields.io/badge/Next.js-14.1.0-black?style=for-the-badge&logo=next.js" alt="Next.js" />
    <img src="https://img.shields.io/badge/TypeScript-5.0-blue?style=for-the-badge&logo=typescript" alt="TypeScript" />
    <img src="https://img.shields.io/badge/Liveblocks-1.9.7-purple?style=for-the-badge" alt="Liveblocks" />
    <img src="https://img.shields.io/badge/Fabric.js-5.3.0-teal?style=for-the-badge" alt="Fabric.js" />
    <img src="https://img.shields.io/badge/TailwindCSS-3.4.1-06B6D4?style=for-the-badge&logo=tailwindcss" alt="Tailwind CSS" />
  </p>
</div>

## 📋 Table of Contents

- [Live Demo](#-live-demo)
- [Project Overview](#-project-overview)
- [Features](#-features)
- [Technologies Used](#%EF%B8%8F-technologies-used)
- [Getting Started](#-getting-started)
- [Environment Variables](#-environment-variables)
- [Project Structure](#-project-structure)
- [Collaboration Features](#-collaboration-features)
- [Design Tools](#%EF%B8%8F-design-tools)
- [Known Issues & Future Improvements](#-known-issues--future-improvements)
- [Contributing](#-contributing)
- [License](#-license)
- [Contact](#-contact)

## 📝 Project Overview

This project is a feature-rich Figma clone built with modern web technologies. It provides a collaborative design platform where multiple users can work together in real-time, chat, comment, and create designs using various tools similar to the original Figma platform.

## 🔋 Features

### Collaboration
- **Multi-Cursor Support**: See where other users are working in real-time
- **Cursor Chat**: Communicate with other users directly through cursor chat bubbles
- **Reactions**: React to designs with emoji reactions
- **Active Users**: View all active users in the current workspace
- **Comments**: Leave comments tied to specific parts of the design

### Design Tools
- **Shape Creation**: Create rectangles, circles, triangles, lines, and more
- **Image Upload**: Add images to your canvas
- **Freeform Drawing**: Draw freely on the canvas
- **Text Elements**: Add and format text
- **Object Customization**: Change colors, sizes, and positions
- **Layering**: Bring elements forward or backward

### Workspace Features
- **Undo/Redo**: Revert or reapply changes
- **Keyboard Shortcuts**: Speed up your workflow with shortcuts
- **History Tracking**: View the history of changes
- **Canvas Management**: Delete, scale, move, and clear canvas elements
- **Export Options**: Export designs in various formats

## ⚙️ Technologies Used

- **Frontend Framework**: Next.js 14
- **Programming Language**: TypeScript
- **Real-time Collaboration**: Liveblocks
- **Canvas Manipulation**: Fabric.js
- **UI Components**: Shadcn UI
- **Styling**: Tailwind CSS
- **PDF Generation**: jsPDF
- **Unique IDs**: UUID

## 🚀 Getting Started

### Prerequisites

- Node.js (v16.0.0 or later)
- npm (v7.0.0 or later)

### Installation

1. Clone the repository
```bash
git clone https://github.com/Saksham-goel1107/Figma.git
cd Figma
```

2. Install dependencies
```bash
npm install
```

3. Set up environment variables
   - Create a `.env` file in the root directory
   - Copy the contents from `.env.example`
   - Fill in the required values (see [Environment Variables](#-environment-variables))

4. Start the development server
```bash
npm run dev
```

5. Open [http://localhost:3000](http://localhost:3000) in your browser

## 🔐 Environment Variables

```
# Liveblocks API key for real-time collaboration
NEXT_PUBLIC_LIVEBLOCKS_PUBLIC_KEY=

# Next.js environment variables
NEXT_PUBLIC_APP_URL=http://localhost:3000

# Optional: For production environments
NODE_ENV=production
```

To obtain your Liveblocks API keys:
1. Sign up at [liveblocks.io](https://liveblocks.io)
2. Create a new project
3. Navigate to API Keys in your dashboard
4. Copy both Public and Secret keys to your `.env` file

## 📁 Project Structure

```
├── app/                # Next.js app directory
│   ├── App.tsx         # Main application component
│   ├── Room.tsx        # Liveblocks room configuration
│   └── page.tsx        # Entry page
├── components/         # UI components
│   ├── comments/       # Comment-related components
│   ├── cursor/         # Cursor-related components
│   ├── reaction/       # Reaction-related components
│   ├── settings/       # Settings panels
│   ├── ui/             # UI components from ShadCN
│   └── users/          # User-related components
├── constants/          # Application constants
├── hooks/              # Custom React hooks
├── lib/                # Utility functions
│   ├── canvas.ts       # Canvas manipulation functions
│   ├── shapes.ts       # Shape creation utilities
│   └── utils.ts        # General utilities
├── public/             # Static assets
└── types/              # TypeScript type definitions
```

## 👥 Collaboration Features

### Real-time Cursors

The multi-cursor feature allows users to see where others are working in real-time. Each user gets a unique cursor color for easy identification.

### Comment System

The comment system allows users to leave feedback on specific parts of the design. Comments are attached to coordinates on the canvas and are visible to all collaborators.


### Reactions

Users can react to designs or comments with emoji reactions, providing quick feedback without interrupting the workflow.

## 🖌️ Design Tools

### Canvas Tools

The application provides a comprehensive set of tools for creating and manipulating designs:

- **Selection Tool**: Select and manipulate objects
- **Shape Tools**: Create various geometric shapes
- **Text Tool**: Add and format text elements
- **Image Tool**: Upload and resize images
- **Pen Tool**: Create freeform drawings
- **Color Picker**: Change the color of objects
- **Alignment Tools**: Align objects horizontally or vertically

### Properties Panel

The properties panel allows for detailed customization of selected objects:
- Dimensions (width and height)
- Position (x and y coordinates)
- Fill and stroke colors
- Opacity
- Layer positioning

## 🔧 Known Issues & Future Improvements

- **Authentication**: Implementing user authentication and access control
- **Templates**: Adding pre-designed templates for quick starts
- **More Export Options**: Supporting additional export formats
- **Performance Optimizations**: For handling larger and more complex designs
- **Mobile Responsiveness**: Improving the experience on smaller devices

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📬 Contact

Saksham Goel - [GitHub](https://github.com/Saksham-goel1107)

Project Link: [https://github.com/Saksham-goel1107/Figma](https://github.com/Saksham-goel1107/Figma)

---

<div align="center">
  <p>
    If you found this project helpful, please give it a ⭐️ on 
    <a href="https://github.com/Saksham-goel1107/Figma">GitHub</a>
  </p>
  <p>
    Built with ❤️ by <a href="https://github.com/Saksham-goel1107">Saksham Goel</a>
  </p>
</div>
