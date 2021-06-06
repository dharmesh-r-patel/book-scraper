Warning: The ethics and legality of web scraping are very complex and constantly evolving. They also differ based on your location, the data’s location, and the website in question. This tutorial scrapes a special website, books.toscrape.com, which was specifically designed to test scraper applications. Scraping any other domain falls outside the scope of this tutorial.

Prerequisites
Node.js installed on your development machine. This tutorial was tested on Node.js version 12.18.3 and npm version 6.14.6. You can follow this guide to install Node.js on macOS or Ubuntu 18.04, or you can follow this guide to install Node.js on Ubuntu 18.04 using a PPA.

On Linux machines, Puppeteer might require some additional dependencies.

If you are using Ubuntu 18.04, check the ‘Debian Dependencies’ dropdown inside the 'Chrome headless doesn’t launch on UNIX’ section of Puppeteer’s troubleshooting docs. You can use the following command to help find any missing dependencies:

$ ldd chrome | grep not

- headless - false means the browser will run with an Interface so you can watch your script execute, while true means the browser will run in headless mode. Note well, however, that if you want to deploy your scraper to the cloud, set headless back to true. Most virtual machines are headless and do not include a user interface, and hence can only run the browser in headless mode. Puppeteer also includes a headful mode, but that should be used solely for testing purposes.
- ignoreHTTPSErrors - true allows you to visit websites that aren’t hosted over a secure HTTPS protocol and ignore any HTTPS-related errors.

npm install

npm start
