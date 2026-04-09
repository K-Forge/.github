<p align="center">
  <img src="https://img.shields.io/badge/◈_CONTRIBUTING-4C1D95?style=for-the-badge" alt="Contributing"/>
</p>

<p align="center">
  <sub>Guia para contribuir a los proyectos de <strong>K-Forge</strong>.</sub>
</p>

<br/>

## ◈ Antes de empezar

1. Se miembro activo de K-Forge o solicita acceso en [kforge.dev@gmail.com](mailto:kforge.dev@gmail.com).
2. Familiarizate con el proyecto al que deseas contribuir.
3. Lee este documento completo.

<br/>

## ◈ Convencion para Commits

Seguimos la convencion de **Conventional Commits**. Formato:

```
type: short message in english
```

> El mensaje siempre debe estar en **ingles**, en **minusculas**, y sin punto final. No usar scopes entre parentesis.

### Tipos de Commits

| Tipo       | Descripcion                                                  |
| ---------- | ------------------------------------------------------------ |
| `feat`     | Nueva funcionalidad                                          |
| `fix`      | Correccion de errores                                        |
| `chore`    | Tareas de mantenimiento del proyecto                         |
| `release`  | Preparacion de una nueva version                             |
| `hotfix`   | Correccion urgente en produccion                             |
| `docs`     | Cambios en documentacion                                     |
| `refactor` | Refactorizacion de codigo sin cambiar comportamiento         |
| `test`     | Agregar o modificar tests                                    |

### Ejemplos

```
feat: add login screen
fix: resolve jwt token expiration bug
chore: update spring boot dependencies
docs: add branching guide to contributing
refactor: extract user validation logic
test: add integration tests for user service
release: prepare version 1.0.0
hotfix: fix cors config in gateway
```

<br/>

## ◈ Modelo de Ramas — Git Flow

Seguimos el modelo **Git Flow** para organizar el trabajo en ramas. Todas las ramas deben partir de `develop` (excepto `hotfix/*`, que parte de `main`).

```
main ← release/* ← develop ← feature/tu-feature
main ← hotfix/*
```

### Tipos de Ramas

| Rama        | Proposito                                           | Nace de   | Se fusiona en       |
| ----------- | --------------------------------------------------- | --------- | ------------------- |
| `main`      | Codigo estable en produccion                        | —         | —                   |
| `develop`   | Integracion de funcionalidades en desarrollo        | `main`    | `release/*`, `main` |
| `feature/*` | Desarrollo de nuevas funcionalidades                | `develop` | `develop`           |
| `chore/*`   | Mantenimiento (docs, configs, dependencias, CI/CD)  | `develop` | `develop`           |
| `bugfix/*`  | Correccion de bugs no urgentes en desarrollo        | `develop` | `develop`           |
| `test/*`    | Pruebas de integracion o experimentacion            | `develop` | `develop`           |
| `hotfix/*`  | Correcciones urgentes en produccion                 | `main`    | `main`, `develop`   |
| `release/*` | Preparacion de una version para produccion          | `develop` | `main`, `develop`   |

### Convencion de nombres

Usar **kebab-case** (minusculas separadas por guiones) despues del prefijo. Ser descriptivo pero conciso.

```
feature/student-dashboard           (correcto)
feature/assignment-submission-api   (correcto)
chore/update-spring-dependencies    (correcto)
bugfix/fix-null-pointer-product     (correcto)
hotfix/fix-cors-gateway             (correcto)
release/1.2.0                       (correcto)
test/sprint-3                       (correcto)

feature/changes                     (incorrecto — muy vago)
mi-rama                             (incorrecto — falta prefijo)
feature/StudentDashboard            (incorrecto — no usar camelCase)
feat/login                          (incorrecto — usar feature, no feat)
```

### Flujo completo de trabajo

```bash
# 1. Actualizar develop
git checkout develop
git pull origin develop

# 2. Crear rama
git checkout -b feature/course-enrollment

# 3. Trabajar y hacer commits
git add .
git commit -m "feat: add course enrollment endpoint"

# 4. Push de la rama
git push origin feature/course-enrollment

# 5. Crear Pull Request → develop
# Esperar code review y aprobacion

# 6. Merge a develop (via PR)
# 7. Eliminar la rama feature
git branch -d feature/course-enrollment
```

<br/>

## ◈ Versionamiento

Seguimos **SemVer** (Semantic Versioning) con formato `MAJOR.MINOR.PATCH`.

| Segmento | Cuando incrementar                                | Ejemplo            |
| -------- | ------------------------------------------------- | ------------------ |
| `MAJOR`  | Cambios incompatibles con versiones anteriores    | `1.0.0` → `2.0.0`  |
| `MINOR`  | Nueva funcionalidad compatible hacia atras        | `1.0.0` → `1.1.0`  |
| `PATCH`  | Correcciones de errores en produccion (hotfix)    | `1.1.0` → `1.1.1`  |

### Versiones Pre-release

```
1.0.0-alpha.1    → Primera iteracion en desarrollo
1.0.0-beta.1     → Primera version en pruebas
1.0.0            → Version estable
```

Ciclo: **alpha** → **beta** → **release candidate** → **stable** → **maintenance / patch**

<br/>

## ◈ Pull Requests

- Titulo claro siguiendo convenciones de commits.
- Descripcion breve de **que** cambia y **por que**.
- Vincula el issue relacionado si existe.
- Asegurate de que el codigo compila y los tests pasan.
- Espera la revision de al menos **1 miembro** del equipo.

<br/>

## ◈ Estandares de codigo

- Escribe codigo claro y autoexplicativo.
- Nombra variables y funciones de forma descriptiva.
- Documenta funciones publicas.
- No subas credenciales, tokens ni informacion sensible.
- Usa variables de entorno para datos sensibles.

<br/>

## ◈ Reporte de bugs

Abre un **Issue** con:

- Descripcion del problema.
- Pasos para reproducirlo.
- Comportamiento esperado vs. actual.
- Capturas de pantalla si aplica.

<br/>

---

<p align="center">
  <sub>Dudas? Contacta a tu lider de equipo o escribenos a <a href="mailto:kforge.dev@gmail.com"><strong>kforge.dev@gmail.com</strong></a></sub>
</p>
