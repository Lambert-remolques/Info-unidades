# Guia de identidad visual Lambert

Este documento resume criterios de estilo extraidos del manual de marca Lambert y sirve como referencia para disenar interfaces, piezas digitales y componentes del banco de unidades.

## Personalidad visual

La identidad Lambert se apoya en una estetica industrial, comercial y directa. Debe transmitir robustez, confianza, movimiento y cercania con el mundo del transporte.

La marca debe verse:

- Fuerte.
- Tecnica.
- Clara.
- Comercial.
- Moderna, pero no futurista.
- Industrial, pero prolija.
- Cercana al rubro transporte, acoplados y remolques.

Evitar estilos demasiado decorativos, blandos, genericos de startup o con gradientes excesivos. Lambert funciona mejor con planos limpios, contraste fuerte y elementos graficos bien definidos.

## Paleta de colores

Colores principales:

```css
--verde-lambert: #159947;
--rojo-lambert: #da251d;
--negro-lambert: #262626;
--gris-oscuro: #333333;
--gris-claro: #e6e6e6;
--blanco: #ffffff;
```

Uso recomendado:

- Verde `#159947`: color principal de marca. Usar en titulos, botones principales, lineas decorativas, iconos, estados activos y fondos destacados.
- Rojo `#da251d`: color secundario o acento. Usar con moderacion para detalles, alertas, etiquetas o llamados puntuales.
- Negro `#262626`: fondos oscuros, textos principales y tarjetas destacadas.
- Gris oscuro `#333333`: textos secundarios o fondos alternativos.
- Gris claro `#e6e6e6`: fondos suaves, separadores y areas neutras.
- Blanco `#ffffff`: base principal para claridad, aire y jerarquia.

## Tipografia

El logo utiliza Univers y debe reservarse exclusivamente para el logo y slogan.

Para textos de comunicacion e interfaces se recomienda Montserrat.

Jerarquia tipografica:

- Primer nivel: Montserrat Black Italic, imprenta mayuscula, color verde o blanco segun el fondo.
- Segundo nivel: Montserrat Bold, con tamano aproximado a la mitad del primer nivel.
- Tercer nivel: Montserrat Medium, para parrafos, descripciones y textos funcionales.

Ejemplo CSS:

```css
.titulo-principal {
  font-family: "Montserrat", sans-serif;
  font-weight: 900;
  font-style: italic;
  text-transform: uppercase;
  color: #159947;
}

.subtitulo {
  font-family: "Montserrat", sans-serif;
  font-weight: 700;
}

.texto {
  font-family: "Montserrat", sans-serif;
  font-weight: 500;
}
```

## Composicion

La composicion Lambert usa mucho espacio blanco y una jerarquia clara. Los elementos no deben sentirse apretados.

Recursos visuales frecuentes:

- Margenes amplios.
- Fondos blancos.
- Titulos alineados a la izquierda.
- Linea vertical verde antes del titulo de seccion.
- Titulos de seccion en verde, italic y bold.
- Subtitulo debajo del titulo, tambien en verde y con menor peso visual.
- Bloques o tarjetas con bordes finos verdes.
- Imagenes reales de unidades como apoyo comercial.

Patron sugerido para encabezados de seccion:

```html
<div class="section-label">
  <span></span>
  <div>
    <strong>Identidad visual</strong>
    <p>tipografia y paleta de colores</p>
  </div>
</div>
```

La linea vertical verde funciona como firma grafica. Conviene usarla en secciones importantes y no repetirla en exceso.

## Logo

El logo debe conservar un area de seguridad. No debe quedar pegado a bordes, textos, botones, imagenes u otros elementos.

Buenas practicas:

- Dejar aire alrededor del logo.
- Usarlo sobre blanco en version verde/roja.
- Usarlo sobre verde o fondo oscuro en version blanca.
- No deformarlo.
- No encerrarlo demasiado justo.
- No ubicarlo muy cerca de otros logos o textos.

La distancia minima alrededor del logo debe respetar la unidad de seguridad indicada en el manual.

## Iconografia

Los iconos deben ser siempre de contorno, nunca plenos.

Reglas:

- Iconos verdes sobre fondo claro.
- Iconos blancos sobre fondo verde u oscuro.
- Trazo simple, tecnico y legible.
- Evitar iconos rellenos o muy ilustrativos.
- Usarlos para organizar informacion: DNI, ejes, peso, banco, cuotas, beneficios, pasos o categorias.

Para interfaces HTML conviene usar SVG lineal o una libreria de iconos de trazo, manteniendo el estilo de contorno.

## Fotografia

La marca utiliza fotos reales de unidades, camiones, acoplados, rutas y aplicaciones concretas.

Estilo recomendado:

- Producto real.
- Transporte en contexto.
- Rutas, campo, carga e industria.
- Contraste alto.
- Recortes limpios.
- Posibilidad de combinar imagenes con placas verdes, negras o blancas.

Evitar:

- Fotos genericas demasiado stock.
- Imagenes muy oscuras donde no se reconozca el producto.
- Efectos excesivos.
- Fondos decorativos que compitan con la unidad.

## Botones y componentes

Los botones deben sentirse solidos, simples y con buen contraste.

Boton principal:

- Fondo verde.
- Texto blanco.
- Montserrat Bold.
- Mayusculas.
- Bordes levemente redondeados.
- Hover con verde mas oscuro, negro o sombra leve.

Boton secundario:

- Fondo blanco.
- Borde verde.
- Texto verde.
- Hover verde con texto blanco.

Evitar botones demasiado redondeados, suaves, pastel o con decoracion innecesaria.

## Aplicacion al banco de unidades

Para el HTML del banco de unidades, la direccion visual recomendada es:

- Fondo principal blanco o gris muy claro.
- Header oscuro o verde con logo blanco.
- Titulo grande: `BANCO DE UNIDADES` en Montserrat Black Italic.
- Categorias como chips o botones solidos, no excesivamente redondeados.
- Tarjetas tecnicas limpias con borde fino, sombra suave y acento verde.
- Iconos de contorno para cada unidad o categoria.
- Boton `VER FICHA TECNICA` fuerte, en verde o negro.
- Detalles rojos solo como acentos pequenos, no como color dominante.

El sitio debe sentirse como una herramienta comercial interna/profesional: mas catalogo tecnico que landing publicitaria.

## Prompt base para asistir diseno HTML

```text
Disenar una interfaz web para Lambert respetando su identidad visual. Usar una estetica industrial, limpia y profesional. La paleta principal debe ser verde #159947, rojo #da251d, negro #262626, gris oscuro #333333, gris claro #e6e6e6 y blanco. Usar Montserrat como tipografia general. Los titulos principales deben estar en Montserrat Black Italic, en mayusculas y color verde o blanco segun el fondo. Los subtitulos deben usar Montserrat Bold y los textos Montserrat Medium.

La composicion debe usar mucho espacio blanco, jerarquias claras, lineas verticales verdes como recurso de seccion, tarjetas limpias con bordes sutiles y botones solidos. Los iconos deben ser siempre de contorno, no rellenos, verdes sobre fondo claro y blancos sobre fondo oscuro o verde. El logo debe tener aire alrededor y no debe deformarse ni quedar pegado a otros elementos.

El resultado debe verse tecnico, robusto, comercial e industrial, alineado al rubro de acoplados, semirremolques, carrocerias y bitrenes. Evitar estilos demasiado decorativos, gradientes exagerados, formas blandas, colores fuera de marca o estetica generica de startup.
```
