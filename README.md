# PXE Pro APT Repository

This is the APT repository for PXE Pro.

## Installation Instructions

Before installing PXE Pro, you need to prepare your system by updating packages and installing required dependencies.

### 1. Prepare the System

```bash
sudo apt install software-properties-common
sudo apt update -y && sudo apt upgrade -y && sudo apt autoremove -y
sudo apt install dpkg-dev linux-headers-generic linux-image-generic
sudo apt install zfs-dkms zfsutils-linux
```

### 2. Add the PXE Pro Repository
Run the following command to add the PXE Pro APT repository to your system:
```bash
echo "deb [trusted=yes] https://soatrix.github.io/PXEPro stable main" | sudo tee /etc/apt/sources.list.d/pxepro.list
```

### 3. Install PXE Pro
Update your package list and install PXE Pro:

```bash
sudo apt update
sudo apt install pxepro-snapshot    # or pxepro-enterprise depending on the branch
```
Note: Make sure you choose the correct package based on your PXE Pro license or intended use.
