# TiQRBlobReader

Appcelerator Titanium module to detect a QR code in a TiBlob image.


### Note:

This might not work on older devices. See : https://forums.developer.apple.com/thread/20887


## Usage:

```
    var qr = require("com.kosso.qrblobreader");
 
    // required
    var blob = an image TiBlob ... eg: event.media from the photo picker...
    // required
    var callback = function(e){
        
        console.log(e);

        if(e.code){
        	console.log('Code detected: ', e.code);
        }

    };
 
    // detect QR code in image blob
    qr.detectCode( blob, callback );

```

See example.

-------------------

@Kosso : March 28, 2016