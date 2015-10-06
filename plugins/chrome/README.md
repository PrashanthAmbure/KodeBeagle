# KodeBeagle chrome extension
This is a chrome browser extension, which helps users to search for code snippets from various open source repositories.
## Table of contents
* [Installation steps](#installation-steps)
    *  [From Github releases](#from-github-releases)
    *  [From chrome store](#from-chrome-store)
* [Using the chrome extension](#using-chrome-ext)
* [Developer notes](#dev-notes)
    * [Requirements.](#requirements)
    * [Loading unpacked extension.](#load-unpacked-ext)
    * [Packaging extension.](#packaging-ext)
    * [Updating extension.](#update-ext)
    * [Publishing extension.](#publish-ext)

<a id="installation-steps">
## Installation steps
<a>

<a id="from-github-releases">
#### From Github releases
<a>

1. Download the .crx file from the Github release or follow the steps on _"Packaging extension"_ below.
2. Open the chrome browser and type in - _**chrome://extensions**_. Drag and drop the .crx file on this page and it will instruct with a message as _**Drop to install**_,  now drop the extension.
![Chrome Ext](http://chrome-extension-downloader.com/images/chrome-extensions-drop.png)

<a id="from-chrome-store">
#### From Chrome store
<a>

- Soon the extension will be available in the chrome extensions factory for public use and once available we can install it from the factory directly.

<a id="using-chrome-ext">
## Using the chrome extension
<a>

Once the extension has been installed, it's time for us to make use of this extension.

1. Select either a collection of code phrases or a word on the browser window and right click, upon doing this we should see a context menu saying _**"Search this selection on KodeBeagle"**_

![](https://lh3.googleusercontent.com/HNIBPtvdWpnUmwLHDkx3tNDc7_po5GL226sSmF8nRZQ_IiQyKF5GPnb320HjLzxOjIJ88Uom2cTm1uIPJ3FP4zQ8RRl9TPtcIrRml3E7YG0dZAczloo3LrA6fG7jG22Mhm2_fGTW7hLIBwrJBz9D7IoJCrwWl3vdxU7TT9J4z3xDWgp0EZ02rPy6bxcVDPcL53IrBsMLUTqBfBgT3z-nabSNBpYDe9_Ar4DgIaqGygzOTkknmq9rl1TI1cnb7DKiSiz4RMdXSK2PwxRbPrDnGKn0wsFekmC9ye9MKOszvslMRsgQNlpvw8MTjGMC_bi9mqi2ug2xA0HD7jowRZFPoa3Y5aDyaTG8OP9HZBaE-kG7IyXvwZq6KGxqlus46FqhLe0ajWfgsGyqBZRjMm9DwCaoFA3hz2ru845aotFf0jbNcunkfvGYOPrJQXFDa6og49PoYJ4gr9IQlDZu6-P-dKByM8wUFEd1u0FwLDRDCxt00LRcvT7Rhdkls3c75wzq34YgMEpQ9pUPTGaHBGryf4j15spfh_16i81nmHnxIWI=w1354-h447-no)
2. And a new tab opens up which lists out the code snippets for the selection from various repositories.

![](https://lh3.googleusercontent.com/LkB9nZEeptja6p3odjO4bqsWI71qYHIduo0lrspPNhE4qPrAHNNetzZ-3ovhjoPWFVEC0v_wE0THlvovmzSBD71ZLkabM1-7kj7vpaVER6_wKgyiPXkF8kFOnSj_Cu77keGwXiMtusqvwNJ0zCsUDG9CK1dYYONyiXRvqKSYrs9eYpg8H6QBPRjWBI1VjnsRQhxpOjKHkRl9PZFqzZF4WvdCahBRCUUM-mEQs326FaMu6IQRGxHU_l1X_rFeTYgXXR2RdnWL0y2B_YOabMASI0stlzYOBOD42C3260aV7bQwIjjPxuvdLR7b-mpmS4QCjPvV02_tD7nYWObEHxIQWSYsmzMWTK39jfaq2qPvja_e2GVTxXx56kOM9kuaDb0ATyy3qpKcOyqIAX-tGyX0gB-JTQp-Piyj02cKw_cQPXkUqZyH_5UBn-Cda0PCZd-kw-PiaQSaFI2Oa7IljFi09_lKHhcE78a34WghHXNjQ-Zm_1fj8cMNYD0zgS96VBe64OWmuMHvv766grXoSn6XSiLfzqIpRQVd9d2OGS6o4Hs=w1227-h655-no)

<a id="dev-notes">
## Developer notes
<a>

<a id="requirements">
### Requirements
<a>

* [NodeJS & NPM](http://nodejs.org/download)
* _gulp_ node package
* chrome browser

<a id="load-unpacked-ext">
### Loading unpacked extension.
<a>

1. Open the chrome browser and type in - _**chrome://extensions**_.
2. Ensure that the _"Developer mode"_ checkbox in the top right-hand corner is checked.
3. Click on _'Load unpacked extension'_ and choose the _src_ folder from the repo. Once the folder is uploaded we should be seeing something similar to below snap.
![](https://lh3.googleusercontent.com/VGS2HACIXedEZAt_aFWAe9okP3eQi0KvOlrVo-5WzERhMiD4C7lTY6qAwxn8BaC0SWuU2V87COGVhmMaDoNZ7wzxS8ujVRtvu_LsqO9Lzgq7Ceta3RU-613fn5pG_6bxlAGhuiWCZJIJCkq-V1IW1VFZVcBsbbAksN4o-Im0LQCe5AsfuRgariVNskfksywbbie0qIjdJrPTeSU3OhN2ltfi5NRXb9Lv5M53biYgPgBbqUB5rwcDE_h2Y0wDI-GZOwEYUZYbe6anqWjknsypb9uUjdFrEc1EtWj5mm2cUomu-6Fnb7_UT8fkkfvXmKGaS6nAE2rdbgTqbjCp8ML1uo4v9oAf6wh9BFhjl3DyHg90H4afJ_B9QX1T9ELpaSdK8EhH5v7nFL9tol2Umal-qvbGoYzptFIe0BnRr0M6BMEor5FnxkXPihBTu-SrHKTBmNrQj8FFf_i5Fvx9fz2KPyL_PMYSMIYNDq37nqLFEdtSo7lUJplGU5NXxxNdcW93Pn-x_KWysRtihEzqXLKcgd6YDNsHAbZpm95VlFa4RbQ=w988-h455-no)
4. We're now ready to debug the extension code, to do so, open the _**backgroundpage**_ from the chrome extensions page and setup the breakpoints.  

<a id="packaging-ext">
### Packaging extension.
<a>

> This section is relevant only for the following three reasons...              
> 1 - Either the crx file is not available on the Github,   
> 2 - Or we would like to update the extension,     
> 3 - Or upload the extension to the chrome web store  
> **Note:** For #2 and #3 we will be using the same pem file.

Once the extension code gets stable, its time to create the .crx file which can be published to chrome extension factory for public use. Please note that chrome extensions are packaged as signed zip files with the file extension as _"crx"_.
**Note:** We package our own extension to distribute a non-public version.
1. Get the _.pem_ file from **_project leads_** and copy it to the root directory of the extension and do not change the .pem file name.
2. Open the terminal and execute _**sudo npm install**_ command which would download all the required node module dependencies mentioned in _package.json_.
3. Now run the gulp task using the following command - _**gulp create:crx**_. This command creates a .crx file under build directory .
4. Open the chrome browser and type in - _**chrome://extensions**_. Drag and drop the .crx file on this page and it will instruct with a message as _**Drop to install**_, now drop the extension.
![Chrome Ext](http://chrome-extension-downloader.com/images/chrome-extensions-drop.png)

<a id="updating-ext">
### Updating an extension
<a>

To create an updated version of your extension:
1. Increase the version number in manifest.json.
2. Follow the steps from _Packaging extension_

<a id="publish-ext">
### Publishing an extension
<a>

[Click here](https://developer.chrome.com/webstore/publish) to publish chrome extension.

Alternatively, please follow the steps in the below YouTube video.

[![Image](http://img.youtube.com/vi/Gn_jlvkHTnM/0.jpg)](https://www.youtube.com/watch?v=Gn_jlvkHTnM)
