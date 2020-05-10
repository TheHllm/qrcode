# qrcode
## Usage
Include the js file
```
<script src="https://raw.githubusercontent.com/TheHllm/qrcode/master/qrcode.min.js"></script>
```
use it
```
<script>
var qr = qrcode(0, 'H'); // TypeNumber(0 for auto), ErrorCorrectionLevel('L','M','Q','H')
qr.addData("Hello world"); //add some data to be 'encoded'
qr.make();
var img = qr.createImgTag(); // create a <img>
documend.body.appendChild(img); // add it to the dom
window.open(qr.createBlobUrl(20,10), '_self'); // open the qrcode
</script>
```

# Additonal information
https://github.com/kazuhikoarase/qrcode-generator/tree/master/js