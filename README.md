# blowfish-wasm
Symmetric-key block cipher. Before usage needs to be compiled into wasm with [AssemplyScript](https://github.com/AssemblyScript/assemblyscript).

### Install project dependencies

In the root folder run:

    $ npm i
    
### Compile wasm

In the root folder run:

    $ npm run asbuild
   
### Usage in the project

#### For encryption

```javascript
const blowfish = new Blowfish('your_secret_key');
const encryptedString = blowfish.encr('phrase_to_encrypt');
```
#### For decryption

```javascript
const blowfish = new Blowfish('your_secret_key');
const decryptedString = blowfish.decr('phrase_to_decrypt');
```
