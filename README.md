# sonificacion-aguaNL
Sonificación de concesiones de agua en estado de Nuevo León usando datos de la iniciativa "Rastreo del agua en Nuevo León".

Fue presentada en el LabNL Lab Cultural Ciudadano como parte del FestiLab '22.

<h3 align="center">
  <a href="https://github.com/MikeMorenoDSP/sonificacion-aguaNL/archive/refs/heads/main.zip">Descarga el código en .zip</a>
</h3>

## 🖥️ Software 
Esta sonificación fue programada en [pure data vanilla versión 0.52-1](https://puredata.info/).

Se requiere uso de la librería [else versión 1.0-rc4](https://github.com/porres/pd-else/releases/tag/v1.0-rc4) para la parte sonora y [GEM](https://github.com/umlaeute/Gem) para la parte visual reactiva.

## 🔊 Sonificación
Se tomaron los datos de un archivo .csv del repositorio [MapatonAgua](https://github.com/cesar-xyz/MapatonAgua/blob/main/files/UnionRegiosDOF.csv).

En él se consideraron las siguientes columnas para relacionarlo a diferentes parámetros musicales:
- **Fecha de registro:** orden de lectura para cada concesión.
- **Volumen anual en m^3:** longitud de frase melódica/rítmica.
- **Municipio:** frase rítmica.
- **Acuífero:** frase melódica.
- **Titular:** dinámica (piano, mezo, forte) y otros parametros de instrumento.
- **Uso Amparado:** determina el tipo de instrumento a usar.
    1. Acuacultura (9 - 0.01%): clicks senoidales.
    2. Agrícola (1 – 47%): senoidales.
    3. Agroindustrial (10 - 0.01%): drum machine.
    4. Diferentes usos (2 – 17%): ruido blanco.
    5. Doméstico (4 – 10%): síntesis aditiva con LPG.
    6. Generación de energía eléctrica (8 – 0.01%): unfiltered sawtooths.
    7. Industria (5 – 7%): drum machine.
    8. Político Urbano (7 – 3%): unfiltered sawtooths.
    9. Pecuario (3 – 11%): karplus síntesis.
    10. Servicios (6 – 4%): clicks.

## 🔗 Enlaces
- Sitio del proyecto: https://sites.google.com/view/acuiferosnl/inicio
- Mapa interactivo: https://cesar-xyz-mapatonagua-appapp-vp0zii.streamlit.app/
- Repositorio Mapaton de Agua NL: https://github.com/cesar-xyz/MapatonAgua
- Publicación de FestiLab '22: https://www.instagram.com/p/Cl4-L0fsgEz/