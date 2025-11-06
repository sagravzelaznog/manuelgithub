# Curso Rápido de GitHub

## 1. Configuración Inicial

### Instalar Git

Descarga e instala Git desde [git-scm.com](https://git-scm.com/)

### Configuración Inicial

```bash
# Configurar nombre de usuario
git config --global user.name "Tu Nombre"

# Configurar correo electrónico
git config --global user.email "tu@email.com"

# Verificar configuración
git config --list
```

## 2. Comandos Básicos

### Inicializar un repositorio

```bash
# Inicializar repositorio local
git init
```

### Verificar estado

```bash
git status
```

### Añadir archivos

```bash
# Añadir un archivo específico
git add nombre-archivo.ext

# Añadir todos los archivos
git add .
```

### Hacer commit

```bash
git commit -m "Mensaje descriptivo del cambio"
```

## 3. Trabajando con Ramas

### Crear y cambiar de rama

```bash
# Crear nueva rama
git branch nombre-rama

# Cambiar a la rama
git checkout nombre-rama

# Crear y cambiar de rama en un solo comando
git checkout -b nombre-rama
```

### Fusionar ramas

```bash
# Cambiar a la rama principal
git checkout main

# Fusionar la rama
git merge nombre-rama
```

## 4. Trabajando con GitHub

### Conectar repositorio local con GitHub

```bash
# Añadir repositorio remoto
git remote add origin https://github.com/usuario/repositorio.git

# Verificar repositorios remotos
git remote -v
```

### Subir cambios a GitHub

```bash
# Subir rama principal
git push -u origin main

# Para ramas adicionales
git push -u origin nombre-rama
```

### Actualizar repositorio local

```bash
git pull origin main
```

## 5. Flujo de Trabajo Básico

1. Actualiza tu repositorio local

   ```bash
   git pull origin main
   ```

2. Crea una nueva rama para tu característica

   ```bash
   git checkout -b nombre-caracteristica
   ```

3. Realiza tus cambios y guárdalos

4. Añade los cambios

   ```bash
   git add .
   ```

5. Haz commit de los cambios

   ```bash
   git commit -m "Descripción de los cambios"
   ```

6. Sube los cambios a GitHub

   ```bash
   git push -u origin nombre-caracteristica
   ```

7. Crea un Pull Request en GitHub

## 6. Comandos Útiles

### Ver historial de commits

```bash
git log --oneline
```

### Deshacer cambios

```bash
# Descartar cambios en un archivo
git checkout -- nombre-archivo

# Deshacer el último commit (manteniendo los cambios)
git reset --soft HEAD~1
```

### Clonar un repositorio

```bash
git clone https://github.com/usuario/repositorio.git
```

## 7. Buenas Prácticas

- Haz commits atómicos (un cambio lógico por commit)
- Escribe mensajes de commit claros y descriptivos
- Actualiza tu rama principal regularmente
- Usa ramas para nuevas características o correcciones
- Revisa tus cambios antes de hacer commit

## 8. Recursos Adicionales

- [Documentación oficial de Git](https://git-scm.com/doc)
- [GitHub Guides](https://guides.github.com/)
- [Git Cheat Sheet](https://education.github.com/git-cheat-sheet-education.pdf)
