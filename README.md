
# easywaze-cli

Project to get metrics from Waze CCP platform and genarate a set of metrics and alerts.

## Production mode

Requirements:
- Ubuntu, Debian, Fedora or CentOS.
- Docker support.
- Packages `curl` and `bash`.

How to install

```bash
curl https://raw.githubusercontent.com/thenets/easywaze-cli/master/easywaze-install.sh --output easywaze-install.sh
chmod +x easywaze-install.sh
sudo ./easywaze-install.sh
```

## Developer mode

This mode allow the development of EasyWaze.

```bash
# Build Docker images
make build

# Start all containers and prepare directories
make prepare

# Enter into shell mode inside the EasyWaze container
make shell

# Install dependencies
pip install -r requirements.txt

# Run main file
python main.py
```

Acesse `localhost:5000` com `root` e `root` e confira se os dados foram capturados

