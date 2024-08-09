# TypeScript Project Starter Template

Starter template for TypeScript projects. It comes pre-configured with the following features:

- **TypeScript**: TypeScript to allow you to write type-safe code efficiently.
- **ESLint**: ESLint to enforce code quality and consistency.
- **Prettier**: Prettier to format your code automatically and ensure consistent code style.
- **Jest**: Jest to run your tests and ensure your code works as expected.
- **SWC**: For faster and more efficient TypeScript compilation.
- **PNPM**: PNPM to manage your dependencies efficiently.
- **GitHub Actions**: GitHub Actions to run your tests and lint your code automatically on every push.

## Getting Started

Simply, clone the TypeScript Project Starter Template to get started.

```bash copy
git clone https://github.com/pranav-kural/typescript-project-starter-template.git
```

### Install Dependencies

Install the dependencies using PNPM:

```bash copy
pnpm install
```

### Compile Code

Use SWC to compile your TypeScript code:

```bash copy
pnpm build
```

Pre-configured to output the compiled code to the `lib` directory.

### Run the Code

Run the compiled code:

```bash copy
pnpm start
```

Pre-configured to run the `index.js` file in the `lib` directory.

### Development

You can also use the `dev` script instead when making changes to the source code. This script will compile your code and run it in watch mode:

```bash copy
pnpm dev
```

Pre-configured to watch the `src` directory for changes and recompile the code automatically. Please that this uses `tsx` and not `swc` for compilation.

### Testing

Pre-configured with Jest to run your tests. You can run the tests using the following command:

```bash copy
pnpm test
```

By default, Jest is configured to look for tests in `src/tests` directory. You can change the configuration in the `jest.config.js` file, along with any other Jest configurations you may want to change.

### Linting

Pre-configured with ESLint to enforce code quality and consistency. You can run ESLint using the following command:

```bash copy
pnpm lint
```

### Formatting

Pre-configured with Prettier to format your code automatically. You can run Prettier using the following command:

```bash copy
pnpm format
```

### Pre-deploy Workflow

An npm script `predeploy` is defined the `package.json` file to run the following in sequence:

1. `lint`: Run ESLint to enforce code quality and consistency.
2. `format`: Run Prettier to format your code automatically.
3. `build`: Compile your TypeScript code using SWC.
4. `test`: Run Jest to ensure your code works as expected.

```bash copy
pnpm predeploy
```

### GitHub Actions

Pre-configured with GitHub Actions to run your tests and lint your code automatically on every push. You can find the workflow configuration in the `.github/workflows` directory. Also, includes setup for dependabot to keep your dependencies up-to-date. Please note that, you may need to enable dependabot in your repository settings. Learn more about [Dependabot](https://docs.github.com/en/code-security/getting-started/dependabot-quickstart-guide).

## Git Setup

After cloning the repository, you can update the remote URL to point to your repository, or remove the existing git commit history and start fresh.

Update the remote URL to point to your repository:

```bash copy
git remote set-url origin
```

Remove the existing git commit history and start fresh:

```bash copy
rm -rf .git
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin <your-repository-url>
git push -u origin main
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Issues

If you encounter any issues or bugs while using QvikChat, please report them by following these steps:

1. Check if the issue has already been reported by searching our issue tracker.
2. If the issue hasn't been reported, create a new issue and provide a detailed description of the problem.
3. Include steps to reproduce the issue and any relevant error messages or screenshots.

[Open Issue](https://github.com/oconva/qvikchat/issues)

```

```
