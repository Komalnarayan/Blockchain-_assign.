# Blockchain-_assign.

# Prctical 1 Fabric hyperledger

**to update the system**
sudo apt update

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
./network.sh up
```


to create channel
./network.sh createChannel

![577607d3-e238-48f2-aaed-4b79ad64bb35](https://github.com/user-attachments/assets/b8650b72-6c7f-4cb8-84de-b27f3ed369e2)

to down the network
./network.sh down
