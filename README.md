# Blockchain-_assign.

# Practical 1 Fabric hyperledger

**to update the system**
```
sudo apt update
```

**to install golang-go**
```
sudo apt install golang-go
```
**to install docker**
```
sudo snap install docker
```
![8a8af518-ddc5-45bb-b015-31e93945fda8](https://github.com/user-attachments/assets/e3c987c4-4594-4e55-a280-12e2137269a3)


**to install git**
```
sudo apt install git
```
**to install fabric-samples**
```
git clone -b main https://github.com/hyperledger/fabric-samples.git
```
**to install curl**
```
sudo apt install curl
```
**to get in fabric-samples**
```
cd fabric-samples
```
![2cba31d9-fc1d-48dc-902f-70a5779f3526](https://github.com/user-attachments/assets/cebdcbdb-c977-4eae-9bea-edab7f081a58)



**to pull hyperledger docker images**
```
sudo bash
```

```
curl -sSL https://bit.ly/2ysbOFE | bash -s
```

![ed4f2ca3-9832-4180-aae7-cd793f2fc674](https://github.com/user-attachments/assets/222da943-c27b-43f8-98dc-beabe8526bff)



**to get into test network**
```
cd test-network
```

**to up the network**
```
./network.sh
```
```
./network.sh up
```


**to create channel**
```
./network.sh createChannel
```

![577607d3-e238-48f2-aaed-4b79ad64bb35](https://github.com/user-attachments/assets/b8650b72-6c7f-4cb8-84de-b27f3ed369e2)

**to down the network**
```
./network.sh down
```



# Practical- 2 : IPFS
**to install IPFS**
```
wget https://dist.ipfs.io/kubo/v0.32.1/kubo_v0.32.1_linux-amd64.tar.gz
```
![e7b71e7d-a8d3-4b68-a3c9-2ed12403307a](https://github.com/user-attachments/assets/1a9d4056-e32b-4dd1-a7e4-4228cb29f54f)





**to use kubo**
```
tar -xvzf kubo_v0.32.1_linux-amd64.tar.gz
```

**to get into kubo directory**
```
cd kubo
```



**to move to local bin**
```
sudo bash install.sh
```


**to initialise ipfs**
```
ipfs init
```


![a03f8658-b73e-4f68-8e4d-9396b86d367b](https://github.com/user-attachments/assets/945f33db-ce25-435c-beeb-9cd3be87148d)





**to use daemon**
```
ipfs daemon
```


![1a10884d-f0be-43cb-8de2-a9a9d351dbd4](https://github.com/user-attachments/assets/f636effd-5af5-4617-8883-e90abdaeb013)
![3907b456-4a88-48ba-947a-9a64cdeb1e73](https://github.com/user-attachments/assets/a2021bb2-6f4e-4fe2-87e2-ee1da9d4360b)




**to add file**
```
echo "Hello, komal!" > hello.txt
```
```
ipfs add hello.txt
```
```
ipfs cat <CID>
```

![f2a3158b-e70f-41ab-bac9-7e563878664e](https://github.com/user-attachments/assets/11709bdb-cf54-426e-97f2-a1ed1e4f42de)


![28e2d85e-354f-45ac-adc5-d1c2507255f5](https://github.com/user-attachments/assets/6cf2ae19-b43b-4af6-ad9a-064bafd03c86)





**to add a directory**
```
mkdir myfolder
```
```
echo "File 1 content" > myfolder/file1.txt
```
```
echo "File 2 content" > myfolder/file2.txt
```
```
ipfs add -r myfolder
```

![ef29ef9a-0da6-45a2-9e49-d1606524e427](https://github.com/user-attachments/assets/8abfa404-9580-44c5-b169-8a9fe5f28ecf)





**lists running processes**
```
ps aux | grep ipfs
```


**to kill the process**
```
kill <PID>
```


**encrypting and decrypting**
```
echo "hi komal" > myfile.txt
```
```
ipfs add myfile.txt
```
```
openssl enc -aes-256-cbc -pbkdf2 -iter 100000 -salt -in myfile.txt -out myfile_encrypted.txt -pass pass:yourpassword
```
```
ipfs add myfile_encrypted.txt
```
```
cat myfile_encrypted.txt
```
```
openssl enc -d -aes-256-cbc -pbkdf2 -iter 100000 -in myfile_encrypted.txt -out decrypted_file.txt -pass pass:yourpassword
```
```
cat decrypted_file.txt
```
```
ipfs add decrypted_file.txt
```

![875effa0-41ee-4b1b-a2ae-9decfb23c4d8](https://github.com/user-attachments/assets/9ad57088-67fe-435d-ac1b-739de92778c7)



# Practical-3 Metamask

**What is metamask?**
MetaMask is a crypto wallet and gateway to blockchain applications. It lets you store, manage, and transfer cryptocurrencies, especially those on the Ethereum blockchain and other EVM-compatible networks (like BNB Chain, Polygon, Arbitrum, etc.).


**Steps to Create a MetaMask Account**

**Step 1: Install MetaMask**
Browser Extension: Go to https://metamask.io and download the extension for Chrome, Firefox, Brave, or Edge.

Mobile App: Alternatively, install the MetaMask app from Google Play Store or Apple App Store.

**Step 2: Create a New Wallet**
Click “Get Started”.

Choose “Create a Wallet”.

Set a strong password (at least 8 characters).

Agree to the terms and conditions.

**Step 3: Backup the Secret Recovery Phrase**
MetaMask will generate a 12-word Secret Recovery Phrase.

Important: Write it down and store it in a secure and offline place. Never share it with anyone.

Confirm the phrase to complete setup.

**Your account is ready to use!**

![Screenshot (150)](https://github.com/user-attachments/assets/8cfe966d-808b-4cf2-84ae-d058d4ec369c)










Now in order to add tokens in the wallet we can add them via sepolia faucet,
these are the test token because we can't efford the etherum coin , also for the learning purpose we use them , these faucet can be get from the Google Cloud.



![430856293-015216ac-1931-407c-a698-238a237f2c91](https://github.com/user-attachments/assets/88cce6d3-829c-46fa-b518-c5707e6fe9de)

in the above we need to select our network and add our public key then click on recieve.
you will get some test tokens...
![Screenshot (156)](https://github.com/user-attachments/assets/707491b9-02e2-4f3f-8d55-46d95eba18a0)




**Now if we want to send money,we can di it by....**
clicking on **send**
Now enter the public key of whom you want to send tokens
Then, add tokens
And, continue

![Screenshot (161)](https://github.com/user-attachments/assets/780f4409-1f64-484e-b319-4796e8e1b154)


# Practical-4 To learn solidity through cryptozombie


CryptoZombies is an interactive and game baesd platform where we can learn Solidity, the programming language used for writing smart contracts on the Ethereum blockchain. It teaches us by building a zombie game step-by-step. From different lessons we can learn the following:-

**Lesson 1: Making the Zombie Factory**
*In this lesson we learned...*

Solidity basics

Contract structure

State variables

Functions

Events

*Here is the program I've created*
```
pragma solidity ^0.8.0;

contract ZombieFactory {
    event NewZombie(uint zombieId, string name, uint dna);

    uint dnaDigits = 16;
    uint dnaModulus = 10 ** dnaDigits;

    struct Zombie {
        string name;
        uint dna;
    }

    Zombie[] public zombies;

    function _createZombie(string memory _name, uint _dna) private {
        zombies.push(Zombie(_name, _dna));
        emit NewZombie(zombies.length - 1, _name, _dna);
    }

    function _generateRandomDna(string memory _str) private view returns (uint) {
        return uint(keccak256(abi.encodePacked(_str))) % dnaModulus;
    }

    function createRandomZombie(string memory _name) public {
        uint randDna = _generateRandomDna(_name);
        _createZombie(_name, randDna);
    }
}

```
**Lesson 2: Zombie Attributes**
*In this chapter we learnt:-*

to access modifiers (public, private, internal)

msg.sender

Mappings

require statement



```
mapping (uint => address) public zombieToOwner;
mapping (address => uint) ownerZombieCount;

function createRandomZombie(string memory _name) public {
    require(ownerZombieCount[msg.sender] == 0);
    uint randDna = _generateRandomDna(_name);
    _createZombie(_name, randDna);
    zombieToOwner[zombies.length - 1] = msg.sender;
    ownerZombieCount[msg.sender]++;
}
```

**Lesson 3: Advanced Solidity Concepts**
*in this lesson we learned to...*

import
Inheritance
Function overriding

```
import "./ZombieFactory.sol";

contract ZombieFeeding is ZombieFactory {
    function feedAndMultiply(uint _zombieId, uint _targetDna, string memory _species) public {
        require(msg.sender == zombieToOwner[_zombieId]);
        Zombie storage myZombie = zombies[_zombieId];
        _targetDna = _targetDna % dnaModulus;
        uint newDna = (myZombie.dna + _targetDna) / 2;
        if (keccak256(abi.encodePacked(_species)) == keccak256(abi.encodePacked("kitty"))) {
            newDna = newDna - newDna % 100 + 99;
        }
        _createZombie("NoName", newDna);
    }
}
```


**Lesson 4: Zombie Battle System**
*we learnt...*

time units in Solidity (e.g., 1 days)

Cooldowns

Struct updates

Randomness

```
uint cooldownTime = 1 days;

function _triggerCooldown(Zombie storage _zombie) internal {
    _zombie.readyTime = uint32(block.timestamp + cooldownTime);
}

function _isReady(Zombie storage _zombie) internal view returns (bool) {
    return (_zombie.readyTime <= block.timestamp);
}
```

**Lesson 5: ERC721 & Crypto Collectibles**
*In this lesson we learnt...*

ERC721 standard (NFTs)

transferFrom, ownerOf

Interfacing with other contracts

```
import "./erc721.sol";

contract ZombieOwnership is ERC721 {
    mapping (uint => address) zombieApprovals;

    function transferFrom(address _from, address _to, uint256 _tokenId) public override {
        require(_from == msg.sender || zombieApprovals[_tokenId] == msg.sender);
        ownerZombieCount[_to]++;
        ownerZombieCount[_from]--;
        zombieToOwner[_tokenId] = _to;
        emit Transfer(_from, _to, _tokenId);
    }
}
```



















