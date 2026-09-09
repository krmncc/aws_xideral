# Ambientación

Instalación de herramientas como: wsl, python, docker y jupyter 

## Tabla de contenidos
- ¿Qué es wsl?
  - Instalación  
- Feature 2

### ¿Qué es wsl?
Es una herramienta de windows para hacer uso del entorno Linux sin la necesidad de instaar máquinas virtuales que consumen muchos recursos
  ### Instalación
    -Abrir powershell para intalar wsl con el siguiente comando: wsl --install
    -Para cambiar la distribución instalada por default de Linux ponemos: wsl.exe --list --online ->para verficar las distribuciones , wsl.exe --install -d [Distro] -> colocamos el nombre de la distribución elegida
    -Verificar la distribución wsl que estamos usando wsl.exe --list --verbose y wsl.exe --set-default-version <1|2> -> Para establecer la versión predeterminada en WSL 1 o WSL 2 al instalar una nueva distribución de Linux, wsl.exe --set-default <Distro> -> Enviar la distribución or defecto de Linux, wsl.exe --distribution <DistroName>
    -Actualizar versión wsl 1 a 2: wsl.exe --set-version <Distro> <1|2>
    
    

## 🛠️ Usage
Explain how to run, use, or test the project.
```bash
npm start
```

## 🤝 Contributing
Guidelines for how people can help improve the code.

## 📄 License
This project is licensed under the MIT License.

