# AMAC · Bolsa de trabajo

Entrega 2 del proyecto final: maquetación en HTML y CSS de la plataforma de empleo de AMAC para personas adultas mayores, basada en nuestro prototipo de Figma.

- **Sitio publicado:** https://PONER-AQUI-LA-URL.vercel.app
- **Repositorio:** https://github.com/amauryperez-glitch/amac-web

## Integrantes

| Integrante | Qué hizo |
|---|---|
| Amaury Pérez Garza | Creó el repositorio y la estructura de carpetas. Hizo `variables.css`, `base.css`, `layout.css` y `componentes.css`, y los estilos de tablet y escritorio. |
| Juan Collado | Hizo las páginas `login.html`, `mis-solicitudes.html`, `vacante.html`, `registro-candidato.html` y `confirmacion.html`. |
| Carlos Aguilar | Hizo las páginas `index.html` (listado, buscador y filtros) y `empresa-vacantes.html`. |

## Páginas

| Archivo | Pantalla |
|---|---|
| `index.html` | Listado de vacantes con buscador y filtros |
| `vacante.html` | Detalle de la vacante con "Postularme" y "Llamar" |
| `confirmacion.html` | Confirmación de postulación enviada (extra, viene del Figma) |
| `mis-solicitudes.html` | Mis solicitudes con distintos estatus y "Cancelar" |
| `login.html` | Inicio de sesión |
| `registro-candidato.html` | Registro de candidato |
| `empresa-vacantes.html` | Panel de vacantes de la empresa |

## Paleta de colores

| Variable | Color | Uso |
|---|---|---|
| `--color-primario` | `#202945` | Azul marino AMAC: textos, pie de página, botón oscuro |
| `--color-acento` | `#ff815c` | Coral AMAC: botón principal y foco |
| `--color-acento-oscuro` | `#f26a42` | Coral al pasar el mouse |
| `--color-azul-claro` | `#cae4ef` | Fondos de cajas e inicio de sesión |
| `--color-durazno` | `#fddaad` | Etiqueta "En revisión" / "Pausada" |
| `--color-texto` | `#202945` | Texto normal |
| `--color-texto-suave` | `#4a5068` | Texto secundario |
| `--color-fondo` | `#ffffff` | Fondo |
| `--color-borde` | `#d5d8e0` | Bordes de tarjetas |
| `--color-verde` / `--color-verde-claro` | `#15803d` / `#dcf5e3` | Estatus "Aceptada" / "Activa" |
| `--color-rojo` / `--color-rojo-claro` | `#b91c1c` / `#fde8e8` | Estatus "Rechazada" |
| `--color-gris-claro` | `#e4e6eb` | Estatus "Cerrada" |

El botón coral lleva texto azul marino (no blanco) para cumplir el contraste mínimo de 4.5:1.

## Tipografía

| Variable | Valor |
|---|---|
| `--fuente-titulos` | Libre Baskerville (títulos) |
| `--fuente-base` | Work Sans (texto) |
| `--texto-base` | `1.125rem` (18 px) |
| `--texto-h3` | `1.25rem` |
| `--texto-h2` | `1.375rem` |
| `--texto-h1` | `1.75rem` |

Espaciados: `--espacio-s` 0.5rem, `--espacio-m` 1rem, `--espacio-l` 1.5rem. Bordes redondeados: `--radio` 0.5rem.

## Componentes reutilizables

Cada uno está escrito una sola vez en `css/componentes.css` y en la Entrega 3 será un componente de React.

| Clase CSS | Componente React | Dónde se usa |
|---|---|---|
| `.boton` (`--primario`, `--secundario`, `--oscuro`, `--chico`) | `<Boton />` | Todas las páginas |
| `.tarjeta` | `<TarjetaVacante />`, `<TarjetaSolicitud />` | Listado, mis solicitudes, panel de empresa |
| `.etiqueta` (`--revision`, `--aceptada`, `--rechazada`, `--cerrada`) | `<EtiquetaEstatus />` | Mis solicitudes, panel de empresa |
| `.campo` | `<CampoFormulario />` | Login, registro, buscador |
| `.grupo` y `.opcion` | `<GrupoOpciones />` | Filtros, registro, postulación |
| `.buscador` | `<Buscador />` | Listado de vacantes |
| `.filtros` | `<Filtros />` | Listado de vacantes |
| `.info-vacante` y `.dato` | `<InfoVacante />` | Detalle de vacante |
| `.aviso` | `<Aviso />` | Detalle de vacante (llamar a la empresa) |
| `.panel` | `<Panel />` | Inicio de sesión |
| `.confirmacion` | `<Confirmacion />` | Postulación enviada |
| `.enlace-volver` | `<EnlaceVolver />` | Detalle de vacante |
| Encabezado (`.encabezado`, `.menu`) | `<Encabezado />` | Todas las páginas |
| Pie de página (`.pie`) | `<Pie />` | Todas las páginas |

## Capturas

### index.html en celular

![index.html en celular](img/index-celular.png)

### index.html en escritorio

![index.html en escritorio](img/index-escritorio.png)

### Lighthouse – Accessibility

![Puntaje de Lighthouse](img/lighthouse.png)
