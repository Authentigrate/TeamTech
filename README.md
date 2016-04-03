*Authentigrate* by Cryptr Team, Steven Povlitz and Nina Laurel

**Authentigrate** is an app that makes issuing and verifying cryptographically secure identities easy.

## User Stories

The following **required** functionality is completed:

- [x] User can take a picture (of a QR code)
- [x] QR code is processed such that the app has access to the data encoded in the QR code, and the data is not staved between app restarts
- [x] The app attempts to produce valid output by decrypting the data with the RSA algorithm and a public key stored within the app. The result is accessible to other parts of the app, but is not stored between app restarts
- [ ] If the output is valid and correctly decrypted by the private key, a ‘Valid’ screen containing the decrypted plaintext information is displayed
- [x] If the output is not valid, an ‘Invalid’ screen is displayed with a brief explanation of why the code is invalid, of either 'incorrect format' or 'no QR code found'

The following **optional** functionality is completed:
- [ ] User can import new signing / verifying RSA key pairs. This is done by taking a picture of a QR code containing a key pair from the default camera on the home screen
- [ ] User can set an imported signing / verifying key pair as the default key pair
- [ ] User can create new ID picture with encoded and QR code encrypted with RSA and private key
- [ ] User can create new ID picture with both QR and plaintext data
- [ ] User can share (using default ‘share’ procedure found in other apps) the ID picture
- [ ] The app can be set up to require a fingerprint scan to unlock
- [x] A “Help” screen is accessible from the home screen

## Wireframe Mock UP

<img src='http://i.imgur.com/cgzMfN2.jpg' title='Wireframe 2' width='' alt='Wireframe 2' />

## License

Copyright [2016] [Cryptr Team, Steven Povlitz and Nina Laurel]

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.




## Things from hackathon

<<<<<<< HEAD
# AsymmetricCryptoManager
AsymmetricCryptoManager is a Swift implementation of an asymmetric cryptography manager to facilitate the use of asymmetric cryptographic operations in Swift. Included is a sample view controller for testing purposes.

![](http://digitalleaves.com/blog/wp-content/uploads/2015/10/ezgif.com-optimize.gif)

## Usage

AsymmetricCryptoManager follows the Singleton pattern, thus it must be accessed by means of the sharedInstance variable.

### Generating a key pair

```swift
AsymmetricCryptoManager.sharedInstance.createSecureKeyPair({ (success, error) -> Void in
  if success {
    // start using the key pair.
  } else { 
    // handle the error
  }
})
```

### Encryption: 

```swift
AsymmetricCryptoManager.sharedInstance.encryptMessageWithPublicKey(clearText) { (success, data, error) -> Void in
  if success {
    let b64encoded = data!.base64EncodedStringWithOptions([])
    // transmit b64encoded encrypted string.
  } else { 
    // handle the error ...
  }
}
```

### Decryption:

```swift
AsymmetricCryptoManager.sharedInstance.decryptMessageWithPrivateKey(encryptedData) { (success, result, error) -> Void in
  if success {
    // manage the resulting string.  
  } else {
    // manage the error
  }
```

### Sign a message:

```swift
AsymmetricCryptoManager.sharedInstance.signMessageWithPrivateKey(clearText) { (success, data, error) -> Void in
  if success {
    let b64encoded = data!.base64EncodedStringWithOptions([])
  } else {
    // manage the error
  }
}
```

### Verify the signature:

```swift
AsymmetricCryptoManager.sharedInstance.verifySignaturePublicKey(rawData, signatureData: signatureData) { (success, error) -> Void in
  if success {
    // verification was successful
  } else {
    // verification failed.
  }
}
```

## LICENSE

The MIT License (MIT)
Copyright (c) 2015 Ignacio Nieto Carvajal (http://digitalleaves.com)

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
=======
*Authentigrate* by Cryptr Team, Steven Povlitz and Nina Laurel

**Authentigrate** is an app that makes issuing and verifying cryptographically secure identities easy.

## User Stories

The following **required** functionality is completed:

- [ ] User can take a picture (of a QR code)
- [ ] QR code is processed such that the app has access to the data encoded in the QR code, and the data is not staved between app restarts
- [ ] The app attempts to produce valid output by decrypting the data with the RSA algorithm and a public key stored within the app. The result is accessible to other parts of the app, but is not stored between app restarts
- [ ] If the output is valid and correctly decrypted by the private key, a ‘Valid’ screen containing the decrypted plaintext information is displayed
- [ ] If the output is not valid, an ‘Invalid’ screen is displayed with a brief explanation of why the code is invalid, of either 'incorrect format' or 'no QR code found'

The following **optional** functionality is completed:
- [ ] User can import new signing / verifying RSA key pairs. This is done by taking a picture of a QR code containing a key pair from the default camera on the home screen
- [ ] User can set an imported signing / verifying key pair as the default key pair
- [ ] User can create new ID picture with encoded and QR code encrypted with RSA and private key
- [ ] User can create new ID picture with both QR and plaintext data
- [ ] User can share (using default ‘share’ procedure found in other apps) the ID picture
- [ ] The app can be set up to require a fingerprint scan to unlock
- [ ] A “Help” screen is accessible from the home screen

## Wireframe Mock UP

<img src='http://i.imgur.com/cgzMfN2.jpg' title='Wireframe 2' width='' alt='Wireframe 2' />

## License

    Copyright [2016] [Cryptr Team, Steven Povlitz and Nina Laurel]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
>>>>>>> 529347e66f74a01377766fabceef473b15e46c51
