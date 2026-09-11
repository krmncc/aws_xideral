# Ambientación

Instalación de herramientas como: wsl, python, docker y jupyter 

## Tabla de contenidos
- ¿Qué es wsl?
  - Instalación  
- ¿Qué es Docker?
  - Configuración
- ¿Qué es python?
  - Instalación
- ¿Qué es jupyter?
  - Instalación 

### ¿Qué es wsl?
Es una herramienta de windows para hacer uso del entorno Linux sin la necesidad de instaar máquinas virtuales que consumen muchos recursos
  ### Instalación
    -Abrir powershell para intalar wsl con el siguiente comando: wsl --install
    -Para cambiar la distribución instalada por default de Linux ponemos: wsl.exe --list --online ->para verficar las distribuciones , wsl.exe --install -d [Distro] -> colocamos el nombre de la distribución elegida
    -Verificar la distribución wsl que estamos usando wsl.exe --list --verbose y wsl.exe --set-default-version <1|2> -> Para establecer la versión predeterminada en WSL 1 o WSL 2 al instalar una nueva distribución de Linux, wsl.exe --set-default <Distro> -> Enviar la distribución or defecto de Linux, wsl.exe --distribution <DistroName>
    -Actualizar versión wsl 1 a 2: wsl.exe --set-version <Distro> <1|2>
    
    

### ¿Qué es docker?
Docker es una plataforma de software libre que permite empaquetar aplicaciones y todas sus dependencias en contenedores ligeros y portátiles. 

### Configuración
  #### Add Docker's official GPG key:
    sudo apt update
    sudo apt install ca-certificates curl
    sudo install -m 0755 -d /etc/apt/keyrings
    sudo curl -fsSL https://download.docker.com/linux/ubuntu/gpg -o /etc/apt/keyrings/docker.asc
    sudo chmod a+r /etc/apt/keyrings/docker.asc

  #### Add the repository to Apt sources:
    sudo tee /etc/apt/sources.list.d/docker.sources <<EOF
    Types: deb
    URIs: https://download.docker.com/linux/ubuntu
    Suites: $(. /etc/os-release && echo "${UBUNTU_CODENAME:-$VERSION_CODENAME}")
    Components: stable
    Architectures: $(dpkg --print-architecture)
    Signed-By: /etc/apt/keyrings/docker.asc
    EOF
    sudo apt update

### Instalar paquetes Docker

  #### After installation, verify that Docker is running:
    sudo systemctl status docker
  #### If Docker is not running, start it manually:
    sudo systemctl start docker

### Verificar instalación
  sudo docker run hello-world
  
### ¿Qué es python?
  Python es un lenguaje de programación de alto nivel, interpretado y de propósito general, diseñado para que su código sea    muy fácil de leer y escribir
### Instalación
  #### Instalar dependencias
    sudo apt install -y
    make
    build-essential
    libssl-dev
    zlib1g-dev
    libbz2-dev
    libreadline-dev
    libsqlite3-dev
    curl
    git
    llvm
    libncurses-dev
    xz-utils
    tk-dev
    libxml2-dev
    libxmlsec1-dev
    libffi-dev
  #### Instalar pyenv
    
    git clone https://github.com/pyenv/pyenv.git ~/.pyenv
    ls ~/.pyenv
    echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.bashrc echo 'export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.bashrc echo 'eval     "$(pyenv init - bash)"' >> ~/.bashrc source ~/.bashrc
    pyenv --version
    liblzma-dev

  #### Instalar python 3.14.7
    pyenv install --list | grep " 3.14" pyenv install 3.14.7 pyenv versions pyenv global 3.14.7 pyenv rehash python --version
  
### ¿Qué es jupyhter?
  Jupyter es una aplicación web de código abierto que permite crear y compartir documentos interactivos con código en vivo,    texto, ecuaciones y gráficos
### Instalación
  #### Crear el workspace y el entorno virtual
    mkdir -p ~/jupyter cd ~/jupyter python --version python -m venv .venv source .venv/bin/activate
  #### Instalar y ejecutar Jupyter Notebook
    Install the classic Jupyter Notebook with:
      pip install notebook
    To run the notebook:
      jupyter notebook

