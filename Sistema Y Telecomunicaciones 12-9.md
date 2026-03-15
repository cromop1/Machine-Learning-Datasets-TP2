<p align="center">
  <img src="https://i.imgur.com/cKPuyVG.png" width="100%" alt="Banner Proyecto Integrador 2025">
</p>
<p align="center">
  <img src="https://i.imgur.com/RVGaecC.png" width="100%" alt="Banner Proyecto Integrador 2025">
</p>







<p align="center">
  <img src="https://i.imgur.com/BBMgp0q.png" width="100%" alt="Banner Proyecto Integrador 2025">
</p>

<p align="center">
  <img src="https://custom-icon-badges.demolab.com/badge/Contribuidores-4-6F42C1.svg?logo=people&logoColor=white">
  <img src="https://custom-icon-badges.demolab.com/badge/Entorno-Produccion-FD7E14.svg?logo=gear&logoColor=white">
  <img src="https://custom-icon-badges.demolab.com/badge/Repo-GitHub-181717.svg?logo=github&logoColor=white">
  <img src="https://custom-icon-badges.demolab.com/badge/Status-Finalizado-28A745.svg?logo=check-circle&logoColor=white">
  <img src="https://custom-icon-badges.demolab.com/badge/Raspberry%20Pi-CC0000.svg?logo=raspberrypi&logoColor=white">
  <img src="https://custom-icon-badges.demolab.com/badge/Router-0078D7.svg?logo=router&logoColor=white">
  <img src="https://custom-icon-badges.demolab.com/badge/Configuracion inicial-008000.svg?logo=network&logoColor=white">
</p>



<p align="center">
  <img src="https://i.imgur.com/RVGaecC.png" width="100%" alt="Banner Proyecto Integrador 2025">
</p>

<div align="center">

## 📘 Índice

 [Introducción](#-introducción)  
 [Objetivo](#-objetivo)  
 [Desarrollo](#3-desarrollo)  
    [3.1 Kit utilizado](#31-kit-utilizado)  
    [3.2 Preparación de la Raspberry Pi](#32-preparación-de-la-raspberry-pi)  
      [3.2.1 Eliminación de la ISO anterior](#321-eliminación-de-la-iso-anterior)  
      [3.2.2 Instalación de la nueva ISO](#322-instalación-de-la-nueva-iso)  
      [3.2.3 Configuración inicial](#323-configuración-inicial)  
    [3.3 Acceso remoto mediante SSH](#33-acceso-remoto-mediante-ssh)  
 [Conclusión](#-conclusión)

</div>


<p align="center">
  <img src="https://i.imgur.com/RVGaecC.png" width="100%" alt="Banner Proyecto Integrador 2025">
</p>



# 🔸 Introducción

En esta actividad comenzamos el proceso para convertir una Raspberry Pi 3 en un router educativo, capaz de gestionar una red local aislada mediante servicios de red como DHCP y SSH.
Este trabajo busca preparar el dispositivo para que pueda asignar direcciones IP, permitir acceso remoto y administrar la comunicación entre los equipos conectados a un switch, simulando así el funcionamiento básico de un router real.

Para lograrlo, primero se realiza la instalación del sistema operativo, la configuración inicial del entorno y la habilitación de acceso remoto. Esto sienta las bases para tareas más avanzadas en etapas posteriores.
 
<p align="center">
  <img src="https://i.imgur.com/zDTIHyR.png" width="100%" alt="Banner Proyecto Integrador 2025">
</p>

# 🔸 Objetivo

El objetivo de este informe es preparar y configurar una Raspberry Pi 3 para su uso como router, logrando:

Instalar correctamente un sistema operativo.

Realizar la configuración inicial del usuario y entorno.

Manejar comandos fundamentales de Bash para administración del sistema.

Habilitar el servicio SSH para permitir acceso remoto seguro.

Establecer comunicación desde otra computadora hacia la Raspberry Pi.

<p align="center">
  <img src="https://i.imgur.com/zDTIHyR.png" width="100%" alt="Banner Proyecto Integrador 2025">
</p>

# 🔹3 Desarrollo

<p align="center">
  <img src="https://i.imgur.com/zDTIHyR.png" width="100%" alt="Banner Proyecto Integrador 2025">
</p>

## 🔹 3.1 Kit Utilizado
####  - **Raspberry Pi 3**  
 ![imagen](Raspberry_Pi_3.jpg)


####  - **Switch**  
![imagen](Switch.png)
####  - **Cable Ethernet**  
![imagen](Cable_Ethernet.png)
####  - **Fuente de alimentación** (para Switch y Raspberry Pi)  
![imagen](Fuente_de_alimentación.png)
####  - **MicroSD 16 GB**  Y  **Adaptador de microSD**  
 ![imagen](MicroSD.jpg)

####  - **Teclado**
  
![imagen](Teclado.png)

####  - **Monitor**  
![imagen](Monitor.png)





## **3.2 Preparación de la Raspberry Pi**

<p align="center">
  <img src="https://i.imgur.com/zDTIHyR.png" width="100%" alt="Banner Proyecto Integrador 2025">
</p>

### **3.2.1 Eliminación de la ISO anterior**

<p align="center">
  <img src="https://i.imgur.com/zDTIHyR.png" width="100%" alt="Banner Proyecto Integrador 2025">
</p>

- Retirar la microSD de la Raspberry Pi.  
- Insertarla en un adaptador y conectarla a la computadora.  
- Borrar la ISO vieja o formatear la microSD.

<p align="center">
  <img src="https://i.imgur.com/zDTIHyR.png" width="100%" alt="Banner Proyecto Integrador 2025">
</p>

### **3.2.2 Instalación de la nueva ISO**

<p align="center">
  <img src="https://i.imgur.com/zDTIHyR.png" width="100%" alt="Banner Proyecto Integrador 2025">
</p>

1. Descargar el instalador oficial desde:  
   https://www.raspberrypi.com/software/

2. En el programa seleccionar:  
   - **Dispositivo:** Raspberry Pi 3  
   - **Sistema operativo:** Arquitectura de 64 bits  
   - **Destino:** microSD  

3. Esperar a que finalice la instalación.  
4. Expulsar la tarjeta e insertarla nuevamente en la Raspberry Pi.

<p align="center">
  <img src="https://i.imgur.com/zDTIHyR.png" width="100%" alt="Banner Proyecto Integrador 2025">
</p>

### **3.2.3 Configuración inicial**

<p align="center">
  <img src="https://i.imgur.com/zDTIHyR.png" width="100%" alt="Banner Proyecto Integrador 2025">
</p>

Conectar:

- MicroSD  
- Monitor  
- Teclado  
- Fuente de alimentación  

Luego:

1. Encender la Raspberry Pi.  
2. Iniciar sesión con:  
   - **Usuario:** `grupo6`  
   - **Contraseña:** `123`

<p align="center">
  <img src="https://i.imgur.com/zDTIHyR.png" width="100%" alt="Banner Proyecto Integrador 2025">
</p>

## **3.3 Acceso remoto mediante SSH**

<p align="center">
  <img src="https://i.imgur.com/zDTIHyR.png" width="100%" alt="Banner Proyecto Integrador 2025">
</p>

### **🔹 Activación del servicio SSH**

En la Raspberry Pi ejecutar:

```bash
sudo systemctl enable ssh
sudo systemctl start ssh
```

enable → lo activa en cada reinicio

start → lo enciende en ese momento

### 🔹 Obtención de la dirección IP

Ejecutar:
```bash
hostname -I
```
Esto muestra la dirección IP de la Raspberry Pi dentro de la red local.



### 🔹 Configuración del SSH en notebook (Linux)

Para habilitar SSH en la notebook:
```bash
sudo apt-get install openssh-server
```
Luego activar el servicio:

```bash
sudo systemctl enable ssh
```

### 🔹 Conexión SSH desde la notebook

Una vez conocida la IP, ejecutar:
```bash
ssh grupo6@<IP_de_Raspberry>
```

Ejemplo:
```bash
ssh grupo6@192.168.60.112
```

Esto inicia una sesión remota segura dentro de la Raspberry Pi.






<p align="center">
  <img src="https://i.imgur.com/zDTIHyR.png" width="100%" alt="Banner Proyecto Integrador 2025">
</p>



# 🔸 Conclusión

<p align="center">
  <img src="https://i.imgur.com/zDTIHyR.png" width="100%" alt="Banner Proyecto Integrador 2025">
</p>

La preparación inicial de la Raspberry Pi 3 sienta la base para convertir el dispositivo en un router educativo funcional.
Gracias a la instalación correcta del sistema operativo, la configuración básica y la habilitación del acceso SSH, se obtuvo una Raspberry Pi completamente operativa y accesible remotamente.



<p align="center">
  <img src="https://i.imgur.com/iPxDSQA.png" width="100%" alt="Banner Proyecto Integrador 2025">
</p>








