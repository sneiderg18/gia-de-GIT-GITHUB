# Informe: Uso de Git y GitHub

**Autor:** Luis Sneider González Padilla  
**Tema:** Control de versiones con Git y GitHub  

---

##  Introducción
Git y GitHub son herramientas fundamentales para el control de versiones y la colaboración en proyectos de software.  
Git permite gestionar el historial de cambios de un proyecto localmente, mientras que GitHub sirve como plataforma en la nube donde esos proyectos pueden compartirse, almacenarse y mejorarse junto con otros desarrolladores.  

En este informe se presentan los conceptos aprendidos en dos videos, los comandos principales de Git, el proceso completo para subir un proyecto a GitHub y reflexiones personales sobre las ventajas y desafíos del uso de estas herramientas.

---

## 1. Resumen de los videos

### **Video 1 — Git y GitHub desde cero (Brais Moure)**
 [Ver video](https://www.youtube.com/watch?v=jGehuhFhtnE&t=225s)

**Conceptos aprendidos:**
- Git es un sistema de control de versiones que guarda el historial de cambios de un proyecto.
- Un commit representa un “punto de guardado” dentro del repositorio.
- GitHub permite almacenar repositorios en la nube y colaborar con otros programadores.
- La autenticación puede hacerse mediante HTTPS o SSH.
- Es importante usar mensajes claros en cada commit para mantener orden.

**Reflexión personal:**
Aprendí la importancia de usar Git desde el inicio de un proyecto para no perder el control del código. Me pareció muy útil la explicación sobre cómo los commits permiten volver a versiones anteriores sin dañar el trabajo. También entendí que GitHub facilita el trabajo en equipo, ya que cada miembro puede clonar, modificar y subir sus aportes.

---

### **Video 2 — Curso práctico de Git y GitHub (Midudev)**
 [Ver video](https://www.youtube.com/watch?v=VdGzPZ31ts8)

**Conceptos aprendidos:**
- Se explicó el flujo completo de trabajo: crear un repositorio local, hacer commits y sincronizar con GitHub.
- Uso de los comandos `git init`, `git add`, `git commit`, `git push` y `git pull`.
- Cómo crear ramas (`git branch`) para trabajar de forma paralela sin afectar la versión principal.
- Resolución de conflictos y buenas prácticas de colaboración.
- Uso del archivo `.gitignore` para excluir archivos innecesarios.

**Reflexión personal:**
Este video me ayudó a comprender el proceso real de trabajo con Git y GitHub. Me quedó claro cómo los cambios locales se envían al repositorio remoto, y cómo se pueden combinar ramas para mantener versiones organizadas. Lo más valioso fue aprender el flujo profesional que usan los desarrolladores día a día.

---

##  2. Comandos principales de Git

| Comando | Descripción |
|----------|--------------|
| `git init` | Inicializa un nuevo repositorio local. |
| `git status` | Muestra el estado actual de los archivos. |
| `git add .` | Agrega todos los archivos al área de preparación. |
| `git commit -m "mensaje"` | Guarda los cambios en el historial con una descripción. |
| `git branch -M main` | Renombra la rama actual a “main”. |
| `git remote add origin <url>` | Conecta el repositorio local con el remoto de GitHub. |
| `git push -u origin main` | Envía los cambios locales al remoto. |
| `git pull` | Descarga y combina los últimos cambios del remoto. |
| `git clone <url>` | Copia un repositorio remoto en tu máquina local. |
| `git log --oneline` | Muestra el historial resumido de commits. |
| `git branch` | Ver ramas existentes. |
| `git branch desarrollo` | Crear rama llamada 'desarrollo. |
| `git branch -d pruebas .` | Eliminar rama 'pruebas. |
| `git checkout main` | Cambiar a la rama 'main. |
| `git checkout -b pruebas` | Crear y cambiar a la rama 'pruebas. |
| `git switch desarrollo` | Cambiar a la rama 'desarrollo. |
| `git switch -c login` | Crear y cambiar a la rama 'login. |

---

##  3. Proceso paso a paso para subir un proyecto a GitHub

### **Pasos : Inicializar el repositorio y subirlo**
```bash
git --version

git config --global user.name "Tu Nombre"
git config --global user.email "tu_email@example.com"

cd /ruta/a/tu/proyecto
git init
git status

git add .
git commit -m "Inicial: agregar archivos del proyecto"

git branch -M main

git remote add origin https://github.com/sneiderg18/hello-git.git
git remote -v

git push -u origin main

```
# Evidencias de Git y GitHub

## 1 Clonación del repositorio
![Clonación del repositorio](./capturas/Screenshot%202025-11-02%20171317.png)

## 2 Confirmación (commit)
![Commit realizado](./capturas/Screenshot%202025-11-02%20171354.png)

## 3 Push al repositorio remoto
![Push al repositorio remoto](./capturas/Screenshot%202025-11-02%20171436.png)