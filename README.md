# PWA-CodeJournal

## Description
a sophisticated, browser-based text editing application that provides developers with the convenience of creating and managing notes and code snippets, even without an internet connection.


## Table of Contents 
- [Installation](#installation)
- [Dependencies](#dependencies)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Questions](#questions)
  
## Installation 
There is no installation necessary for this application as it is deployed using [Render](https://docs.render.com/). You can access and use the application [here](https://pwa-codejournal.onrender.com/) or at the following link: https://pwa-codejournal.onrender.com/

If you are interested in running the application locally, please use the following steps:
1. Clone this repository to your local machine. (For reference, visit the [Cloning a Repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository) GitHub Docs article.)
2. Run `npm install && npm run build` in your CLI to download the npm package dependencies.
3. Run `npm run start` to start up the backend and serve the client.
4. Navigate to `http://localhost:3000` on your local web browser to use the application. 
  
## Dependencies
This project requires the following npm package dependencies, which are included in `client/package.json`:  

![Package dependencies](Assets/pwa-dependencies.png)

## Usage 

### Getting Started
Upon accessing the [text editor](https://pwa-text-editor-xj19.onrender.com/), `IndexedDB` will immediately create a database storage and the user will be presented with the main page, depicted below.  

![Main Page](Assets/JATE-landing.png)

When navigating to Chrome DevTools, you'll see the app details for the registered service worker, manfifest file, and pre-cached static assets. 

![Service worker](Assets/devtools-service.png)
![Manifest file](Assets/devtools-manifest.png)
![Pre-cached static assets](Assets/devtools-cache.png)

### Updating Content
After writing some content and clicking off of the DOM window, the new content is updated in the database storage. You will find that the content data persists after closing and reopening the application by re-rendering the value saved in `IndexedDB`.  

![Put content](Assets/devtools-put.png)

### Installing a Desktop Shortcut
As a PWA, this text editor supports installation so that it can be saved to your local desktop. By pressing the Install button, J.A.T.E. will be downloaded as a Chrome App and can be accessed directly as a desktop shortcut. 

![Install button](Assets/install-button.png)
![J.A.T.E. installed to desktop](Assets/JATE-shortcut.png)

## Contributing
To make contributions to this project:  
1. Fork the repository  
2. Make some commits to improve the application
3. Open a Pull Request on GitHub
4. From there, we can discuss your changes and merge the pull request once your contributions have been approved!

## License 
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
- This GitHub repository is licensed under the MIT license. Please refer to the license documentation [here](https://opensource.org/licenses/MIT).
  
## Questions
This project was developed by [Domj1204](https://github.com/DomJ1204).  
For any related questions, please contact me via email at <jenningsdomonic@gmail.com>.