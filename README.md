# Working with an AcademicPages Site

This is a personal academic site based on [AcademicPages](https://github.com/academicpages/academicpages.github.io).
After forking AcademicPages, here are some notes on setting up for site development on Windows.
Changes are made locally, with a live preview, and then published to GitHub.


---

## Tools/Installation

- Install [GitHub Desktop](https://desktop.github.com) – for updating GitHub from the local project copy.
- Install [Visual Studio Code (VSCode)](https://code.visualstudio.com) – for editing content of the local copy.
- Install [RubyInstaller](https://rubyinstaller.org) + Jekyll – to build and preview the site locally before publishing to GitHub.
  - Run RubyInstaller, selecting:
    - Add Ruby to PATH
    - Run `ridk install`
  - Install Jekyll and Bundler (in the command prompt):
    ```sh
    gem install jekyll bundler
    ```
  - Install site dependencies (in the command prompt):
    ```sh
    cd path\to\your-username.github.io
    bundle install
    ```

---

## Preview the Site Locally

1. Build and serve the site (in the command prompt):
   ```sh
   cd path\to\your-username.github.io
   bundle exec jekyll serve
   ```
2. Open/Preview the site in a browser (changes reflected in real-time):
   ```
   http://127.0.0.1:4000
   ```
