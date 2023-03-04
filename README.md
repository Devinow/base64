## Installation
```
composer require devinow
```
## Usage

### Standard

 * Encoding data

   ```php
   \Delight\Base64\Base64::encode('Gallia est omnis divisa in partes tres');
   // string(52) "R2FsbGlhIGVzdCBvbW5pcyBkaXZpc2EgaW4gcGFydGVzIHRyZXM="
   ```

 * Decoding data

   ```php
   \Delight\Base64\Base64::decode('R2FsbGlhIGVzdCBvbW5pcyBkaXZpc2EgaW4gcGFydGVzIHRyZXM=');
   // string(38) "Gallia est omnis divisa in partes tres"
   ```

### URL-safe

 * Encoding data

   ```php
   \Delight\Base64\Base64::encodeUrlSafe('πάντα χωρεῖ καὶ οὐδὲν μένει …');
   // string(80) "z4DOrM69z4TOsSDPh8-Jz4HOteG_liDOus6x4b22IM6_4b2QzrThvbLOvSDOvM6tzr3Otc65IOKApg~~"
   ```

 * Decoding data

   ```php
   \Delight\Base64\Base64::decodeUrlSafe('z4DOrM69z4TOsSDPh8-Jz4HOteG_liDOus6x4b22IM6_4b2QzrThvbLOvSDOvM6tzr3Otc65IOKApg~~');
   // string(58) "πάντα χωρεῖ καὶ οὐδὲν μένει …"
   ```

### URL-safe without padding

 * Encoding data

   ```php
   \Delight\Base64\Base64::encodeUrlSafeWithoutPadding('πάντα χωρεῖ καὶ οὐδὲν μένει …');
   // string(78) "z4DOrM69z4TOsSDPh8-Jz4HOteG_liDOus6x4b22IM6_4b2QzrThvbLOvSDOvM6tzr3Otc65IOKApg"
   ```

 * Decoding data

   ```php
   \Delight\Base64\Base64::decodeUrlSafeWithoutPadding('z4DOrM69z4TOsSDPh8-Jz4HOteG_liDOus6x4b22IM6_4b2QzrThvbLOvSDOvM6tzr3Otc65IOKApg');
   // string(58) "πάντα χωρεῖ καὶ οὐδὲν μένει …"
   ```