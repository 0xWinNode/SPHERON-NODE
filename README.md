# SPHERON WORKER NODE INCENTIVE

## Spek VPS

|  Hardware/VPS |  Minimum |
| ------------ | ------------ |
| CPU  | 4 or more physical CPU cores  |
| RAM | At least 8GB of memory (RAM) |
| Penyimpanan  | At least 100GB of SSD disk storage |
| Internet | At least 10mbps network bandwidth |

## Claim Faucet Arb Sepolia & Bridge to Spheron
- [Faucet 1](https://faucet.quicknode.com/arbitrum/sepolia) | [Faucet 2](https://www.alchemy.com/faucets/arbitrum-sepolia) | [Faucet 3](https://faucets.chain.link/arbitrum-sepolia) | [Faucet 4](https://learnweb3.io/faucets/arbitrum_sepolia/)
- Bridge Arb Sepolia to Spheron : [Here](https://spheron-devnet-eth.bridge.caldera.xyz/)

## Register Node
- Signup : https://app.spheron.network/login
- Signup with google/github
- Connect NEW WALLET METAMASK
- Klik Register Fizz Node
- Select Operating System (Linux)
- Configure Resources (sesuaikan dengan spek VPS kalian)
- Select a Region (Sesuai Negara VPS)
- Select the Payment token you want to accept (WETH)
- Select a Provider (Pilih yang Tier Kecil)
- Register > Confirm Metamask
- Download Skrip
- Upload Skrip to VPS

## Run Node
  - Install Docker (kalo belum punya)
    ```
    sudo apt update -y && sudo apt upgrade -y
    for pkg in docker.io docker-doc docker-compose podman-docker containerd runc; do sudo apt-get remove $pkg; done

    sudo apt-get update
    sudo apt-get install ca-certificates curl gnupg
    sudo install -m 0755 -d /etc/apt/keyrings
    curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg
    sudo chmod a+r /etc/apt/keyrings/docker.gpg

    echo \
      "deb [arch="$(dpkg --print-architecture)" signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/ubuntu \
      "$(. /etc/os-release && echo "$VERSION_CODENAME")" stable" | \
      sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
      sudo apt update -y && sudo apt upgrade -y

    sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
    sudo chmod +x /usr/local/bin/docker-compose
    ```
  - Cek Versi Docker
    ```
    docker --version
    ```
  - Run Skrip Node (Ganti namaskrip jadi namafile yang udah di download dari web)
    ```
    bash namaskrip.sh
    ```
  - Check Logs
    ```
    docker-compose -f ~/.spheron/fizz/docker-compose.yml logs -f
    ```
## Mint NFT & Check Status Node
**Back to web for Mint NFT & Check your Node If Success your node ACTIVE**
- Website : https://app.spheron.network/login
<p align="center">
  <img height="300" height="auto" src="https://github.com/zamzasalim/spheron/blob/main/xxxxxxxx.png">
</p>
