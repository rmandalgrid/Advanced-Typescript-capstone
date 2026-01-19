# Advanced TypeScript Capstone Project

A project management application built with TypeScript that demonstrates advanced TypeScript concepts including classes, interfaces, decorators, generics, and drag-and-drop functionality.

## 🚀 Features

- **Project Management**: Create and manage projects with title, description, and team size
- **Drag & Drop**: Move projects between "Active" and "Finished" lists using native HTML5 drag-and-drop API
- **Form Validation**: Client-side validation with custom validation utilities
- **State Management**: Singleton pattern for centralized state management
- **Component-Based Architecture**: Reusable component classes with inheritance
- **Type Safety**: Full TypeScript type checking with strict mode enabled

## 🛠️ Technologies Used

- **TypeScript** (v5.0.0) - Type-safe JavaScript
- **HTML5** - Native drag-and-drop API
- **CSS3** - Styling
- **ES6 Modules** - Modern JavaScript module system

## 📋 Prerequisites

- Node.js (v14 or higher)
- npm (v6 or higher)

## 🔧 Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd Advanced-Typescript-capstone
```

2. Install dependencies:
```bash
npm install
```

## 🎯 Usage

### Development Mode

Run TypeScript compiler in watch mode and start a development server:
```bash
npm run dev
```

This will:
- Compile TypeScript files automatically on changes (`tsc -w`)
- Start a live server on port 8080
- Open the application in your browser

### Build for Production

Compile TypeScript to JavaScript:
```bash
npm run build
```

### Start Production Server

Build and start a production server:
```bash
npm start
```

This will:
- Compile TypeScript files
- Start an HTTP server on port 8080
- Open the application in your browser

## 📁 Project Structure

```
Advanced-Typescript-capstone/
├── src/
│   ├── app.ts                    # Application entry point
│   ├── components/
│   │   ├── base-component.ts     # Base component class
│   │   ├── project-input.ts      # Project input form component
│   │   ├── project-item.ts       # Individual project item component
│   │   └── project-list.ts       # Project list component
│   ├── interfaces/
│   │   └── drag-drop.ts          # Drag and drop interfaces
│   ├── models/
│   │   └── project.ts            # Project model and status enum
│   ├── state/
│   │   └── project-state.ts      # State management (Singleton pattern)
│   └── util/
│       ├── decorators.ts         # Custom decorators (autobind)
│       └── validation.ts         # Validation utilities
├── dist/                         # Compiled JavaScript output
├── index.html                    # HTML template
├── app.css                       # Stylesheet
├── tsconfig.json                 # TypeScript configuration
└── package.json                  # Project dependencies and scripts
```

## 🎓 Key TypeScript Concepts Demonstrated

### 1. **Classes and Inheritance**
- Base component class with generic types
- Component inheritance for reusable UI elements

### 2. **Interfaces**
- `Draggable` and `DragTarget` interfaces for drag-and-drop functionality
- `Validatable` interface for form validation

### 3. **Generics**
- Generic `State<T>` class for type-safe state management
- Generic `Component<T, U>` class for flexible component creation

### 4. **Decorators**
- Custom `@autobind` decorator for automatic method binding
- Experimental decorator support enabled in TypeScript config

### 5. **Enums**
- `ProjectStatus` enum for project state management

### 6. **Type Guards**
- Type checking and validation utilities
- Type-safe form input handling

### 7. **Singleton Pattern**
- `ProjectState` singleton for centralized state management

### 8. **Strict Type Checking**
- All strict TypeScript options enabled
- No implicit any, strict null checks, and more

## 📝 How It Works

1. **Project Input**: Users can create new projects by filling out a form with:
   - Title (required)
   - Description (required, minimum 5 characters)
   - Number of people (required, between 1-5)

2. **Project Lists**: Projects are displayed in two lists:
   - **Active Projects**: Newly created projects appear here
   - **Finished Projects**: Completed projects are moved here

3. **Drag & Drop**: Users can drag projects between the two lists to change their status

4. **State Management**: The `ProjectState` singleton manages all projects and notifies listeners when changes occur

5. **Validation**: All form inputs are validated before submission using custom validation utilities

## 🎨 Customization

You can customize the application by:
- Modifying `app.css` for styling changes
- Updating validation rules in `src/util/validation.ts`
- Adding new project fields in `src/models/project.ts`
- Extending components in the `src/components/` directory

## 📄 License

ISC

## 👤 Author

**Roshni Mandal**

---

This project is part of a TypeScript course capstone project demonstrating advanced TypeScript features and best practices.
