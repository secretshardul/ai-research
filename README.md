# Pinecone hack

## Python setup

```sh
# Install deps
sudo apt install python3-pip
sudo apt install python3.11-venv

# Create env
python3 -m venv ./venv
source ./venv/bin/activate

# Exit venv
deactivate
```

## CUDA setup

```sh
sudo apt install nvidia-driver-530 nvidia-dkms-530 nvidia-cuda-toolkit -y && reboot
```

