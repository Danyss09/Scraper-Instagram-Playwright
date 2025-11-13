# Instagram Followers Scraper (Playwright)

Este script realiza web scraping en Instagram para obtener:
- El número de seguidores de una cuenta pública
- El nombre de usuario (username) de cada seguidor
- El número de seguidores que tiene cada uno de esos seguidores
- Exporta toda la información a un archivo Excel (`instagram_followers.xlsx`)

---

## 🚀 Requisitos

- Python 3.10 o superior
- pip
- Google Chrome o navegador compatible

---

## 📦 Instalación

1. Clonar o copiar este proyecto en tu máquina
2. Abrir una terminal dentro del proyecto
3. Crear entorno 
```bash
   python -m venv venv
```
4. Instalar dependencias:

   ```bash
   pip install -r requirements.txt
   playwright install
   ```


---

## ⚙️ Configuración

Antes de ejecutar el script, define tus credenciales de Instagram como variables de entorno:

### En macOS / Linux
```bash
export IG_USER="tu_usuario"
export IG_PASS="tu_contraseña"
```

### En Windows (PowerShell)
```bash
$env:IG_USER="tu_usuario"
$env:IG_PASS="tu_contraseña"
```

---

## ▶️ Ejecución

```bash
python ig_followers_scraper.py
```

El script:
1. Inicia sesión en Instagram (si no hay sesión guardada)
2. Abre el perfil objetivo (`TARGET` definido dentro del script)
3. Extrae todos los seguidores y sus datos
4. Guarda los resultados en `instagram_followers.xlsx`

---

## 📁 Archivos

| Archivo | Descripción |
|----------|--------------|
| `ig_followers_scraper.py` | Script principal del scraping |
| `requirements.txt` | Dependencias del proyecto |
| `README.md` | Instrucciones de uso |
| `auth.json` | Sesión guardada de Instagram (se genera automáticamente) |
| `instagram_followers.xlsx` | Archivo con los resultados exportados |

---

## 🧠 Notas

- Solo funciona con **cuentas públicas** o cuentas privadas donde tengas acceso.
- No hagas scraping de grandes volúmenes seguido (Instagram puede limitar temporalmente tu cuenta).
- Puedes ajustar el número máximo de seguidores a extraer modificando la variable `MAX_FOLLOWERS_TO_SCRAPE`.

---

## 💬  **Proyecto académico sobre scraping con Playwright.**
#**Programación para dispositivos moviles - UCE**
**Grupo 3**