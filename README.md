# parcialAREP
Parcial 2 AREP

COMO CLONAR EL PROYECTO?

 git clone https://github.com/danielsperezb/parcialAREP.git

Antes de todo nunca estaria mal: Ejecutar "mvn clean install" en la ubicacion de tu archivo 

Ejecutas el anterior comando en la carpera que te quede mas comodo, hay maneras de correrlo:

1. AWS pero lastimosaente deberiamos dejar el servidor prendido para ver su funcionamiento (http://ec2-54-196-27-135.compute-1.amazonaws.com:34000/), se  deja un video de Youtube para su visualizacion;  https://www.youtube.com/shorts/LigUioT2BcE

2. Usa tu IDLE preferido puede ser NETBEANS y lo ejecutas RUN de manera interactiva http://localhost:4500/

3. En CMD puedes correr el siguiente comando java -cp "target/classes;target/dependency/*" com.mycompany.parcialarep.ParcialAREP http://localhost:4500/

5. Uno de los mas sencillos es ejecutar en cmd dentro de este proyecto clonado: "docker-compose up -d"    http://localhost:42000/

   


LOCAL:

![image](https://github.com/danielsperezb/parcialAREP/assets/101849347/8d7b649e-6c6b-4109-a540-e6d1953d2550)

DOCKER HUB:

Corriedo con docker de manera local:

![image](https://github.com/danielsperezb/parcialAREP/assets/101849347/adfd06c1-47a0-40d7-9fae-57fc0f0213c1)

![image](https://github.com/danielsperezb/parcialAREP/assets/101849347/37620e63-d38c-4de4-983d-a2072f9676d9)


![image](https://github.com/danielsperezb/parcialAREP/assets/101849347/cd2eecdc-8488-4689-ba0a-4ef8d368e879)

DOCKER DE MANERA LOCAL PERO CON DOCKER-COMPOSE.YML 

![image](https://github.com/danielsperezb/parcialAREP/assets/101849347/1239e9c3-3225-4a67-97ca-fc59ea9fc1fc)


DOCKER HUB EN MI PERFIL
![image](https://github.com/danielsperezb/parcialAREP/assets/101849347/d46821c4-261e-4665-8363-96c059b89512)

AWS:


![image](https://github.com/danielsperezb/parcialAREP/assets/101849347/b4edb119-887e-44ad-89f8-2f2802ea016e)

URL TESTED EN EL VIDEO -> https://www.youtube.com/shorts/LigUioT2BcE

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




![image](https://github.com/danielsperezb/parcialAREP/assets/101849347/870b76d1-d56c-461d-9136-2f2505dd6e69)

Respuesta JSON:

![image](https://github.com/danielsperezb/parcialAREP/assets/101849347/65951834-5400-43f5-8fe0-f3263fd694ba)


