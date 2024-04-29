# **Lectura 2 📕: Instalación de Linux en Maquina virtual**

## **Preparación del entorno de virtualización.**

Aunque ya hayamos tocado el tema de virtualización anteriormente, recordaremos brevemente el concepto. La virtualización es una tecnología que permite la creación de múltiples entornos virtuales en un solo servidor físico. Estos entornos virtuales, también conocidos como máquinas virtuales, son independientes entre sí y pueden ejecutar diferentes sistemas operativos y aplicaciones.

Preparar un entorno para virtualización puede constar de diferentes pasos, tales como:

- **Hardware adecuado**: Antes de comenzar, asegúrate de contar con un hardware adecuado para la virtualización. Esto incluye un servidor potente con suficiente capacidad de almacenamiento, memoria RAM y capacidad de procesamiento para soportar las máquinas virtuales que planeas crear.
- **Selección del software de virtualización**: Existen diferentes opciones de software de virtualización, como VMware, VirtualBox y Hyper-V. Es importante investigar y seleccionar el software que mejor se adapte a tus necesidades y requisitos.
- **Instalación del software**: Una vez que hayas seleccionado el software de virtualización, deberás instalarlo en el servidor. Podemos seguir la documentacion de la empresa desarrolladora del software o conseguir documentacion en linea
- **Configuración de la red**: Este paso es esencial para permitir la comunicación entre las máquinas virtuales y el resto de la red. Configura las interfaces de red de acuerdo con tus necesidades y asegúrate de asignar direcciones IP únicas a cada máquina virtual.
- **Creación de máquinas virtuales**: Una vez que el entorno de virtualización esté configurado, podrás crear las máquinas virtuales. Define los recursos asignados a cada máquina virtual, como la cantidad de memoria RAM, espacio en disco y número de núcleos de procesador.
- **Instalación de sistemas operativos y aplicaciones**: Después de crear las máquinas virtuales, deberás instalar los sistemas operativos y las aplicaciones necesarias en cada una de ellas. Esto se puede hacer utilizando imágenes ISO o discos de instalación.
- **Configuración de seguridad**: No olvides configurar medidas de seguridad adecuadas para proteger tu entorno de virtualización. Esto incluye la configuración de firewalls, actualizaciones de seguridad y políticas de acceso.

La preparación de un entorno de virtualización es un proceso que requiere planificación y ejecución cuidadosa. Sin embargo, los beneficios de la virtualización pueden ser significativos, por lo que vale la pena invertir el tiempo y los recursos necesarios para preparar un entorno adecuado.

## **Descarga e instalación de una distribución de Linux en servidores**

Recordemos que una distribución de Linux es un sistema operativo que puede usar el kernel de Linux, el cual cada versión puede variar en su sistema de gestión de paquetes y librerías.

Entre las distribuciones de Linux más populares para servidores tenemos:

- **Ubuntu Server:**

Ubuntu server es una de las distribuciones más conocidas y usadas para servidores actualmente en el mercado, es una variación de los sistemas operativos basados en Debian, esto significa que pueden tener una arquitectura similar y el mismo sistema manejador de paquetes, aunque en un ambiente profesional, Ubuntu Server puede tener un manejo mucho más fácil y una más alta compatibilidad del hardware.

Su instalación y configuración del sistema operativo son relativamente sencillas, y cuenta con una gran cantidad de documentación y recursos en línea para ayudarte en el proceso. Además, es compatible con una amplia gama de arquitecturas de hardware, lo que te brinda flexibilidad al elegir el servidor adecuado para tus necesidades.

La principal desventaja que puede tener Ubuntu server es que es un sistema operativo que ocupa mucho espacio en la máquina, y que las personalizaciones del sistema son posibles solo dentro de un marco limitado

<aside>
👉 Ubuntu Server es una gran opción cuando se busca administrar un servidor dentro de una estructura más fácil de manejar, sobre todo si se está en cambio desde windows.

</aside>

- **Red Hat Enterprise Linux (RHEL)**

Este sistema operativo es otra de las plataformas más usadas en servidores y en entornos empresariales, también hay que mencionar que está certificado en cientos de nubes, RHEL se destaca por su enfoque en la estabilidad, seguridad y rendimiento.

Una de las características clave de RHEL para servidores es su capacidad para manejar cargas de trabajo críticas y de alto rendimiento. Está diseñado para ofrecer un rendimiento óptimo y una alta disponibilidad, lo que lo convierte en una opción confiable para aplicaciones empresariales y servicios en línea también ofrece una amplia gama de herramientas y servicios para facilitar la administración y el despliegue de servidores.

La empresa detrás de RHEL, Red hat ofrece soporte técnico y servicios profesionales, lo que brinda a las empresas la tranquilidad de contar con asistencia experta en caso de problemas o necesidades específicas. También hay una gran comunidad de usuarios y desarrolladores de RHEL que proporcionan recursos y soporte adicional en línea.

Entre las desventajas que ofrece RHEL tenemos que no un sistema gratuito, ya que se maneja por suscripciones y además, no es un sistema solamente basado en línea de comando por lo que no lo hace ideal para principiantes

Si bien mencionamos como desventaja que RHEL no es un sistema gratuito, esto lo podemos tomar también como una ventaja ya que en seguridad, ofrece varias soluciones como Security-Enhanced Linux (SELinux) y los controles de acceso obligatorios (MAC), que le permiten evitar las intrusiones y cumplir con la normativa vigente. La plataforma también está certificada conforme a los Estándares Federales de Procesamiento de la Información (FIPS) 140-2, y es el primer soporte de los marcos de contenedores de Linux en obtener la certificación de Common Criteria (v7.1).

Este sistema operativo es ideal cuando queremos trabajar en un amplio ecosistema de software, hardware y nube (AWS, Microsoft Azure, Oracle Cloud Infrastructure).

- **CentOs**

CentOS está basado en Red Hat Enterprise Linux (RHEL) desde 2009, pero es de código abierto y gratuito. El sistema operativo es compatible con RHEL y destaca por su facilidad de uso. Especialmente en el ámbito de las distribuciones de servidores Linux, CentOS siempre ha sido convincente y se consideraba una solución de entrada que era válida para muchos usuarios. Sin embargo, Red Hat ha anunciado que la compatibilidad con CentOS finalizará en 2024. El sucesor CentOS Stream es visto con recelo por muchos desarrolladores, ya que es muy experimental y no es totalmente compatible con RHEL. La nueva solución funciona más bien como un entorno de prueba para el sistema.

CentOS es y fue considerado una solución gratuita a nivel básico que podía ofrecer las características de RHEL. El sistema operativo funciona de forma muy estable y es muy seguro gracias a una fuerte supervisión y a los parches regulares de la comunidad.

Sin embargo, CentOS no es una solución para el futuro, ya que la compatibilidad del sistema operativo se interrumpirá en un futuro cercano. Aunque muchas aplicaciones de RHEL también funcionan en CentOS, esto no siempre está garantizado porque faltan muchas certificaciones necesarias.

CentOS solo es apto para principiantes que quieran conocer RHEL sin pagar por él. Para proyectos a largo plazo, recomendamos otras distribuciones de Linux.

- **Debian**

Debian es una de las distribuciones para servidores web clásicas y de larga duración. El sistema existe desde 1993 y cuenta con una enorme comunidad en todo el mundo. Esta comunidad no solo utiliza Debian, sino que también mantiene el sistema. Debian es la base de muchas otras distribuciones de Linux, pero también está siendo constantemente optimizado por más de 1000 desarrolladores oficiales. El sistema operativo es igualmente recomendable para servidores, ordenadores de mesa y portátiles.

Además de su disponibilidad gratuita, la estabilidad y versatilidad de Debian hablan por sí mismas. El sistema operativo no solo es fiable, sino que también es compatible con numerosas arquitecturas de hardware y permite a los usuarios realizar numerosos ajustes individuales

Los principiantes pueden tener dificultades con Debian, ya que la instalación y la configuración pueden resultar complejas. Las actualizaciones no se producen a intervalos fijos y, por tanto, son difíciles de planificar. No se admiten archivos de paquetes personales. Además, la interfaz es clara, pero no muy moderna.

Debian es una solución fiable para los desarrolladores experimentados que se dediquen principalmente al sector del software y el hardware.

Existen distintas maneras de instalar una distribución de linux para un servidor. Para hacer una instalación directa debemos contar con la imagen ISO que descargamos en el paso anterior, y lo convertimos en un medio de instalación con un CD o una memoria USB para instalarlo directamente a la máquina que queramos usar en nuestro servidor, la ventaja de este método es que estaremos aprovechando el 100% de todos los recursos dedicados al servicio o servicios que queramos usar.

Otro de los metodos de instalacion que nos puede resultar bastante útil es la virtualización, el cual anteriormente hemos mencionado que permite crear versiones virtuales de recursos informáticos, como servidores, redes, almacenamiento y sistemas operativos y así en lugar de depender de una única instancia física, la virtualización permite la creación de múltiples instancias virtuales que se ejecutan de manera independiente en un entorno compartido, la virtualización implica la creación de servidores virtuales que se ejecutan en un servidor físico subyacente.

Para este módulo vamos a instalar ubuntu server en una máquina virtual para familiarizarnos con este entorno

Así como haciamos la instalación de una distribución de Linux, podemos descargar el sistema operativo a través de la página web de soporte de la distribución, para efecto de este módulo vamos a instalar Ubuntu server ingresando a [https://ubuntu.com/download/server](https://ubuntu.com/download/server) y descargando la version LTS (Long Term Support). Si quieres probar con otra distribución para servidor, puedes investigar cual es la página de descarga para la distribución que quieras usar.

Una vez descargado abrimos nuestro software de virtualización, para este módulo seguiremos con Virtual Box. Si no lo has descargado, puedes hacerlo a través de [https://www.virtualbox.org/wiki/Downloads](https://www.virtualbox.org/wiki/Downloads).

![administracionDeServidores-parte1%20ab5924e8fe3644549acdf70f4425a531/image1.png](administracionDeServidores-parte1%20ab5924e8fe3644549acdf70f4425a531/image1.png)

Para comenzar la configuración de nuestro servidor seleccionamos la opción nueva y llenar la información de las características que queremos colocar a nuestra máquina virtual:

![administracionDeServidores-parte1%20ab5924e8fe3644549acdf70f4425a531/image2.png](administracionDeServidores-parte1%20ab5924e8fe3644549acdf70f4425a531/image2.png)

1. Asignamos 2 GB de ram y dos procesadores.

![administracionDeServidores-parte1%20ab5924e8fe3644549acdf70f4425a531/image3.png](administracionDeServidores-parte1%20ab5924e8fe3644549acdf70f4425a531/image3.png)

1. Seleccionamos la opción de crear un disco duro virtual y asignamos la cantidad de memoria.

![administracionDeServidores-parte1%20ab5924e8fe3644549acdf70f4425a531/image4.png](administracionDeServidores-parte1%20ab5924e8fe3644549acdf70f4425a531/image4.png)

1. Vemos el resumen de cómo estará configurada nuestra máquina virtual y aceptamos.

![administracionDeServidores-parte1%20ab5924e8fe3644549acdf70f4425a531/image5.png](administracionDeServidores-parte1%20ab5924e8fe3644549acdf70f4425a531/image5.png)

<aside>
👉 Ya tenemos nuestra máquina virtual configurada y lista para funcionar, en la próxima lectura aprenderemos como configurar ubuntu server y por primera vez ver el entorno de un servidor.

</aside>

## **Configuración inicial del sistema operativo**

Aca te dejamos una pequeña guia de como configurar inicialmente ubuntu server dentro de nuestra máquina virtual:

- Antes de comenzar la instalación tenemos que hacer una previa configuración de la red por lo que entraremos en la seccion de configuracion del menu

![administracionDeServidores-parte1%20ab5924e8fe3644549acdf70f4425a531/image6.png](administracionDeServidores-parte1%20ab5924e8fe3644549acdf70f4425a531/image6.png)

- Seleccionaremos la opción de red y en la opción de *Conectado a:* seleccionamos la opción *Adaptador puente*. Esto nos permite que nuestra máquina virtual pueda conectarse a la tarjeta de red que tengamos en la máquina host y seleccionamos aceptar

![administracionDeServidores-parte1%20ab5924e8fe3644549acdf70f4425a531/image7.png](administracionDeServidores-parte1%20ab5924e8fe3644549acdf70f4425a531/image7.png)

- Una vez configurado la red, le damos click en iniciar y se nos abrirá una nueva ventana con la maquina virtual

### **Laboratorio 1** Escenario:

Acabas de ser contratado por la start-up D´sistemas cta para ser su administrador de sistemas, esta empresa necesita montar unos servidores para poder operar y facilitar el acceso a su información, aunque no tengas muchos conocimiento de como instalar un sistema operativo en un servidor, tu jefe decide acompañarte y explicarte en todo momento el paso a paso para la instalacion de nuestro servidor ubuntu.

1. Una vez arrancada la instalacion seleccionamos la primera opción “Try or install Ubuntu Server”

![administracionDeServidores-parte1%20ab5924e8fe3644549acdf70f4425a531/image8.png](administracionDeServidores-parte1%20ab5924e8fe3644549acdf70f4425a531/image8.png)

1. Lo primero que configuraremos será el idioma, por lo que seleccionaremos el idioma en el que nos queramos manejar en nuestro servidor.
2. La próxima ventana nos indicará la configuración de idioma del teclado, por lo que también seleccionaremos el idioma que queramos usar en nuestro teclado.
3. En la próxima ventana nos dara a seleccionar el tipo de instalación que queremos hacer
    
    ![administracionDeServidores-parte1%20ab5924e8fe3644549acdf70f4425a531/image9.png](administracionDeServidores-parte1%20ab5924e8fe3644549acdf70f4425a531/image9.png)
    
4. Ubuntu Server instalará una serie de paquetes que nos ayudará en el manejo de nuestro sistema operativo.
5. Ubuntu server (Minimized) es una versión más adaptable para ambientes de pruebas donde se espera algún tipo de ingreso de usuario.
    
    ![administracionDeServidores-parte1%20ab5924e8fe3644549acdf70f4425a531/image10.png](administracionDeServidores-parte1%20ab5924e8fe3644549acdf70f4425a531/image10.png)
    
6. Seleccionaremos la primera opción.
7. El próximo paso configuramos un adaptador de red, gracias a la configuración de red de adaptador puente que hicimos previamente podemos seleccionar nuestra tarjeta de red de nuestra máquina host.
8. Luego debemos que configurar un servidor Proxy en el caso que tengamos uno disponible, de no tener podemos saltar este paso
    
    ![administracionDeServidores-parte1%20ab5924e8fe3644549acdf70f4425a531/image11.png](administracionDeServidores-parte1%20ab5924e8fe3644549acdf70f4425a531/image11.png)
    
9. Después de la configuración de un proxy, tendremos que configurar el archivo Mirror, este es el archivo al cual nos vamos a conectar para obtener los repositorios del gestor de paquetes de archivos, ahi nos van a dar una opción por defecto la cual vamos a aceptar
    
    ![administracionDeServidores-parte1%20ab5924e8fe3644549acdf70f4425a531/image12.png](administracionDeServidores-parte1%20ab5924e8fe3644549acdf70f4425a531/image12.png)
    
10. El próximo paso paso será configurar un disco en el que vamos a almacenar nuestro Sistema operativo, en este caso de virtualización, tendremos la opción de un disco virtual, después tendremos el resumen de las particiones del disco en el cual tendremos dos particiones, partition 1 que tendremos el grub, y la partition 2 donde tendremos nuestro Sistema operativo
    
    ![administracionDeServidores-parte1%20ab5924e8fe3644549acdf70f4425a531/image13.png](administracionDeServidores-parte1%20ab5924e8fe3644549acdf70f4425a531/image13.png)
    
11. En la próxima ventana nos pedirá que le coloquemos los nombres a la máquina y al servidor junto a su contraseña.
    
    ![administracionDeServidores-parte1%20ab5924e8fe3644549acdf70f4425a531/image14.png](administracionDeServidores-parte1%20ab5924e8fe3644549acdf70f4425a531/image14.png)
    
    ![administracionDeServidores-parte1%20ab5924e8fe3644549acdf70f4425a531/image15.png](administracionDeServidores-parte1%20ab5924e8fe3644549acdf70f4425a531/image15.png)
    
12. El próximo paso nos preguntará si queremos instalar el servicio OpenSSH, recordemos que SSH es un protocolo el cual nos permitirá que podamos acceder a nuestro servidor de manera remota por lo que lo recomendable es aceptar.
    
    ![administracionDeServidores-parte1%20ab5924e8fe3644549acdf70f4425a531/image16.png](administracionDeServidores-parte1%20ab5924e8fe3644549acdf70f4425a531/image16.png)
    
13. Seleccionaremos algunos paquetes que queramos tener en nuestro sistema operativo, estas selecciones son opcionales por lo que no aceptaremos ninguno para esta práctica.
    
    ![administracionDeServidores-parte1%20ab5924e8fe3644549acdf70f4425a531/image17.png](administracionDeServidores-parte1%20ab5924e8fe3644549acdf70f4425a531/image17.png)
    
14. Después del último paso comienza la instalación del sistema operativo por lo que esperaremos unos minutos a que se termine una vez finalizada la instalación, seleccionamos la opción reboot now.
    
    ![administracionDeServidores-parte1%20ab5924e8fe3644549acdf70f4425a531/image18.png](administracionDeServidores-parte1%20ab5924e8fe3644549acdf70f4425a531/image18.png)
    

![administracionDeServidores-parte1%20ab5924e8fe3644549acdf70f4425a531/image19.png](administracionDeServidores-parte1%20ab5924e8fe3644549acdf70f4425a531/image19.png)

<aside>
💭 Una vez terminada la instalacion tu jefe se sienta contigo y te hace ciertas preguntas saber que tanto aprendiste en este proceso.

</aside>

- ¿Por que se elegio el tipo de instalacion?
- De tener un proxy para el servidor, ¿se puede agregar al momento de instalar?
- ¿Que beneficio podemos tener al instalar openssh?