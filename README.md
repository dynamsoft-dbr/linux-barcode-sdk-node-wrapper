# Linux Barcode SDK Wrapper for Node.js
Build the **Node.js** extension with Dynamsoft Barcode Reader SDK for Linux. Create server-side barcode reader apps using JavaScript.

## Environment
* Node 8.4.0
* Npm 5.3.0
* [Dynamsoft Barcode SDK 6.2](https://www.dynamsoft.com/Downloads/Dynamic-Barcode-Reader-for-Linux-Download.aspx)

## How to Build the Extension 
1. Create symlink for libDynamsoftBarcodeReaderx64.so:

    ```
    sudo ln -s <Your PATH>/libDynamsoftBarcodeReaderx64.so /usr/lib/libDynamsoftBarcodeReader.so
    ```

2. Install **node-gyp**:

    ```
    npm install -g node-gyp
    ```

3. Configure building environment:

    ```
    node-gyp configure
    ```

4. Build the extension:

    ```
    node-gyp build
    ```

5. Run the test app:

    ```
    node test.js -f test.tif
    ```
    ![camera list in Python](screenshot/linux-node-barcode-reader.PNG)

## Blog
[How to Wrap Dynamsoft Linux Barcode SDK for Node.js](http://www.codepool.biz/linux-barcode-sdk-node-javascript.html)
