# Node-Config-Loader
## Prerequisites
This is a configuration manager for Node.js so that you can load different environments by startup parameters or environment variables.

## Installation
* Drag and drop the config folder to the root directory of your project

## Usage
### Setting the environment on startup
You are able to set the loaded config file on startup of the node script:

    node index.js dev  // Loads app_dev.json
    node index.js test // Loads app_test.json

You can also use an export variable:

    export NODE_ENV test // Loads app_test.json on node index.js
    export NODE_ENV dev  // Loads app_dev.json on node index.js

The default environment being loaded is app_dev.json

### In Code
just run the require line that points towards the config folder:

    var config = require(process.cwd() + '/config');
