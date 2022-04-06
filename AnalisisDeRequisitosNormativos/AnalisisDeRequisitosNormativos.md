# Analisis de Requisitos Normativos
## Normativa
La norma en la que se basan los requisitos de diseño es la IEC60601-3-02.

## Naturaleza de los requisitos
Los requisitos mencionados son: 
- La respuesta en frecuencia.
- La impedancia de entrada.
- La relación de rechazo del modo común (CMRR).
- El desequilibrio del potencial de contacto de los electrodos.

Estos requisitos son requisitos de eficacia, debido a que el cumplimiento de los mismos aseguran una buena señal en la adquisición y no aspectos de seguridad.

## Filtrado

No es posible cumplir los requisitos solamente utilizando filtros digitales debido a que el ruido de alta frecuencia (> a fm/2) producen el efecto de aliasing. El aliasing no se puede discriminar una vez que se discretiza la señal de entrada.