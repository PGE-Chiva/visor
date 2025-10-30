# VISOR COMPLETO

Este repositorio contiene el "visor" web con los siguientes elementos principales:

- `index.html` — página principal
- `css/` — hojas de estilo
- `js/` — scripts JavaScript
- `images/`, `webfonts/` — recursos estáticos
- `data/` — datos utilizados por el visor
- `legend/`, `markers/` — recursos específicos del visor

Cómo ver el proyecto localmente
1. Abrir `index.html` directamente en el navegador (suficiente para una demo estática).
2. O servirlo desde un servidor local (recomendado para evitar problemas con peticiones XHR):

```powershell
# Usando Python 3 (desde la carpeta raíz del proyecto):
python -m http.server 8000
# luego abrir http://localhost:8000 en el navegador
```

Subir a GitHub (pasos rápidos)

1. Comprueba que `git` está instalado en tu máquina.
2. Desde PowerShell, sitúate en la raíz del proyecto (`VISOR COMPLETO`) y ejecuta:

```powershell
cd "C:\Users\Oficina\Desktop\webpge\combinación visores\VISOR COMPLETO"
git add .
git commit -m "Importar proyecto VISOR COMPLETO"
# crea el remote en GitHub manualmente o usando la CLI gh
# si ya tienes la URL remota:
git remote add origin https://github.com/TU_USUARIO/TU_REPO.git
git branch -M main
git push -u origin main
```

Si tienes la CLI `gh` instalada puedes crear y empujar el repo en un solo paso:

```powershell
gh repo create TU_USUARIO/visor --public --source="." --remote=origin --push
```

Nota sobre repos anidados

He detectado que existe una carpeta `.git` dentro de `visor` además del `.git` en la raíz `VISOR COMPLETO`. Esto crea un repositorio git anidado y suele causar confusión. Si no necesitas un repo independiente dentro de `visor`, renómbralo o elimínalo:

```powershell
# para renombrar (seguro):
Rename-Item -LiteralPath "C:\Users\Oficina\Desktop\webpge\combinación visores\VISOR COMPLETO\visor\.git" -NewName ".git.bak"

# o para eliminar (si estás seguro):
Remove-Item -LiteralPath "C:\Users\Oficina\Desktop\webpge\combinación visores\VISOR COMPLETO\visor\.git" -Recurse -Force
```

Si quieres, puedo:
- añadir más detalles al `README.md` (cómo desarrollar, dependencias, licencias),
- o renombrar/eliminar la carpeta `.git` anidada por ti (dime qué prefieres).

---

Archivo creado automáticamente por la herramienta de ayuda.
