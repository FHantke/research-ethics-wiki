# Research Ethics Wiki

A comprehensive collection of information regarding research ethics in computer security and privacy research.

## About

This wiki provides researchers, practitioners, and students with resources for understanding and navigating the ethical considerations inherent in conducting security and privacy research. It covers topics such as ethical frameworks, IRB processes, informed consent, vulnerability disclosure, data privacy, and publication ethics.

## Build Process

### Build locally

1. Install the [Hugo Framework](https://gohugo.io/getting-started/installing/) **extended** version (>= 0.68)
2. Clone this repository
3. Initialize and update the theme submodule: `git submodule update --init --recursive`
4. Run `hugo server --minify` in the root directory
5. Open your browser and go to http://localhost:1313 (or as indicated by hugo output)

### Generate static files

1. Run `hugo --minify` to build the static site
2. The generated files will be in the `public/` directory

## Automatic Deployment

This repository uses [GitHub Actions](https://github.com/features/actions) to automatically build and publish a static version of the Research Ethics Wiki once a Pull Request is merged to the main branch. The site is deployed to GitHub Pages.

## Contributing

Contributions are welcome! Whether you want to add new content, improve existing pages, or fix issues, please feel free to:

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

For major changes, please open an issue first to discuss what you would like to change.

## License

This project is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details.
