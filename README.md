# work-enviroment
Creacion de contenedores para poder trabajar, como devops

## Instalamos las dependencias para poder correr el contenedor 
 
    - docker 
    - virtualbox

### Con el dockerfile de *Dockerfile.devops* crearemos nuestro contenedor que contendrá Terraform, vagrant, packer, ansible, aws-cli

 - 1º crearemos la imagen con el comando ```docker build -t devops -f images/Dockerfile.devops .```
 - 2º crearemos el contendor con el comando ```docker run -it --rm -v ./workspace-devops:/workspace devops```