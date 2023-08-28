# Shortcut Script to Install Nomad on Virtual Machines

The script, `install-nomad.sh`, is derrived from the [official documentation](https://developer.hashicorp.com/nomad/docs/install) setup process. 

Here are the minified steps to install Nomad on a virtual machine:

### 1. Install Nomad (required)
```bash
# Download install script from this repo
curl -fsSL https://raw.githubusercontent.com/jmitchel3/roadtok8s-nomad/main/install-nomad.sh -o install-nomad.sh

 # make it executable 
chmod +x install-nomad.sh

 # Run it
./install-nomad.sh

# Remove install script
rm install-nomad.sh
```

### 2. Install Docker (required)
After installing Nomad, install Docker Engine:

```bash
# Download install script from Docker
curl -fsSL https://get.docker.com -o install-docker.sh

# make it executable 
chmod +x install-docker.sh

 # Run it
./install-docker.sh

# Remove install script
rm install-docker.sh
```

### 3. Install Consul (optional):

```bash
sudo apt update && sudo apt install -y consul
```

### 4. Verify Nomad:

```
nomad --version
```
