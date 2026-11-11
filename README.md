[Versión 0.7.1]: #
# fire - Actualiza y lanza firefox-esr, después actualiza y limpia el sistema

En firefox-esr no se pueden abrir nuevas pestañas cuando se ha instalado una nueva actualización mientras estaba en ejecución. Dado que el navegador es de lo primero que se abre, con "fire" primero se actualizará firefox y se abrirá al mismo tiempo que se sigue actualizando el resto del sistema. Con este script podremos actualizar en segundo plano mientras usamos firefox sin miedo a que necesitamos reiniciarlo.

---
## Estado del proyecto
Funciona correctamente
Se pueden mejorar detalles menores que no afectan al funcionamiento normal.

### Ficheros
- fire: script principal de llamada
- actualizar: lógica de actualizacion
- LICENSE: contenido de la licencia
- README.md: información del proyecto
- .gitignore: define elementos a ignorar

---
## Instalación
No requiere instalación

### Lenguaje
- Bash

### Dependencias
Sí, tiene dependencias de:
- nohup (Debian/Ubuntu)
- ./actualizar (script propio, leer apartado recomendación)

### Sistemas operativos compatibles
Probado en:
- Debian

---
## Recomendación
Para un uso mas ágil se puede crear una carpeta para script de forma que todos los que se añadan se puedan llamar desde la propia terminal como cualquier otro comando.

Esto se puede conseguir añadiendo a ~/.bashrc la línea:

```bash
    export PATH=$PATH:/ruta/a/carpeta/con/scripts
```

---
## Uso
Para usarlo es aconsejable aplicar la recomendación, este programa está compuesto por dos scripts

- **fire**
>>-> Es un lanzador que llama a actualizar y lanza firefox.

- **actualizar**
>>-> Actualiza el sistema (primero firefox-esr)

>>-> Limpia archivos de actualziaciones antiguas

>>-> Vacía la papelera de reciclaje

### Opciones de ejecución
A continuación veremos las diferentes opciones que existen:
- **fire**
>>-> Ejecución normal:
>>1. Se actualiza firefox
>>2. Se ejecuta firefox
>>3. Se actualiza y limpia el resto del sistema
- **fire e**
>>-> Ejecución normal + cierra la terminal al acabar de actualizar

>>-> ¡Cuidado! Si hay algun problema no lo verás
- **fire web1 web2**
>>-> Ejecución normal + abre webs pasadas como argumentos

- **actualizar**
>>-> Ejecución normal
>>1. Actualiza firefox
>>2. Actualiza y lismpia sistema

- **actualizar paquete1 paquete2**
>>-> Ejecución normal + actualizacion de paquetes

>>-> Se actualizan primero, junto a firefox los paquetes pasados como argumentos

---
## Licencia
Este proyecto está licenciado bajo GPLv2 - consulta el archivo LICENSE para más detalles.

---
## Autor
>**Alex**
- Github: [https://github.com/4lexKy](https://github.com/4lexKy)
- Email: [alex.correu@pm.me](mailto:alex.correu@pm.me)

---
