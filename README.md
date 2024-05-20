## Overview

Overview

This project is a Chrome extension designed to provide users with real-time statistics on a specific topic. It centralizes data from various sources and displays it in an easily digestible and accessible format directly within the browser.

##
## Features

Features

- **Real-Time Statistics**: Fetch and display the most up-to-date statistics.
- **User Request History**: Keep track of the last three user requests.
- **Accordion View**: Clean and organized display of statistical data using an accordion view.
- **Dynamic Data Handling**: Efficiently process and manage data for global statistics.

##
## Installation Instructions

Installation Instructions

Follow these steps to install and set up the Chrome extension:

1. **Clone the Repository**: Open your terminal and run the following command to clone the repository:
   ```sh
   git clone https://github.com/m-seamew/chromeExtension.git
   ```

2. **Navigate to the Project Directory**:
   ```sh
   cd chromeExtension
   ```

3. **Load the Extension in Chrome**:
   - Open Google Chrome and navigate to `chrome://extensions/`.
   - Enable "Developer mode" by toggling the switch in the top right corner.
   - Click on the "Load unpacked" button and select the cloned project directory.

4. **Verify Installation**: The extension should now appear in your Chrome extensions list. You can pin it to your toolbar for easy access.

##
## Usage Examples

Usage Examples

Once the extension is installed, here's how you can use it:

1. **Open the Extension**: Click on the extension icon in the toolbar.
2. **View Statistics**: The main view will display real-time global statistics.
3. **Access Accordion View**: Click on the different sections of the accordion to view detailed information.
4. **User Request History**: The extension keeps track of the last three requests made by the user, which can be reviewed in the history section.

##
## Code Summary

Code Summary

### File Structure

- **background.js**: Contains the logic for background processes required by the extension.
- **content.js**: Handles dynamic content scripts that are injected into web pages.
- **main.js**:
  - **Global Variables**:
    - `arr`: General-purpose array.
    - `allWorldStat`: Array for storing world statistics.
    - `database`: Array holding data about the current situation in all countries from requests.
    - `clientArr`: Array to save the last three client requests.
    - `maxid`: Counter for creating unique IDs in `clientArr`.
    - `accordionField`: Node list array for managing accordion views.
  - **Functions**:
    - `request()`: Initiates the app and starts the data fetching process.

### Key Files

- **background.js**: Runs in the background to manage persistent operations.
- **content.js**: Script injected into web pages to manipulate DOM or interact with webpage content.
- **main.js**: Core script that initializes app logic, makes data requests, and manages global statistics.

##
## License

License

This project is licensed under the MIT License. For more details, please refer to the LICENSE file in the repository.

```

Feel free to clone the repository and get started with exploring and enhancing the project. Your contributions and feedback are welcome!
```