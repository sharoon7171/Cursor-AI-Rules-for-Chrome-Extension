# Chrome Extension Development - Cursor Rules

Professional, organized Chrome extension development rules using latest web standards (September 2025).

## ⚡ One-Line Installation

### Using Git (Recommended)
```bash
git clone --depth 1 --filter=blob:none --sparse https://github.com/sharoon7171/Cursor-AI-Rules-for-Chrome-Extension.git temp && cd temp && git sparse-checkout set .cursor && cp -r .cursor ../. && cd .. && rm -rf temp
```

### Manual Installation
1. Download this repository as ZIP
2. Extract the `.cursor` directory  
3. Copy it to your Chrome extension project root
4. Restart Cursor IDE to load the rules

### Verify Installation
```bash
ls .cursor/rules/  # Should show 6 .mdc rule files
```

## 📁 Rule Structure

```
.cursor/rules/
├── chrome-extension-development.mdc     # Core standards: Manifest V3, Chrome APIs (Always Applied)
├── ultra-modular-project-structure.mdc # Architecture: Component hierarchy, file organization  
├── javascript-mjs-standards.mdc        # JavaScript: ES2024+ features, patterns (.mjs files)
├── html-css-ui-standards.mdc          # UI/UX: HTML5/CSS3, responsive design (.html/.css files)
├── security-permissions-standards.mdc  # Security: Zero-trust, permissions, validation
└── testing-deployment-workflows.mdc    # Quality: Testing, CI/CD, store publishing
```

## 🎯 Key Features

### ✅ Modern Standards
- **Manifest V3** exclusively - no legacy code
- **ES Modules (.mjs)** - latest JavaScript features
- **Service Workers** - replaces background pages
- **Latest Chrome APIs** - 2025 standards
- **Security-first approach** - minimal permissions

### ✅ Ultra-Modular Organization
- **Every component separated** - button, input, form, table all individual files
- **Component hierarchy** - basic → composite → complex → layouts
- **Single responsibility** - one purpose per file, no duplicates
- **Simple naming conventions** - kebab-case, descriptive terms
- **Professional hierarchy** - logical folder structure
- **Zero code duplication** - each component exists once

### ✅ Enterprise-Grade Security
- **Zero-trust architecture** - validate all inputs
- **CSP v3 compliance** - no inline scripts
- **Encrypted storage** - secure sensitive data
- **Rate limiting** - prevent API abuse
- **Security event logging** - comprehensive monitoring

## 🚀 Rule Application

### Always Applied
- `chrome-extension-development.mdc` - Core standards for all files

### Auto-Attached (by file type)
- `ultra-modular-project-structure.mdc` - Triggers on `**/project-structure`, `**/architecture`
- `javascript-mjs-standards.mdc` - Triggers on `**/*.mjs`, `**/*.js`
- `html-css-ui-standards.mdc` - Triggers on `**/*.html`, `**/*.css`
- `security-permissions-standards.mdc` - Triggers on `**/manifest.json`, security files
- `testing-deployment-workflows.mdc` - Triggers on test files, build configs

### Manual Activation
Use `@rulename` in your prompts to specifically invoke rules:
- `@chrome-extension-development` - Core development guidance
- `@ultra-modular-project-structure` - Ultra-modular architecture guidance
- `@javascript-mjs-standards` - Modern JavaScript help
- `@html-css-ui-standards` - UI/styling assistance
- `@security-permissions-standards` - Security reviews
- `@testing-deployment-workflows` - Testing/deployment help

## 📋 **Rule Responsibilities**

| Rule File | Primary Focus | What It Covers |
|-----------|---------------|----------------|
| **chrome-extension-development** | Core Standards | Manifest V3, Chrome APIs, basic code standards |
| **ultra-modular-project-structure** | Architecture | File organization, component hierarchy, naming conventions |
| **javascript-mjs-standards** | JavaScript Code | ES2024+ features, patterns, performance |
| **html-css-ui-standards** | UI Development | HTML5, CSS3, responsive design, accessibility |  
| **security-permissions-standards** | Security | Permissions, validation, encryption, CSP |
| **testing-deployment-workflows** | Quality Assurance | Testing, CI/CD, store publishing |

## 🛠 Technology Stack

### Core Technologies
- **JavaScript**: ES2024+ features, .mjs modules
- **HTML**: HTML5 semantic elements, accessibility
- **CSS**: CSS3 Grid/Flexbox, Container queries, Custom properties
- **Chrome APIs**: Manifest V3, Service workers, Storage API

### Development Tools
- **Build**: Webpack 5, Babel
- **Testing**: Jest, Playwright, Chrome DevTools
- **Quality**: ESLint, Prettier, Security audits
- **CI/CD**: GitHub Actions, automated publishing

## 📋 Ultra-Modular Project Structure

```
chrome-extension/
├── manifest.json                    # Extension configuration
├── service-worker.mjs              # Main background worker
├── components/                     # UI Component Hierarchy
│   ├── basic/                      # Basic elements
│   │   ├── button.mjs             # Button component
│   │   ├── input.mjs              # Input field
│   │   ├── toggle.mjs             # Toggle switch
│   │   └── badge.mjs              # Badge component
│   ├── composite/                  # Composite components
│   │   ├── search-box.mjs         # Search input + button
│   │   ├── form-field.mjs         # Label + input + error
│   │   └── button-group.mjs       # Multiple buttons
│   └── complex/                    # Complex components
│       ├── header.mjs             # Page header
│       ├── footer.mjs             # Page footer
│       ├── table.mjs              # Data table
│       └── form.mjs               # Complete form
├── pages/                          # Extension pages
│   ├── popup/                      # Popup page files
│   └── options/                    # Options page files
├── services/                       # Business logic
│   ├── api/                        # API communication
│   ├── storage/                    # Data storage
│   ├── messaging/                  # Inter-script communication
│   └── security/                   # Security services
├── utils/                          # Utility functions
│   ├── dom/                        # DOM utilities
│   ├── data/                       # Data utilities
│   └── async/                      # Async utilities
└── styles/                         # CSS modules
    ├── components/                 # Component-specific styles
    └── themes/                     # Theme variations
```

## 🔧 Quick Start

1. **Initialize project structure** (rules will guide you)
2. **Create manifest.json** with Manifest V3 structure  
3. **Implement service worker** for background tasks
4. **Build popup/options UI** with modern HTML/CSS
5. **Add content scripts** for page interaction
6. **Set up testing** with Jest and Playwright
7. **Configure CI/CD** with GitHub Actions

## 🎯 Best Practices Enforced

### Development
- One feature per file, clear module boundaries
- Async/await patterns, no callback chains  
- Comprehensive error handling with custom error types
- TypeScript-style JSDoc documentation
- Performance-optimized code patterns

### Security  
- Minimal permissions principle
- Input validation and sanitization
- Secure message passing between scripts
- Encrypted storage for sensitive data
- CSP compliance, no inline code

### Quality
- 80%+ test coverage requirement
- ESLint + Prettier code formatting
- Security audits and dependency scanning
- Performance monitoring and optimization
- Accessibility compliance (WCAG)

## 📖 Usage Examples

### Creating ultra-modular Chrome extension:
```
Ask: "Create a new Chrome extension with @ultra-modular-project-structure for [your feature]"
```

### Building modular components:
```  
Ask: "@ultra-modular-project-structure Create button, input, and form components following component hierarchy"
```

### Security review:
```  
Ask: "@security-permissions-standards Review my manifest.json and content script security"
```

### Performance optimization:
```
Ask: "@javascript-mjs-standards Help optimize this service worker for better performance"
```

### Project structure guidance:
```
Ask: "@ultra-modular-project-structure How should I organize components for my extension feature?"
```

---

**Built for professional Chrome extension development with guaranteed working approaches and latest 2025 web standards.**
