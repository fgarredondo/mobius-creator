# Mobius Creator

**Impresora 3D delta reparable, modificable y adaptada a componentes disponibles en Argentina.**

> **Estado actual:** desarrollo y prototipado activo.  
> Todavía no existe una versión liberada para fabricación.

![Estructura principal de Mobius Creator](https://github.com/user-attachments/assets/8bc3c71f-5907-4190-829e-2219b956a86d)

## Descripción

Mobius Creator es un proyecto de impresora 3D delta de gran formato, diseñado con énfasis en la reparabilidad, la disponibilidad de repuestos y la posibilidad de adaptación por parte de sus usuarios.

El objetivo es desarrollar una máquina con un volumen y una velocidad de impresión considerables, que pueda ser construida, mantenida, modificada y reparada utilizando componentes estándar y alternativas disponibles en el mercado argentino, siempre que resulte técnicamente posible.

La publicación abierta de los archivos de diseño está planificada una vez que exista una configuración suficientemente estable, documentada y validada.


## ¿Por qué elegí una impresora delta?

La elección de la cinemática delta responde principalmente a la posibilidad de repetir un mismo mecanismo en las tres torres.

Al utilizar tres conjuntos mecánicos iguales, se reduce la cantidad de piezas diferentes que deben diseñarse, fabricarse, probarse y mantenerse. Una mejora realizada sobre el mecanismo de una torre puede aplicarse directamente a las otras dos.

En la configuración actual, cada torre utiliza solamente tres modelos diferentes de piezas impresas en 3D. Sus extremos están integrados en las bases inferior y superior de la estructura.

Como resultado, la estructura principal, incluidos los tensores de las correas, puede construirse a partir de cuatro modelos de piezas impresas en 3D y 4 chapas de aluminio cortadas mediante CNC.

Esta baja diversidad de componentes busca:

- Simplificar la fabricación.
- Reducir la cantidad de piezas que deben validarse.
- Facilitar la identificación y el almacenamiento de repuestos.
- Simplificar el armado y el mantenimiento.
- Permitir que las mejoras se apliquen de manera uniforme a las tres torres.

Sin embargo, la elección no fue solamente técnica. Desde que conocí las impresoras delta, siempre me fascinaron sus movimientos fluidos e hipnóticos. Esa combinación entre repetición mecánica, velocidad y movimiento terminó convirtiéndose en una parte central de Mobius Creator.

<img width="3300" height="2550" alt="Despiece base" src="https://github.com/user-attachments/assets/abb470a2-2a86-47c7-89b4-1313ba386a0f" />
<img width="2048" height="1536" alt="Tensor correa" src="https://github.com/user-attachments/assets/59e2f0c5-1e4c-4e42-9827-b95167aa4b26" />
<img width="2048" height="1536" alt="Carro" src="https://github.com/user-attachments/assets/3b429b73-4fd4-45d2-b7f4-8f37e9632786" />

## Objetivos del proyecto

El proyecto prioriza:

- Reparabilidad y facilidad de mantenimiento.
- Disponibilidad local de repuestos.
- Uso de componentes estándar.
- Documentación técnica clara.
- Publicación de archivos de diseño modificables.
- Adaptación a diferentes presupuestos y disponibilidades.
- Validación mediante prototipos y ensayos documentados.
- Identificación de alternativas compatibles para componentes críticos.

## Especificaciones preliminares

Las siguientes características representan el estado y los objetivos actuales del desarrollo. No deben considerarse especificaciones definitivas.

- **Arquitectura:** Delta.
- **Diámetro objetivo de impresión:** 350 mm.
- **Altura mínima objetivo de impresión:** 350 mm.
- **Firmware previsto:** Klipper.
- **Controladora prevista para el primer prototipo:** BTT SKR Mini.
- **Computadora de control prevista:** BTT Pi.
- **Extrusor previsto:** Sherpa Mini V3.
- **Rótulas previstas:** IGUS KCLM-06-EK.
- **Brazos previstos:** Fibra de carbono de 8 x 6 mm.
- **EndStop previstos:** Opticos.
- **Auto Nivelación:** Utilizando accesorio desmontable en la boquilla (tipo Biqu o Flsun).
- **Hotend experimental:** Disipador Creality K1, Barrel de titanio, Bloque Volcano y Boquilla CHT.
- **Efector experimental:** Nucleo impreso en 3D reforzado con placas de FR4 (tipo sandwitch). 

Las prestaciones de velocidad, aceleración, caudal, precisión y repetibilidad serán publicadas cuando puedan ser verificadas mediante ensayos reproducibles.

## Estado del proyecto

Mobius Creator se encuentra en fase de desarrollo y prototipado.

Los archivos, dimensiones, componentes y soluciones mecánicas pueden cambiar durante esta etapa. Las versiones preparadas para fabricación serán identificadas explícitamente y estarán acompañadas por su documentación correspondiente.

### Avances actuales

- [x] Definición inicial de la arquitectura.
- [x] Diseño de la estructura principal y las torres.
- [x] Diseño y prueba inicial del tensor de correas.
- [x] Desarrollo de un carro preliminar para validar el movimiento y las guías.
- [x] Selección preliminar de la electrónica.
- [ ] Fabricación de la estructura del primer prototipo (en proceso).
- [ ] Diseño y fabricación del efector (en proceso).
- [ ] Validación definitiva del carro.
- [ ] Fabricación y medición de los brazos.
- [ ] Integración electrónica.
- [ ] Configuración inicial de Klipper.
- [ ] Validación de movimiento.
- [ ] Calibración geométrica.
- [ ] Primera impresión.
- [ ] Ensayos de repetibilidad y precisión.
- [ ] Primera versión documentada para construcción externa.

## Desarrollo del efector

El efector se encuentra actualmente en etapa de diseño.

La configuración preliminar utiliza:

- Rótulas plásticas IGUS KCLM-06-EK.
- Extrusor Sherpa Mini V3.
- Disipador Creality K1.
- Barrel de titanio.
- Bloque calefactor tipo Volcano.
- Boquilla CHT.
- Nucleo impreso en 3D reforzado con placas de FR4 (tipo sandwitch). 

Esta combinación busca mantener un conjunto compacto y de bajo peso, facilitar el mantenimiento y conservar un caudal de material adecuado para impresiones de gran tamaño y velocidad. El diseño se realizara priorizando el fácil acceso y cambio de sus componentes.

La configuración podrá cambiar como resultado de las pruebas mecánicas, térmicas y de extrusión.

## Criterios de validación

Antes de publicar una primera versión reproducible se prevé evaluar, como mínimo:

- Repetibilidad del posicionamiento.
- Geometría y perpendicularidad de las torres.
- Uniformidad de movimiento de los carros.
- Estabilidad del sistema de correas.
- Precisión dimensional.
- Vibraciones y resonancias.
- Temperatura de motores y electrónica.
- Funcionamiento durante impresiones prolongadas.
- Facilidad de mantenimiento y sustitución de componentes.

Los resultados serán identificados como medidos, estimados o pendientes de validación.

## Hoja de ruta

### Etapa 1: prototipo mecánico

- Completar el efector.
- Fabricar y medir los brazos.
- Validar carros, guías y tensores.
- Verificar la geometría de la estructura.

### Etapa 2: integración

- Instalar la electrónica.
- Preparar el cableado.
- Configurar Klipper.
- Realizar las primeras pruebas de movimiento.

### Etapa 3: impresión y ensayos

- Realizar la primera impresión.
- Ajustar la calibración delta.
- Medir repetibilidad y precisión.
- Documentar fallas y modificaciones.
- Realizar pruebas de impresión prolongadas.

### Etapa 4: publicación reproducible

- Congelar una configuración experimental.
- Publicar la lista de materiales.
- Publicar archivos de fabricación identificados por versión.
- Preparar instrucciones de montaje.
- Incorporar problemas conocidos y advertencias.
- Convocar a los primeros constructores externos.

## Licencia

El proyecto se encuentra actualmente en fase de desarrollo y prototipado.

Todavía no se han definido las licencias que se aplicarán a los diseños mecánicos, la electrónica, el software y la documentación.

Salvo indicación expresa, la publicación de contenido en este repositorio no concede permiso para reproducir, modificar, fabricar, distribuir o comercializar los archivos o diseños publicados.

Las licencias definitivas serán informadas antes de la publicación de la primera versión abierta y reproducible del proyecto.

## Marca

**Mobius Creator** es una marca registrada en la República Argentina.

El nombre, el logotipo y los demás elementos identificatorios del proyecto no estarán incluidos automáticamente en las licencias abiertas que puedan aplicarse a los archivos de diseño, el software o la documentación.

La autorización para utilizar los diseños no implicará una autorización para comercializar productos utilizando la marca Mobius Creator.

## Advertencia

Este proyecto contiene componentes mecánicos móviles, elementos calefaccionados, conexiones eléctricas y etapas experimentales que pueden presentar riesgos si se fabrican, conectan o utilizan incorrectamente.

Las versiones experimentales no deben considerarse diseños terminados ni validados para producción.

Antes de fabricar o modificar cualquier componente:

1. Verificá la versión del archivo.
2. Consultá la documentación disponible.
3. Revisá los problemas conocidos.
4. Comprobá las dimensiones, los materiales y la compatibilidad.
5. No dejes el prototipo funcionando sin supervisión.

## Imágenes del desarrollo


### Soporte superior de la torre

![Soporte superior de la torre](https://github.com/user-attachments/assets/ba235d99-059a-4ee0-8339-9d9bb1cc3e29)

### Detalle del carro

![Detalle del carro](https://github.com/user-attachments/assets/0ae5da21-a42a-4deb-bd17-aea6d9d68dd7)

## Participación

El proyecto todavía no se encuentra en una etapa de construcción pública.

Sin embargo, son bienvenidos los comentarios relacionados con:

- Disponibilidad de componentes en Argentina.
- Experiencias con impresoras delta.
- Alternativas de componentes.
- Métodos de medición y validación.
- Reparabilidad.
- Documentación técnica.
- Posibles problemas mecánicos o de mantenimiento.

Las instrucciones formales para contribuir serán publicadas cuando se libere la primera versión experimental reproducible.
