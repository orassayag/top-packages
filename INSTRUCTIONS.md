# Setup and Usage Instructions

## Table of Contents

1. [Prerequisites](#prerequisites)
2. [Initial Setup](#initial-setup)
3. [Available Commands](#available-commands)
4. [Package Categories](#package-categories)
5. [Usage](#usage)
6. [Extending the Application](#extending-the-application)
7. [Best Practices](#best-practices)
8. [Troubleshooting](#troubleshooting)
9. [External Resources](#external-resources)

## Prerequisites

### System Requirements

- **Node.js**: Version 20.0.0 or higher
- **Package Manager**: pnpm (recommended) or npm
- **Operating System**: macOS, Linux, or Windows
- **Memory**: 1GB RAM minimum
- **Disk Space**: 200MB for application and dependencies

## Initial Setup

### 1. Install Dependencies

**Using pnpm (recommended):**

```bash
pnpm install
```

**Using npm:**

```bash
npm install
```

## Available Commands

### Development Commands

**Linting and Formatting:**

```bash
# Check code style and quality
npm run lint

# Format all files
npm run format
```

**Security Audits:**

```bash
# Run security audit
npm audit
```

### Running Scripts

**Check for Updates:**

```bash
# List outdated packages
npm outdated
```

**Update Packages:**

```bash
# Update all dependencies
npm update
```

## Package Categories

This project includes popular npm packages organized by category:

### Web Frameworks

- **Express** (v5.2.1) - Fast, unopinionated web framework
- **Fastify** (v5.7.4) - High-performance web framework
- **Socket.io** (v4.8.3) - Real-time bidirectional communication

### Testing Frameworks

- **Jest** (v30.2.0) - JavaScript testing framework
- **Mocha** (v11.7.5) - Feature-rich test framework
- **Chai** (v6.2.2) - BDD/TDD assertion library
- **Sinon** (v21.0.1) - Test spies, stubs, and mocks
- **Supertest** (v7.2.2) - HTTP assertions
- **Karma** (v6.4.4) - Test runner

### Security & Authentication

- **Bcrypt** (v6.0.0) - Password hashing
- **Passport** (v0.7.0) - Authentication middleware
- **Passport-jwt** (v4.0.1) - JWT authentication strategy
- **Jsonwebtoken** (v9.0.3) - JWT implementation
- **Express-jwt** (v8.5.1) - JWT middleware for Express

### Validation Libraries

- **Joi** (v18.0.2) - Schema validation
- **Yup** (v1.7.1) - Schema validation and value parsing
- **Ajv** (v8.18.0) - JSON Schema validator
- **Validator** (v13.15.26) - String validation and sanitization

### Utilities

- **Lodash** (via underscore v1.13.8) - Utility functions
- **Async** (v3.2.6) - Async utilities
- **Bluebird** (v3.7.2) - Promise library
- **Moment** (v2.30.1) - Date manipulation
- **Uuid** (v13.0.0) - UUID generation
- **Nanoid** (v5.1.6) - Unique ID generator

### HTTP Clients

- **Axios** (v1.13.6) - Promise-based HTTP client
- **Superagent** (v10.3.0) - HTTP request library
- **Centra** (v2.7.0) - Lightweight HTTP client

### CLI Tools

- **Commander** (v14.0.3) - Command-line interfaces
- **Chalk** (v5.6.2) - Terminal string styling
- **Inquirer** (via similar tools) - Interactive CLI prompts

### Build & Development Tools

- **Nodemon** (v3.1.14) - Auto-restart during development
- **PM2** (v6.0.14) - Process manager
- **Cross-env** (v10.1.0) - Cross-platform environment variables
- **Grunt** (v1.6.1) - Task runner
- **Rimraf** (v6.1.3) - Cross-platform rm -rf

### Logging

- **Winston** (v3.19.0) - Logging library
- **Morgan** (v1.10.1) - HTTP request logger
- **Pino** (v10.3.1) - Fast JSON logger

### Database

- **Mongoose** (v9.2.3) - MongoDB ODM

### File System & Parsing

- **Fs-extra** (v11.3.4) - Enhanced file system methods
- **Cheerio** (v1.2.0) - HTML parsing
- **Dotenv** (v17.3.1) - Environment variable loader

### Miscellaneous

- **Color** (v5.0.3) - Color manipulation
- **Slugify** (v1.6.6) - URL-friendly strings
- **Anymatch** (v3.1.3) - File matching
- **Cors** (v2.8.6) - CORS middleware
- **Pug** (v3.0.3) - Template engine

## Usage

This project serves as:

1. **Reference Collection**: Quick reference for popular package versions
2. **Starter Template**: Base dependencies for new projects
3. **Learning Resource**: Explore widely-used npm packages
4. **Version Tracking**: Track compatible versions of popular packages

### Using as a Template

Copy the packages you need from `package.json`:

```bash
# Install specific packages from this collection
npm install express joi bcrypt
```

### Exploring Packages

Check individual package documentation:

```bash
# View package info
npm info express
npm info joi
```

## Extending the Application

To add new packages to the collection:

1. Run `pnpm add <package-name>`
2. Update the category lists in `README.md` and `INSTRUCTIONS.md`
3. Add a brief description of the package's purpose
4. Commit and push your changes

## Best Practices

- **Selective Use**: Only use the packages that are necessary for your specific project requirements.
- **Lock Files**: Always commit your lock files (`package-lock.json` or `pnpm-lock.yaml`) to ensure consistent environments.
- **Security First**: Regularly run `npm audit` and address any critical vulnerabilities immediately.
- **Minimal Dependencies**: Aim for a lean dependency tree to reduce security surface area and bundle size.

## Troubleshooting

### Common Issues

**Problem**: Dependency conflicts after updating.
**Solution**: Delete `node_modules` and the lockfile, then run `pnpm install` or `npm install` again.

**Problem**: Node version mismatch.
**Solution**: Ensure you are using Node.js v20 or higher. You can use `nvm use 20` if you have Node Version Manager installed.

**Problem**: Script execution errors.
**Solution**: Verify that all peer dependencies are correctly installed and that the package version is compatible with your environment.

## Package Selection Criteria

Packages included in this collection meet these criteria:

1. **Popularity**: High download counts and community adoption
2. **Maintenance**: Active development and regular updates
3. **Stability**: Stable API and semantic versioning
4. **Documentation**: Well-documented with examples
5. **Security**: Active security maintenance and vulnerability fixes
6. **Purpose**: Serves a common development need

## Version Management

The project uses:

- **Caret (`^`)** for most dependencies - allows minor and patch updates
- Tested combinations to avoid conflicts
- Regular updates for security patches

To update packages:

```bash
# Check for outdated packages
npm outdated

# Update all packages
npm update

# Or with pnpm
pnpm update
```

## Security

Run security audits regularly:

```bash
npm audit

# Or with pnpm
pnpm audit
```

Fix vulnerabilities:

```bash
npm audit fix

# Or with pnpm
pnpm audit fix
```

## Notes

- All packages are installed as dependencies (not devDependencies)
- This is a reference collection; production projects should only install needed packages
- Check individual package documentation for usage instructions
- Verify license compatibility for your use case
- Test thoroughly when using in production

## External Resources

- [npm Documentation](https://docs.npmjs.com/)
- [Node.js Documentation](https://nodejs.org/docs/)
- [pnpm Documentation](https://pnpm.io/)
- [Security Best Practices for npm](https://docs.npmjs.com/security-best-practices)

## Author

- **Or Assayag** - _Initial work_ - [orassayag](https://github.com/orassayag)
- Or Assayag <orassayag@gmail.com>
- GitHub: https://github.com/orassayag
- StackOverflow: https://stackoverflow.com/users/4442606/or-assayag?tab=profile
- LinkedIn: https://linkedin.com/in/orassayag

## Last Updated

May 2026
