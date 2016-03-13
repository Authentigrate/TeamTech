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
