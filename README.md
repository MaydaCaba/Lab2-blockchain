# Lab2-blockchain
Laboratorio 2: Bloque + Cadena + validación
* **Estudiante:** [MAYDA LISBETH CABA CONTRERAS]
* **Modulo1** [Introducción a Blockchain y Criptomonedas]

## Características principales
* **Estructura del Bloque:** Modela la cabecera con `version`, `hash_previo`, `raiz_merkle`, `tiempo`, `bits`, `nonce` y los `datos` asociados.
* **Enlace Criptográfico:** Cada nuevo bloque calcula su huella digital y se vincula mediante el `hash` del bloque anterior, partiendo desde el Bloque Génesis.
* **Validación de Integridad:** Incluye un algoritmo (`es_cadena_valida`) que verifica tanto la consistencia interna de los datos como la continuidad de los enlaces entre bloques.
* **Pruebas de Manipulación:** Contiene pruebas automatizadas con `unittest` que demuestran cómo el sistema detecta alteraciones en los datos o intentos de recalcular hashes en bloques intermedios.
