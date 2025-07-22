# Git y GitHub Guía del Proyecto de Tarjetas Meme Colaborativas.

To read this guide in ENGLISH you can click [here](guide.md)
## ¡Bienvenidos!

¡Bienvenidos al **Proyecto de Tarjetas Meme Colaborativas de Git y GitHub**! Este proyecto es una forma divertida y práctica de aprender los fundamentos del desarrollo colaborativo de código usando Git para el control de versiones y GitHub para el alojamiento y el trabajo en equipo. El objetivo es contribuir con una "Tarjeta Meme" única a una página web compartida. El nivel de dificultad es **apta para principiantes**, diseñada para introducir conceptos fundamentales sin una complejidad abrumadora. El producto final será una página HTML estática que mostrará una colección de las tarjetas meme de todos los participantes, ¡un resultado tangible de nuestro esfuerzo colectivo!

## ¿Para quién es esto?

Veámoslo respondiendo la pregunta:

**¿Qué tanto sabes y usas GIT y GitHub de manera colaborativa?**

**Nivel 1: Principiante**
- Sé clonar repositorios (`git clone`), hacer cambios y subirlos con `git add`, `git commit` y `git push`.
- Puedo crear archivos y carpetas, pero no suelo trabajar con ramas ni resolver conflictos.
- Trabajo principalmente en mi propio repositorio o en el branch principal.

**Nivel 2: Intermedio**
- Trabajo con ramas (`git branch`, `git checkout`, `git merge`) y hago pull requests en GitHub.
- Sé actualizar mi rama con los cambios del repositorio remoto usando `git pull` y resuelvo conflictos simples.
- Participo en revisiones de código, asigno issues y utilizo comentarios para colaborar.

**Nivel 3: Avanzado**
- Manejo flujos de trabajo colaborativos como fork & pull request, rebase interactivo (`git rebase -i`), cherry-pick, y squash merges.
- Resuelvo conflictos complejos y hago mantenimiento de ramas remotas y locales (`git remote`, `git fetch`, `git prune`).
- Automatizo procesos con acciones de GitHub (GitHub Actions), gestiono releases y participo en la administración del repositorio.

Este proyecto está abierto a quien quiera participar pero es ideal para los del **nivel 1** que quieran comprender cómo los programadores colaboran en el código usando Git y GitHub.

### Prerrequisitos:

- **Conocimientos básicos de informática:** Familiaridad con el uso de una computadora, la navegación en sistemas de archivos y la apertura de aplicaciones.
- **Editor de texto:** Acceso a un editor de código como VS Code, Sublime Text, Atom o Notepad++.
- **Navegador web:** Un navegador web moderno como Chrome, Firefox, Edge o Safari.
- **Acceso a internet:** Para conectarse a GitHub y descargar las herramientas necesarias.

### Requisitos:
- **Git instalado:** La herramienta de línea de comandos de Git debe estar instaladas en tu ordenador.
- **Cuenta de GitHub:** Necesitarás una cuenta gratuita de GitHub.

### Nivel de experiencia esperado:
- **No se requiere experiencia previa con Git ni con GitHub.** Esta guía y el proyecto están diseñados para ser tu primer paso en la colaboración de control de versiones.
- **Conocimientos básicos de HTML/CSS son útiles, pero no estrictamente necesarios.** Te proporcionaremos la guía necesaria para crear tu tarjeta.
## Tiempo aproximado de finalización
Prevé dedicar aproximadamente de **2 a 4 horas** a este proyecto. Esto incluye configurar tu entorno, crear tu tarjeta, comprender el flujo de trabajo de Git y participar en el proceso de solicitud de extracción.
## Estructura del proyecto y objetivos de aprendizaje
El proyecto consiste en una página web estática sencilla creada con HTML y CSS. Cada participante añadirá su propia "Tarjeta de meme" a esta página.

### Objetivos de aprendizaje:
Al completar este proyecto, podrás:
- Comprender el **propósito del control de versiones** con Git.
- Aprender a **clonar un repositorio** desde GitHub.
- Practicar la **creación y el cambio de ramas de Git** para el desarrollo aislado.
- Adquirir experiencia con la **preparación y la confirmación de cambios de código**.
- Aprender a **enviar tus cambios locales a un repositorio remoto de GitHub**.
- Dominar el proceso de **creación y gestión de solicitudes de extracción (PR)** en GitHub.
- Comprender la importancia de la **revisión de código** y cómo responder a los comentarios.
- Experimentar la **resolución de conflictos de fusión** (si surgen).
Contribuye a un **proyecto de programación colaborativa** de principio a fin.

## El flujo de trabajo de ramificación de funciones

### Descripción
El **flujo de trabajo de ramificación de funciones** es una práctica estándar en el desarrollo profesional. En lugar de que todos trabajen directamente en el código principal del proyecto, cada nueva función o tarea tiene su propia rama dedicada. Esto aísla tu trabajo, evitando que interrumpas el código base principal u otros desarrollos en curso. Una vez que tu función está completa y revisada, se fusiona de nuevo con la rama principal. Esto mantiene el código base principal estable y limpio.

## Confirmaciones convencionales de GIT (Conventional Commits)

### Descripción
Las **confirmaciones convencionales**, conventional commits, proporcionan una convención ligera sobre los mensajes para los commits. Es una forma estructurada de escribir mensajes de confirmación que facilita la lectura del historial del proyecto, ayuda a automatizar la generación de registros de cambios y facilita el control automático de versiones. Un mensaje típico de según la guía Conventional Commit se ve así:

```
type(scope): subject
[optional body]
[optional footer]
```

En este proyecto, nos centraremos principalmente en `type` y `subject`.
- **`type`**: Describe el tipo de cambio. Los tipos más comunes incluyen:
- `feat`: Una nueva característica
- `fix`: Corrección de un error
- `docs`: Cambios solo en la documentación
- `style`: Cambios que no afectan el significado del código (espacios en blanco, formato, omisión de punto y coma, etc.)
- `refactor`: Un cambio de código que no corrige un error ni añade una característica
- `test`: Adición de pruebas faltantes o corrección de pruebas existentes
- `chore`: Otros cambios que no modifican los archivos src ni de prueba (por ejemplo, proceso de compilación, herramientas)
- **`subject`**: Una breve descripción del cambio.

**Ejemplos de mensajes de confirmación:**
`Feat: se añadió estilos a tarjeta meme`
`Fix: cambio del tipo de display del estilo del div principal de la tarjeta meme`
`Feat: se añadió imagen a la tarjeta meme`
## Proceso
Los siguientes pasos describen el proceso típico para contribuir con tu tarjeta meme. Recuerda consultar los enlaces proporcionados abajo para obtener instrucciones detalladas si tienes alguna dificultad.

- ### Paso 1: **Bifurcar y clonar el repositorio**
- **Bifurcar:** En GitHub, busca el repositorio principal del proyecto y haz clic en el botón "Fork" para crear tu propia copia.
- **Clonar:** desde tu terminal o IDE clona el repositorio. Si lo haces desde la terminal busca y copia la dirección del repositorio del fork en tu cuenta y ejecuta el commando, por ejemplo:
   `git clone https://github.com/forked-repo.git` ó
   `git clone git@github.com:<tuUsuario>/forked-repo.git`

- ### Paso 2: **Crear una nueva rama**
- `git checkout -b feature/[your-github-alias]-card` (p. ej., `git checkout -b feature/jane-doe-card`)
### Paso 3: **Añade tu tarjeta meme**
- Abre `index.html` en tu editor de texto.
- Agrega un nuevo `div` que contenga tu tarjeta, dentro incluye tu alias de GitHub en un H1, un `div` para la imagen del meme y una descripción.
- Para tu imagen meme, usarás un **enlace (URL) a una imagen alojada externamente**. Puedes usar servicios como Imgur, Cloudinary, GitHub Gist (para imágenes pequeñas) o cualquier otra plataforma pública de alojamiento de imágenes. Asegúrate de que la imagen sea accesible públicamente mediante una URL directa.
- Dentro del `div` para la imagen meme, usa una etiqueta `img` con el atributo **src `apuntando a la URL de tu imagen externa** (por ejemplo, `src="https://i.imgur.com/your-meme.jpg" alt="breve descripcion de la imagen Meme">`).
- Agrega los estilos CSS específicos de tu tarjeta a `styles.css.
- Deja tu código limpio y sin comentarios.

### Paso 4: **Prepara y el commit de tus cambios**
- `git add .` (para preparar todos los archivos modificados, incluyendo tu imagen)
- `git commit -m "feat: agregada tarjeta meme de [tu-alias-github]"`

### Paso 5: **Sube tu rama a GitHub**
- `git push origin feature/[your-github-alias]-card`

### Paso 6: **Abre una Pull Request** (PR)
- Ve a tu repositorio en GitHub.
- Haz clic en "Comparar y solicitar Pull Request".
- Asegúrate de que la rama base sea `main` y que la rama de comparación sea tu rama con la tajeta del meme.
- Proporciona un título claro (por ejemplo, `feat: agregada tarjeta meme de [tu-alias-github]) y una breve descripción.

### Paso 7: **Aborda los comentarios y resuelve conflictos**
- Supervisa tu PR para ver si hay comentarios de los revisores. Realiza los cambios solicitados localmente. 
	- `git add .` y luego
	- `git commit -m "fix: address review comments"`,
	-  `git push`
- Si hay conflictos de fusión, ejecuta `git pull origin main` en tu rama, resuelve los conflictos manualmente en tu editor y luego ejecuta:
	- `git add .`
	- `git commit -m "fix: resolucion conflictos del merge"`
	- `git push`.

### Paso 8: **Fusiona tu solicitud de PR**
  - Una vez aprobada tu solicitud de pull request y con todas las comprobaciones correctas, se fusionará en la rama `main`.

### Paso 9: **(Opcional) Limpieza**
	- `git checkout main`
	- `git pull origin main`
	- `git branch -d feature/[your-github-alias]-card` (elimina la rama local)`
  - Ve a GitHub y elimina la rama remota.

## Lista de enlaces

- **Instalación de Git:**
	- [Descargas de Git](https://git-scm.com/downloads)

- **Creación de una cuenta de GitHub:**
	- [Unirse a GitHub](https://github.com/join)

- **Comandos básicos de Git:**
	- [Manual de Git - Guías de GitHub](https://guides.github.com/introduction/git-handbook/)
	- [Hoja de referencia de Git](https://training.github.com/downloads/github-git-cheat-sheet/)

- **Entender las solicitudes de extracción:**
	- [Acerca de las solicitudes de extracción - GitHub Documentación](https://www.google.com/search?q=https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-with-pull-requests/about-pull-requests)

- **Resolución de conflictos de fusión:**

	- [Resolución de un conflicto de fusión en GitHub](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/addressing-merge-conflicts/resolving-a-merge-conflict-on-github)

	- [Cómo resolver un conflicto de Git - Atlassian](https://www.atlassian.com/git/tutorials/using-branches/merge-conflicts)

- **Confirmaciones convencionales:**

	- [Confirmaciones convencionales Especificación](https://www.conventionalcommits.org/en/v1.0.0/

- **Servicios de alojamiento de imágenes:**
	- [Imgur](https://imgur.com/) (simple, ampliamente utilizado para compartir)
	- [Cloudinary](https://cloudinary.com/) (más robusto, pero podría ser excesivo para un meme simple)
	- [GitHub Gist](https://gist.github.com/) (puedes subir imágenes a un gist público y usar la URL original)


## [Glosario de Términos e ideas](glosario.md)
Haz clic en el titulo arriba para leer el glosario.

## Reflexiones finales y consejos

Aprender Git y GitHub es una de las habilidades más valiosas para cualquier aspirante a programador. Abre las puertas a proyectos colaborativos, contribuciones de código abierto y la gestión eficaz de tu propio código. No te desanimes si encuentras dificultades; ¡es parte del proceso de aprendizaje! Cada conflicto resuelto y cada solicitud de extracción fusionada es un paso adelante. ¡Tú puedes!