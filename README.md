TaracotJS
=========

TaracotJS is fast and minimalist CMS based on Node.js. It has the following features:

 - MongoDB as a database storage and Redis for session storage - for maximum perfomance
 - Independent Module structure
 - Multilanguage support out of the box
 - Multifunctional file browser with drag-and-drop and Zip/Unzip support
 - Built-in website statistics
 - WYSIWYG-based page editor (based on CKEditor)
 - Crossplatfrom - works everywhere where Node.JS does
 - And many more 8-)

Official website: https://taracot.org

## Demo

Please take a look at the demo installation instance: https://demo.taracot.org/cp (use admin as username and admin as password).

Note: the demo is automatically re-installing every hour.

## Installation guide

Follow this guide for TaracotJS instance installation.

### Pre-requisites

Download and install Node.js for your operating system: http://nodejs.org/download/. Node Package Manager (npm) should be installed by default; if not, please take care of it's installation.

MongoDB and Redis are required. If your operating system is x64-based Windows, you may download the pre-compiled MongoDB and Redis here: https://taracot.org/source/db/mongo_redis_win64.zip. Unzip the files included to any folder on your hard disk and start using start.cmd. Two minimized console applications will be started, they should remain open every time you run TaracotJS server. For Linux/UNIX and MacOS-based operating systems you may install the corresponding MongoDB and Redis packages manually or compile from sources.

### Quick Start

The quickest way to get started with TaracotJS is to utilize the executable taracotjs to generate an application as shown below.

1. Install taracotjs-generator:

  ```npm install -g taracotjs-generator```

2. Create Taracot JS instance:

  ```taracotjs /tmp/foo && cd /tmp/foo```

3. Install dependencies:

  ```npm install```

4. Edit config.js (using your favorite text editor), don't forget to set MongoDB connection URL and Redis port. You don't have to edit secrets and salt at this point, they will be auto-generated on the next step.

5. Perform system post-configuration:

  ```cd bin && node install-system && node install-modules```

6. Rock and Roll:

  ```node webserver```

If everything goes well, you will see the following message: “TaracotJS server listening on port: 3000” (3000 is the default port). Open up your favorite browser and open the following page: http://127.0.0.1:3000/.

Control panel is accessible via http://127.0.0.1:3000/cp/. Default username is admin, default password is admin.

### Manual installation

Github repository is available at: https://github.com/xtremespb/taracotjs. Use Git to checkout. Then follow the instructions provided above beginning from “Install dependencies” step.

## Documentation

Please visit https://wiki.taracot.org/ for more information on this project.

## License

Copyright (c) 2014-2015 Michael A. Matveev (<xtreme@rh1.ru>)

This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details: http://www.gnu.org/copyleft/gpl.html.
