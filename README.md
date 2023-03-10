## Installation
```
composer require devinow/base64
```
## Usage

### Standard

 * Encoding data

   ```php
   \Devinow\Base64\Base64::encode('test');
   ```

 * Decoding data

   ```php
   \Devinow\Base64\Base64::decode('R2FsbGlhIGVzdCBvbW5pcyBkaXZpc2EgaW4gcGFydGVzIHRyZXM=');
   ```

### URL-safe

 * Encoding data

   ```php
   \Devinow\Base64\Base64::encodeUrlSafe('test');
   ```

 * Decoding data

   ```php
   \Devinow\Base64\Base64::decodeUrlSafe('z4DOrM69z4TOsSDPh8-Jz4HOteG_liDOus6x4b22IM6_4b2QzrThvbLOvSDOvM6tzr3Otc65IOKApg~~');
   ```

### URL-safe without padding

 * Encoding data

   ```php
   \Devinow\Base64\Base64::encodeUrlSafeWithoutPadding('test');
   ```

 * Decoding data

   ```php
   \Devinow\Base64\Base64::decodeUrlSafeWithoutPadding('z4DOrM69z4TOsSDPh8-Jz4HOteG_liDOus6x4b22IM6_4b2QzrThvbLOvSDOvM6tzr3Otc65IOKApg');
   ```
