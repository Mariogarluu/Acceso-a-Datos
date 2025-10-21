# 🔧 Configuración de Git - Autoría de Commits

## 📋 Descripción

Este documento explica cómo configurar Git para que **tus commits aparezcan con tu nombre y correo** como autor, en lugar de aparecer como un contribuidor externo o bot.

---

## 🎯 Problema

Cuando los commits aparecen con un nombre incorrecto o como "contributor" en lugar de como el dueño del repositorio, es porque la configuración de Git no está usando tus credenciales personales.

## ✅ Solución

### 1️⃣ Configuración Local (Solo para este repositorio)

Para configurar tu identidad **solo en este repositorio**, ejecuta:

```bash
# Navega a la carpeta de tu repositorio
cd /ruta/a/tu/Acceso-a-Datos

# Configura tu nombre (el que aparecerá en los commits)
git config user.name "Mario García Luque"

# Configura tu correo (debe ser el asociado a tu cuenta de GitHub)
git config user.email "garcialuquemario7@gmail.com"
```

> **💡 Nota:** El correo debe ser el mismo que usas en tu cuenta de GitHub. Puedes usar tu correo personal o el correo de privacidad de GitHub que tiene el formato: `ID+username@users.noreply.github.com`

### 2️⃣ Configuración Global (Para todos tus repositorios)

Para configurar tu identidad en **todos los repositorios** de tu sistema, usa `--global`:

```bash
# Configura tu nombre globalmente
git config --global user.name "Mario García Luque"

# Configura tu correo globalmente  
git config --global user.email "garcialuquemario7@gmail.com"
```

---

## 🔍 Verificación

### Comprobar la configuración actual

Para ver cómo está configurado Git actualmente:

```bash
# Ver configuración local (del repositorio actual)
git config user.name
git config user.email

# Ver configuración global (de todo el sistema)
git config --global user.name
git config --global user.email

# Ver toda la configuración
git config --list
```

### Verificar historial de commits

Para ver el autor de los commits recientes:

```bash
# Ver los últimos 10 commits con autor
git log --pretty=format:"%h - %an <%ae> : %s" -10

# Ver todos los autores únicos en el repositorio
git log --format='%an <%ae>' | sort -u
```

---

## 📧 Encontrar tu correo de GitHub

Tienes dos opciones para el correo:

### Opción 1: Correo personal
Tu correo personal registrado en GitHub (se mostrará públicamente en los commits).

### Opción 2: Correo de privacidad de GitHub (Recomendado)
GitHub proporciona un correo de privacidad con el formato: `ID+username@users.noreply.github.com`

Para encontrar tu correo de privacidad:

1. Ve a GitHub → Settings → Emails
2. Busca la sección "Primary email address"
3. Encontrarás tu correo de privacidad con el formato: `[ID]+[tu-usuario]@users.noreply.github.com`

Para el usuario **Mariogarluu**, el correo personal es:
```
garcialuquemario7@gmail.com
```

O puedes usar el correo de privacidad:
```
127546757+Mariogarluu@users.noreply.github.com
```

---

## 🔄 Aplicar cambios a commits futuros

Una vez configurado, **todos los commits nuevos** usarán automáticamente tu nombre y correo configurados.

Ejemplo:
```bash
# Después de configurar tu identidad
git add .
git commit -m "Mi primer commit con mi nombre"
git push
```

Este commit aparecerá con tu nombre y correo como autor.

---

## ⚠️ Commits anteriores

> **Importante:** La configuración solo afecta a **commits nuevos**. Los commits anteriores mantendrán el autor original.

### 🔧 Cambiar el autor de commits anteriores

Si deseas cambiar el autor de commits que ya existen (por ejemplo, commits hechos por bots o con información incorrecta), aquí están las opciones:

#### Opción 1: Cambiar solo el último commit

```bash
# Cambia el autor del último commit manteniendo los archivos tal como están
git commit --amend --author="Mario García Luque <garcialuquemario7@gmail.com>" --no-edit
```

#### Opción 2: Cambiar múltiples commits en una rama

Si tienes varios commits de un bot o contribuidor que quieres cambiar a tu autoría:

```bash
# PASO 1: Primero configura tu identidad
git config user.name "Mario García Luque"
git config user.email "garcialuquemario7@gmail.com"

# PASO 2: Reescribe los commits de la rama actual
# Cambia HEAD~2 por el número de commits que quieres modificar
# Ejemplo: HEAD~2 para los últimos 2 commits, HEAD~3 para los últimos 3, etc.
git rebase -i HEAD~2 -x "git commit --amend --author='Mario García Luque <garcialuquemario7@gmail.com>' --no-edit"

# PASO 3: Fuerza el push de la rama actualizada
git push --force-with-lease
```

#### Opción 3: Cambiar todos los commits de un autor específico

Si quieres cambiar TODOS los commits de un autor específico (como un bot) en toda la rama:

```bash
# ⚠️ ADVERTENCIA: Esto reescribe todo el historial
# Usa con precaución y asegúrate de tener un backup

git filter-branch --env-filter '
OLD_EMAIL="198982749+Copilot@users.noreply.github.com"
CORRECT_NAME="Mario García Luque"
CORRECT_EMAIL="garcialuquemario7@gmail.com"

if [ "$GIT_COMMITTER_EMAIL" = "$OLD_EMAIL" ]
then
    export GIT_COMMITTER_NAME="$CORRECT_NAME"
    export GIT_COMMITTER_EMAIL="$CORRECT_EMAIL"
fi
if [ "$GIT_AUTHOR_EMAIL" = "$OLD_EMAIL" ]
then
    export GIT_AUTHOR_NAME="$CORRECT_NAME"
    export GIT_AUTHOR_EMAIL="$CORRECT_EMAIL"
fi
' --tag-name-filter cat -- --branches --tags

# Después de verificar que todo está correcto:
git push --force-with-lease
```

### 📋 Recomendación para tu caso específico

Si tienes commits de "copilot-swe-agent[bot]" en tu rama y quieres cambiarlos a tu autoría **sin modificar los archivos**:

```bash
# 1. Asegúrate de estar en la rama correcta
git checkout copilot/update-contributor-ownership

# 2. Configura tu identidad
git config user.name "Mario García Luque"
git config user.email "garcialuquemario7@gmail.com"

# 3. Cuenta cuántos commits del bot hay (mira el historial)
git log --oneline

# 4. Si son los últimos 2 commits, usa:
git rebase -i HEAD~2 -x "git commit --amend --author='Mario García Luque <garcialuquemario7@gmail.com>' --no-edit"

# 5. Fuerza el push (esto reescribe el historial de la rama)
git push --force-with-lease origin copilot/update-contributor-ownership
```

### ⚠️ Advertencias importantes

1. **`git push --force-with-lease`** reescribe el historial. Solo hazlo en ramas donde trabajes solo tú.
2. **Backup**: Antes de hacer cambios drásticos, crea una rama de respaldo:
   ```bash
   git branch backup-branch
   ```
3. **Coordinación**: Si otros están trabajando en la misma rama, coordina con ellos antes de reescribir el historial.
4. **Rama principal protegida**: No uses `--force` en ramas principales como `main` o `master` si tienen protección.

---

## 📚 Comandos de Referencia Rápida

```bash
# Configurar identidad local
git config user.name "Tu Nombre"
git config user.email "tu@email.com"

# Configurar identidad global
git config --global user.name "Tu Nombre"
git config --global user.email "tu@email.com"

# Ver configuración
git config --list

# Ver últimos commits con autores
git log --pretty=format:"%h - %an <%ae> : %s" -5

# Verificar autor configurado
git config user.name
git config user.email
```

---

## 🎓 Diferencia entre Local y Global

| Tipo | Alcance | Archivo | Prioridad |
|------|---------|---------|-----------|
| **Local** | Solo el repositorio actual | `.git/config` | Alta ⭐ |
| **Global** | Todos los repos del usuario | `~/.gitconfig` | Media |
| **System** | Todos los usuarios del sistema | `/etc/gitconfig` | Baja |

> La configuración **local** tiene prioridad sobre la **global**. Si existe configuración local, se usará esa.

---

## ✨ Recomendación

Para tus repositorios personales, es mejor usar la configuración **global**:

```bash
git config --global user.name "Mario García Luque"
git config --global user.email "garcialuquemario7@gmail.com"
```

De esta forma, todos los commits en todos tus repositorios aparecerán automáticamente con tu nombre, sin necesidad de configurar cada repositorio individualmente.

---

## 🔗 Enlaces Útiles

- [Documentación oficial de Git Config](https://git-scm.com/docs/git-config)
- [GitHub: Setting your commit email address](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-personal-account-on-github/managing-email-preferences/setting-your-commit-email-address)
- [GitHub: Keeping your email address private](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-personal-account-on-github/managing-email-preferences/blocking-command-line-pushes-that-expose-your-personal-email-address)

---

<div align="center">

### 📝 Hecho para el repositorio Acceso a Datos

**¡Ahora todos tus commits aparecerán con tu nombre!** 🎉

</div>
