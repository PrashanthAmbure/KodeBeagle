# KodeBeagle chrome extension
This is a chrome browser extension, which helps users to search for code snippets from various open source repositories.
## Table of contents
* Installation steps
    *  From Github releases
    *  From chrome store
* Using the chrome extension
* Developer notes
    * Requirements.
    * Loading unpacked extension.
    * Packaging extension.
    * Updating extension.
    * Publishing extension.

## Installation steps
#### From Github releases
1. Download the .crx file from the Github release or follow the steps on _"Packaging extension"_ below.
2. Open the chrome browser and type in - _**chrome://extensions**_. Drag and drop the .crx file on this page and it will instruct with a message as _**Drop to install**_,  now drop the extension.
![Chrome Ext](http://chrome-extension-downloader.com/images/chrome-extensions-drop.png)

#### From Chrome store
- Soon the extension will be available in the chrome extensions factory for public use and once available we can install it from the factory directly.

## Using the chrome extension
Once the extension has been installed, it's time for us to make use of this extension.

1. Select either a collection of code phrases or a word on the browser windown and right click, upon doing this we should see a context menu saying _**"Search this selection on KodeBeagle"**_

![](https://lh3.googleusercontent.com/VIVI2nE10YGgJsKiCY-Ac_5BI9K9ikomSbZ325Q_yLpfKpRulQtB_WLOvXx7D2hhVyzNLD1yRlEvs3RnY9dBhlJLtj8XryOacUSQwTofiqTwZ7JLNgKo4-BVt-JdviAOmLFNitOOnDKjFtviM37DQmYUCcXpYdHwqFn1NlV23ugqxrfP6zSb8hXoDA1Kot2wM2B0yhEfGG58eS49bqyAvkFb238loIVGgsXbQuhY-eoNsOOu0L9OZhstx2Y217x9f8IsQDcTevC3R0pM5Lq-h5L2moi9V6r2L4LF6iYLP0PhLhG5YEdFiSvUueaUwZa2tD4PuPbdr1th5sPTlX-FxNALQXug9IShzjnIW6_5zZSZB5ImDEUxwt1v0Furoe1N52TGyH_KLe0gJccxWpZNV-yG9wFX0PdEYQpfqPtGhmfM8Z1bc2-z577YWiD561JFT4GNqdDEddrkaI1g4L5mVvO-tK7kxpiBqIbpln9wIXYUqfXLb9KaMrv6qKBJ_6FTVIxl8em9qLA9S6m-_rLe69yxYUn_j30F_2wiGE_lCdE=w1354-h447-no)
2. And a new tab opens up which lists out the code snippets for the selection from various repositories.

![](https://lh3.googleusercontent.com/fF8uuEASxzulF94sLk8uhNVpvkaQUIBD-GdxPgucC-5smOSWh25oCPeNpMlVymgPZeudRTAz-G7bDbQ_4OSySTbwOKeNKIJ7mrvJXWsMZenitsiHvoYSBl69h85mRd3933AgR51QB2Rskj1yTPruiJe7i1a3IyEo68ASW5czsKfWYv1kta3xgURh098fYk8lfCXU140ye1Jb7vcLAsKJZK272RJEXiMDQjq8qHHlhk5fq-GQ2l1OT4-3e3YX1wjd1OckLK8-QZvUQzrsd0BIQaHbPaQ-O_Ry4q6hBERcx32OXi1sMzx_8RmxRDLOVzBqMrFp18nX-RUYy6rFKwAt0qTBZnnn4BVl7tZ3s2fCZwF0qzTSZi86FCcLjrRrgVijWt1_NCquhuuzBV-DsLr5Hgbdd4zfR_tqJpKtw1eZ_z-Ln7_LqpdO9ZKlpsPHfkt2H94jIY16G6mypV1g6o12QDdQrKk3cE396T3p2m3FAiwqjuS0Ki90oA1hbOP-hs4HxWeDu6J2wioj7mD1RMifKoBN-sJTthBDSazXpWbKzDI=w1227-h655-no)

## Developer notes
### Requirements
* [NodeJS & NPM](http://nodejs.org/download)
* _gulp_ node package
* chrome browser

### Loading unpacked extension.
1. Open the chrome browser and type in - _**chrome://extensions**_.
2. Ensure that the _"Developer mode"_ checkbox in the top right-hand corner is checked.
3. Click on _'Load unpacked extension'_ and choose the _src_ folder from the repo. Once the folder is uploaded we should be seeing something similar to below snap.
![](https://lh3.googleusercontent.com/pe9mdfq9KBT03E-9XBbY5zkG8ONbK9WpovNqdbEYqbihDY7iSgW4IYjcROeg4JLhwpAvf0W--PUEWjLD_i1O3yhfS0PfPjLgabTLdfkAW2Dwqu0SyGSWvq7wOWrJWYaOHQ_9_VDWMOgcDqZ9rTkgGRcr9yUMYoceNoXU5qmll1iyZuYb6gDJ9-6fN2TycTKuiyi_IEFmeHtSa8xlfxzqCBTT5I6WVMbWMqnNlaZb9oYnKtZ4rYB41gFbUMEEiI9hMN_9yuBSaKHT16iajZpmrhzx8nbqedRBdIVON0NwIPRdrDNr36FHp21Z7Q7evxhCFHHyy-yu3I55XMh6Lz36-Om7mhn5-7PJcwScI9kBngYnZElJCbNvXb1nt0kvol7OxLBy_9rMXPMnS1rMzD-aFz5QOX1vEfLuimc0c0u9EB7KswKJlrTDqLb2_PMj8iEaeDf2cSl5BQ0m_JXmgIV60-EOYIJctU8CfFSWXKVY107slf6scrqFgyTlj2oHU-bWa2JDw74fAhP7sruaL3PlFGZSBC7c=s988-w988-h455-no)
4. We're now ready to debug the extension code, to do so, open the _**backgroundpage**_ from the chrome extensions page and setup the breakpoints.  

### Packaging extension.
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

### Updating an extension
To create an updated version of your extension:
1. Increase the version number in manifest.json.
2. Follow the steps from _Packaging extension_

### Publishing an extension
**_Note:_** A one-time developer registration fee of US$5.00 is required to verify your account and publish items.

1. [Click here](https://chrome.google.com/webstore/developer/dashboard) to publish chrome extension.
2. Follow the steps in the below YouTube video.

[![Image](http://img.youtube.com/vi/Gn_jlvkHTnM/0.jpg)](https://www.youtube.com/watch?v=Gn_jlvkHTnM)
