# MG Syndrome - Sitio web

Landing page de la marca de ropa urbana MG Syndrome.
Diseno y estampado a pedido + prendas en stock.

## Estructura

- `index.html` - la pagina completa (HTML, CSS y JavaScript en un solo archivo)
- `assets/` - fotos de las prendas y el logo

## Como publicarlo con GitHub Pages

### Opcion 1: desde la web de GitHub (sin instalar nada)

1. Crear una cuenta en github.com y confirmar el correo.
2. Arriba a la derecha, boton `+` > `New repository`.
3. Nombre del repositorio: `mgsyndrome-web`. Marcarlo como `Public`. Crear.
4. En la pagina del repositorio, click en `uploading an existing file`.
5. Arrastrar **todo el contenido de esta carpeta** (el `index.html`, el `README.md` y la carpeta `assets` completa).
6. Abajo, boton verde `Commit changes`.
7. Ir a `Settings` > en el menu lateral `Pages`.
8. En `Source` elegir `Deploy from a branch`. En `Branch` elegir `main` y carpeta `/ (root)`. Guardar.
9. Esperar 1 o 2 minutos y recargar. GitHub muestra la direccion:
   `https://TU-USUARIO.github.io/mgsyndrome-web/`

Ese es el link para pegar en Instagram.

### Opcion 2: con Git instalado

```bash
cd mgsyndrome-web
git init
git add .
git commit -m "Sitio MG Syndrome"
git branch -M main
git remote add origin https://github.com/TU-USUARIO/mgsyndrome-web.git
git push -u origin main
```

Despues activar GitHub Pages igual que en el paso 7.

## Poner un dominio propio

Si compras un dominio (por ejemplo `mgsyndrome.com.ar`):

1. Crear un archivo llamado `CNAME` en esta carpeta, con una sola linea:
   ```
   mgsyndrome.com.ar
   ```
2. Subirlo al repositorio.
3. En `Settings` > `Pages` > `Custom domain`, escribir el dominio y guardar.
4. En el panel del proveedor del dominio, crear estos registros DNS:
   - Tipo `A` apuntando a `185.199.108.153`, `185.199.109.153`, `185.199.110.153` y `185.199.111.153`
   - Tipo `CNAME` con nombre `www` apuntando a `TU-USUARIO.github.io`
5. Marcar `Enforce HTTPS`.

## Datos de contacto ya cargados

- WhatsApp: 2302 549140
- Instagram: @mgsynco
- Email: majomaidana09@gmail.com

## Precios

- Remeras estampadas: $30.000 ARS
- Pantalones estampados: $45.000 ARS

Los precios se editan en `index.html`, dentro de la lista de productos
(buscar la palabra `precio:`).

## Editar contenido

Todo el contenido esta en `index.html`. Para cambiar un producto, buscar
`var productos = [` y editar los datos de cada prenda: nombre, descripcion,
tipo y precio.
