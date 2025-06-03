<h1> Universidad Nacional de Córdoba</h1>

<h2> Facultad de Ciencias Exactas, Físicas y Naturales</h2>

<h3> Sistemas de Comunicaciones Telefónicas </h3>
<h3> Central Telefónica VoIP con Raspberry Pi </h3>

---

<h3> Grupo: <strong> Transmitiendo Facts </strong>

Integrantes:
  - 
  - 
  - 
  
</h3>

# Introducción

En la actualidad, las comunicaciones basadas en tecnología VoIP (Voice over IP) han revolucionado la forma en que se transmiten las llamadas telefónicas, permitiendo reducir costos, mejorar la flexibilidad y facilitar la integración con otros sistemas informáticos. Este informe describe la implementación de una central VoIP basada en Asterisk y FreePBX sobre una plataforma Raspberry Pi, un dispositivo de bajo costo y consumo energético. El sistema instalado permite gestionar comunicaciones internas y externas mediante el uso del protocolo SIP (Session Initiation Protocol), incluyendo la configuración de un servidor proxy y el registro de extensiones SIP para la realización de llamadas entre usuarios locales y hacia el exterior.

# Instalacion de FreePBX

Se descargó la imagen ISO de FreePBX de la [página oficial](https://www.freepbx.org/sngfd12/) y luego se lamontó en una tarjeta SD mediante el software Raspberry Pi Imager.

![Interfaz de Raspberry Pi Imager](img/imager.webp)

![Inicio en Raspberry](img/inicio.png)

Luego se insertó la SD a la Raspberry y se seleccionó la versión recomendada de FreePBX con la opción de instalación gráfica. Mientras se instala, se puede cambiar la contraseña de inicio en `Root Password`.

![Instalacion](img/sangoma.png)

Luego de la instalación, se reinició la placa y se inició sesión con el usuario `root` y la contraseña configurada anteriormente. La instalación está completa.

# Configuración

Se observó que la placa posee una dirección IP, que si se ingresa a la misma mediante un navegador, se pueden realizar todas las configuraciones de administración gracias a la GUI de FreePBX.

![Pagina principal de FreePBX](img/freepbx_inicio.png)
