<h2>Galcier Verifier</h2>

![Gav5w-TakAAdahn](https://github.com/user-attachments/assets/181dd05c-26ad-4aec-9e83-a255c13a9371)

## Hardware Requirements
### Minimum:
- CPU with 1+ cores
- 2GB RAM
- 4 MBit/sec download Internet service

### Recommended:
- Fast CPU with 2+ cores
- 4GB+ RAM
- 8+ MBit/sec download Internet service

---

## Preparation and Gas Fees

Register new wallet :
[https://www.glacier.io/points](https://www.glacier.io/points/?inviter=0xAD08506e384BD79e2a0F647C49d436F921483460)

Galxe Task : 
https://app.galxe.com/quest/glacierlabs/GChNBtVG6A

Bridge Bnb Testnet to Opbnb Testnet : 
https://opbnb-testnet-bridge.bnbchain.org/deposit

## installation on Linux CLI

```shell
apt install screen
screen -S glacier
mkdir glacier
cd glacier
wget https://github.com/Glacier-Labs/node-bootstrap/releases/download/v0.0.1-beta/verifier_linux_amd64
```
buat file config.yaml
```bash
nano config.yaml
```
Ubah `"YourPrivateKey"` dengan private key kalian
```bash
Http:
  Listen: "127.0.0.1:10801"
Network: "testnet"
RemoteBootstrap: "https://glacier-labs.github.io/node-bootstrap/"
Keystore:
  PrivateKey: "YourPrivateKey"
TEE:
  IpfsURL: "https://greenfield.onebitdev.com/ipfs/"
```

Run Node
```bash
chmod +x ./verifier_linux_amd64
./verifier_linux_amd64
```

