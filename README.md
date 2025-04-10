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
cat decrypted_file.txt
```
```
ipfs add decrypted_file.txt
```


![875effa0-41ee-4b1b-a2ae-9decfb23c4d8](https://github.com/user-attachments/assets/bfb2a3a2-372f-4423-a974-ffc8de05ea6d)





