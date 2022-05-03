# Domotica con SSVEP

Trabajo práctico final realizado en el contexto de la Especialidad en Sistemas Embebidos de la FIUBA para el curso Biopotenciales y signos vitales, registro y aplicaciones.

Autor: [Marcos Dominguez](https://github.com/mrds90)

3 de mayo de 2022

v1.0.0

## Introducción
### Proposito
Se presenta una propuesta de aplicación para personas con tetraplegía. Esta consiste en una solucón para controlar dispositivos del hogar utilizando potenciales evocados visuales en estado estacionario (*SSVEP*).

### Alcances y limitaciones
Este trabajo se realiza en contexto universitacio con fines educactivos. El proyecto se limita a plantear la idea da aplicación y el esquemático del sistema. No se realiza el montaje completo del equipo o el desarrollo del firmware para que la aplicacióon sea funcional.

### Referencias

- **[RD1]** [DS52057A](Docs/RefDocuments/DS52057A%20-%20MCP2210EvaluationKit.pdf) - MCP2210 Evaluation Kit User's Guide
- **[RD2]** [DS20002288C](Docs/RefDocuments/DS20002288C%20-%20MCP2210-USB-to-SPI-Protocol-Converter-with-GPIO-(Host-Mode).pdf) - MCP2210 USB-to-SPI Protocol Converter with GPIO (Host Mode)
- **[RD3]** [SBAS499C](Docs/RefDocuments/SBAS499C%20-%20ads1299.pdf) - ADS1299-x Low-Noise, 4-, 6-, 8-Channel, 24-Bit, Analog-to-Digital Converter for EEG and Biopotential Measurements
- **[RD4]** [SLAU443B](Docs/RefDocuments/SLAU443B%20-%20ADS1299%20Performance%20Demonstration%20Kit.pdf) - ADS1299 Performance Demonstration Kit
- **[RD5]** [Schematics](https://github.com/EFilomena/PonchoDeBiopotenciales/blob/master/Hardware/doc/Schematics.pdf) - Poncho de bioponenciales

## Descripcion de la Aplicación

Esta aplicación consiste en un dispositivo que adquiere EEG y se conecta via USB a una Tablet. La tablet tiene la aplicación que interactua con el usuario.
Esta aplicación posee pantallas con pocas opciones para que el usuario vaya avanzando hasta llegar al dispositivo que quiere controlar.
En las siguiente figura se muestra la pantalla inicial del sistema.

![alt text](Docs/Figures/app_fig1.png)

Al seleccionar una opción se vera un menú similar al siguiente (depende de la configuración del hogar para el usuario particular)

![alt text](Docs/Figures/app_fig2.png)

En el menu anterior los ambientes del menu se muestran en función de los ultimos seleccionados por el usuario. Es decir que siempre que entre a la opción "hogar" del primer menu, las primeras dos opiciones que aparecerán son los dos ultimos ambientes que eligió en la app.

Seleccionado el abmiente aparecen los dispositivos a controlar como se muesta a continuación:

![alt text](Docs/Figures/app_fig3.png)

## Diagrama en bloques del sistema

En la siguiente imagen se puede visualizar el diagrama en bloques del sistema

![alt text](Docs/Figures/block_diagram.png)




