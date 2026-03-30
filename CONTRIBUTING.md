# Contributing

Contributions to this project are [released](https://help.github.com/articles/github-terms-of-service/#6-contributions-under-repository-license) to the public under the [project's open source license](LICENSE).

Everyone is welcome to contribute to this project. Contributing doesn't just mean submitting pull requests—there are many different ways for you to get involved, including answering questions, reporting issues, improving documentation, or suggesting new packages.

## How to Contribute

### Reporting Issues

If you find a bug or have a suggestion:
1. Check if the issue already exists in the GitHub Issues
2. If not, create a new issue with:
   - Clear title and description
   - Steps to reproduce (for bugs)
   - Expected vs actual behavior
   - Your environment details (OS, Node version, npm/pnpm version)

### Submitting Pull Requests

1. Fork the repository
2. Create a new branch for your feature/fix:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Make your changes following the guidelines below
4. Test your changes thoroughly
5. Commit with clear, descriptive messages
6. Push to your fork and submit a pull request

### Package Management Guidelines

When adding or updating packages:

1. **Research thoroughly**: Ensure the package is:
   - Actively maintained
   - Widely used in the community
   - Has good documentation
   - Follows security best practices
   - Has a stable release history

2. **Version management**:
   - Use caret (`^`) for minor version updates
   - Verify compatibility with existing packages
   - Check for breaking changes in release notes

3. **Security**:
   - Run `npm audit` or `pnpm audit` after adding packages
   - Check for known vulnerabilities
   - Prefer packages with active security maintenance

4. **Testing**:
   - Test that the package installs correctly
   - Verify no dependency conflicts
   - Document any special installation requirements

### Adding New Packages

When proposing a new package:

1. Explain why it should be included
2. Provide package statistics (downloads, stars, maintenance status)
3. Ensure it fits one of these categories:
   - Web frameworks
   - Testing frameworks
   - Security utilities
   - Validation libraries
   - CLI tools
   - Build tools
   - HTTP clients
   - Database clients
   - Utility libraries
   - Logging frameworks

### Updating Existing Packages

When updating package versions:

1. Review the changelog for breaking changes
2. Update to the latest stable version when possible
3. Note any breaking changes in your PR description
4. Test for conflicts with other packages

### Code Style Guidelines

This project maintains simplicity:
- Keep `package.json` clean and well-organized
- Group similar packages by category in documentation
- Use consistent formatting
- Document any special considerations

Before submitting:
```bash
# Install/update dependencies
npm install
# or
pnpm install

# Test installation
node index.js
```

## Questions or Need Help?

Please feel free to contact me with any question, comment, pull-request, issue, or any other thing you have in mind.

* Or Assayag <orassayag@gmail.com>
* GitHub: https://github.com/orassayag
* StackOverflow: https://stackoverflow.com/users/4442606/or-assayag?tab=profile
* LinkedIn: https://linkedin.com/in/orassayag

Thank you for contributing! 🙏
