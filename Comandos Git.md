
### Configuración Inicial

| **Comando**                       | **Descripción**                                             |
| --------------------------------- | ----------------------------------------------------------- |
| `git config user.name "Nombre"`   | Define el nombre de usuario local para tus commits.         |
| `git config user.email "email"`   | Define el correo electrónico asociado a tus commits.        |
| `git remote -v`                   | Muestra la URL del repositorio remoto configurado.          |
| `git remote add origin <url>`     | Conecta tu repositorio local con un repositorio en GitHub.  |
| `git remote set-url origin <url>` | Cambia la URL del repositorio remoto (útil si hay errores). |

### Flujo de Trabajo (Subir Cambios)

| **Comando**                 | **Descripción**                                                                                                |
| --------------------------- | -------------------------------------------------------------------------------------------------------------- |
| `git status`                | **El más importante:** Muestra qué archivos han cambiado, qué está "en verde" (staged) y qué falta por añadir. |
| `git add .`                 | Prepara todos los cambios (nuevos, modificados o eliminados) para ser incluidos en el próximo commit.          |
| `git commit -m "mensaje"`   | Empaqueta los cambios preparados con un mensaje descriptivo.                                                   |
| `git push`                  | Sube tus commits confirmados al repositorio remoto (GitHub).                                                   |
| `git push -u origin <rama>` | Sube los cambios y, además, establece la relación directa para que en el futuro solo uses `git push`.          |

### Obtención y Fusión de Cambios

| **Comando**               | **Descripción**                                                                               |
| ------------------------- | --------------------------------------------------------------------------------------------- |
| `git fetch`               | Descarga los cambios del servidor a tu computadora sin mezclarlos con tu código.              |
| `git merge origin/<rama>` | Une los cambios descargados (vía fetch) con tu rama actual.                                   |
| `git pull`                | **El combo:** Descarga (`fetch`) y mezcla (`merge`) los cambios del servidor automáticamente. |

### Traer Rama Eliminando Cambios Locales

| **Comando**                      | **Descripción**                                                        |
| -------------------------------- | ---------------------------------------------------------------------- |
| `git fetch origin`               | Descarga la versión más reciente en GitHub sin fusionar nada.          |
| `git reset --hard origin/master` | Resetea la rama actual para que sea exactamente igual a la rama remota |

### Gestión de Ramas y Estado

| **Comando**             | **Descripción**                                                            |
| ----------------------- | -------------------------------------------------------------------------- |
| `git branch`            | Lista las ramas existentes y te marca con un `*` en cuál estás trabajando. |
| `git checkout <nombre>` | Cambia de una rama a otra para trabajar en ella.                           |
| `git log`               | Muestra el historial de los commits realizados.                            |

### Manejo de Conflictos y Seguridad

| **Comando**                  | **Descripción**                                                                                    |
| ---------------------------- | -------------------------------------------------------------------------------------------------- |
| `git stash`                  | "Estaciona" o guarda tus cambios actuales temporalmente para limpiar el área de trabajo.           |
| `git stash pop`              | Recupera los cambios que habías guardado con `stash`.                                              |
| `git credential-store erase` | (Usado con precaución) Borra credenciales almacenadas que puedan estar causando errores de acceso. |
