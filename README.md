# parcialAREP
Parcial 2 AREP

LOCAL:

![image](https://github.com/danielsperezb/parcialAREP/assets/101849347/8d7b649e-6c6b-4109-a540-e6d1953d2550)

DOCKER HUB:

![image](https://github.com/danielsperezb/parcialAREP/assets/101849347/d46821c4-261e-4665-8363-96c059b89512)

AWS:


![image](https://github.com/danielsperezb/parcialAREP/assets/101849347/b4edb119-887e-44ad-89f8-2f2802ea016e)

URL TESTED EN EL VIDEO ->

COMO CORRERLO EN EC2?

Instale Docker
sudo yum update -y
sudo yum install docker
Inicie el servicio de docker
sudo service docker start
Configure su usuario en el grupo de docker para no tener que ingresar “sudo” cada vez que invoca un comando
sudo usermod -a -G docker ec2-user
Desconectes de la máquina virtual e ingrese nuevamente para que la configuración de grupos de usuarios tenga efecto.
A partir de la imagen creada en Dockerhub cree una instancia de un contenedor docker independiente de la consola (opción “-d”) y con el puerto 6000 enlazado a un puerto físico de su máquina (opción -p):


docker run -d -p 42000:6000 --name firstdockerimageaws danielsperezb/parcialarep


![image](https://github.com/danielsperezb/parcialAREP/assets/101849347/f10bd05e-0ba8-4223-b6f4-4b331465d615)
