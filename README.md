# React Redux Calculator

A modern, accessible calculator built with React 18 and Redux Toolkit. Features a clean iOS-inspired design with full keyboard support and comprehensive error handling.

## 🚀 Quick Start

### Prerequisites
- Node.js 16+ 
- npm or yarn

### Installation & Setup

```bash
# Clone the repository
git clone <https://github.com/hrutikworkspace/React-Redux-Calculator.git>
cd react-redux-calculator

# Install dependencies
npm install

# Start development server
npm start

# Build for production
npm run build

# Run tests
npm test
```

### Available Scripts

- `npm start` - Start development server
- `npm run build` - Create production build
- `npm test` - Run test suite
- `npm run test:coverage` - Run tests with coverage report
- `npm run lint` - Run ESLint
- `npm run format` - Format code with Prettier

## 🛠 Tech Stack

### Core Dependencies
- **React 18** - UI library with hooks and functional components
- **Redux Toolkit** - State management with modern Redux patterns
- **React-Redux** - React bindings for Redux

### Development Tools
- **Vite** - Fast build tool and development server
- **Jest** - Testing framework
- **React Testing Library** - Component testing utilities
- **ESLint** - Code linting
- **Prettier** - Code formatting

### Why These Choices?

**Redux Toolkit**: Chosen over plain Redux for its simplified syntax, built-in best practices, and reduced boilerplate. The `createSlice` API makes state management more intuitive.

**Functional Components + Hooks**: Modern React patterns that are more performant and easier to test than class components.

**CSS-in-JS**: Inline styles for component isolation and dynamic theming without external dependencies.

## 📱 Features

### Core Functionality
- ✅ Basic arithmetic operations (+, −, ×, ÷)
- ✅ Sequential operations (5 + 2 × 3 = 21)
- ✅ Decimal number support
- ✅ Clear (AC) functionality

### Edge Case Handling
- ✅ Division by zero protection with user-friendly error messages
- ✅ Leading zero prevention (0002 → 2)
- ✅ Floating point precision handling
- ✅ Display length limiting

### Accessibility & UX
- ✅ Full keyboard navigation support
- ✅ Screen reader compatibility with ARIA labels
- ✅ Visible focus indicators
- ✅ Semantic HTML elements
- ✅ Responsive design for mobile devices
- ✅ High contrast mode support
- ✅ Reduced motion support

### Keyboard Shortcuts
- `0-9` - Number input
- `+, -, *, /` - Operations
- `Enter` or `=` - Calculate result
- `.` or `,` - Decimal point
- `Escape` or `C` - Clear calculator

## 🏗 Project Structure

```
src/
├── components/
│   ├── Calculator.jsx      # Main calculator component
│   ├── Display.jsx         # Display component
│   ├── Keypad.jsx         # Keypad component
│   └── Button.jsx         # Reusable button component
├── store/
│   ├── index.js           # Store configuration
│   └── calculatorSlice.js # Calculator state slice
├── utils/
│   └── calculations.js    # Math operation utilities
├── __tests__/
│   ├── Calculator.test.js
│   ├── calculatorSlice.test.js
│   └── calculations.test.js
└── App.jsx               # Root component
```

## 🧪 Testing Strategy

### Test Coverage
- **Unit Tests**: All Redux reducers and utility functions
- **Integration Tests**: Component interactions with Redux store
- **Accessibility Tests**: ARIA labels and keyboard navigation
- **Edge Case Tests**: Error handling and boundary conditions

### Running Tests
```bash
# Run all tests
npm test

# Run tests in watch mode
npm test -- --watch

# Generate coverage report
npm test -- --coverage
```

## 🎨 Design Decisions

### Visual Design
- **iOS Calculator Inspired**: Familiar and intuitive interface
- **Dark Theme**: Reduces eye strain and looks modern
- **Rounded Buttons**: Friendly, touchable interface elements
- **Color Coding**: Different colors for numbers, operations, and functions

### State Management
- **Single Slice**: All calculator state in one Redux slice for simplicity
- **Immutable Updates**: Using Redux Toolkit's Immer integration
- **Memoized Selectors**: Prevent unnecessary re-renders

### Performance Optimizations
- **React.memo**: Memoized Button components
- **useCallback**: Memoized event handlers
- **Efficient Re-renders**: Targeted state updates

## 🚧 Development Notes

### Git Workflow
This project follows Conventional Commits:
- `feat:` - New features
- `fix:` - Bug fixes  
- `docs:` - Documentation changes
- `style:` - Code formatting
- `refactor:` - Code restructuring
- `test:` - Test additions/modifications

### Code Style
- Functional components with hooks
- Consistent naming conventions
- Comprehensive prop validation
- Self-documenting code with meaningful variable names

## 📋 Future Enhancements

- [ ] Scientific calculator functions
- [ ] History of calculations
- [ ] Themes and customization
- [ ] Unit conversion
- [ ] Expression parsing

## 🐛 Known Issues

None currently. Please report issues via GitHub Issues.

## 📄 License

MIT License - feel free to use this project for learning and development.

---

**Built with ❤️ using React & Redux Toolkit**