# FacPro Apps para Android

Apps de Android de **FacturaPro EC**:

| App | Para quién | Descargar |
|---|---|---|
| **FacPro Chofer** | Choferes: rutas, entregas, fotos, firma, guías y GPS de la ruta | [FacPro-Chofer.apk](https://github.com/Democresss/FacPro-Android/releases/latest/download/FacPro-Chofer.apk) |
| **FacPro Pedidos** | Vendedores y meseros: toma de pedidos | [FacPro-Pedidos.apk](https://github.com/Democresss/FacPro-Android/releases/latest/download/FacPro-Pedidos.apk) |

## Cómo se instala

1. Abre el enlace de la app desde el teléfono y descarga el `.apk`.
2. Ábrelo. Si Android lo pide, permite «Instalar apps de esta fuente».
3. Entra con la misma cuenta de siempre.

## Cómo funciona

- Las pantallas son las mismas de la web (`/v2/chofer/app` y `/v2/pedidos/dashboard`). Se ven igual y cada cambio publicado en la web llega solo, sin reinstalar.
- **Se actualiza sola.** Al abrirse busca la última versión publicada aquí; si hay una nueva, la descarga y abre el instalador.
- **GPS con la pantalla apagada** (FacPro Chofer). Mientras el chofer tiene entregas pendientes, un servicio con aviso fijo sigue mandando la ubicación y los puntos de la ruta, aunque use WhatsApp o Maps o apague la pantalla.
- **Funciones del teléfono.** La cámara y la galería sirven para las fotos de la entrega. Los PDF se descargan. Los enlaces a Google Maps, Waze, WhatsApp y llamadas se abren en su app.

## Compilación

GitHub Actions compila las dos apps en cada cambio a `main` y publica una versión nueva. Se puede ver en el workflow `.github/workflows/compilar.yml`.

La llave de firma está solo en los secretos del repositorio. Las actualizaciones tienen que salir firmadas con la misma llave para instalarse encima.
