# 🎛️ Anta Knob

**¡Gracias adquirir tu AntaKnob!** El Anta Knob está diseñado para darte precisión, estilo y funcionalidad inmediata.

---
 
## 🚀 Instalación Rápida

El Anta Knob utiliza **VIA**, el estándar de la industria para periféricos custom. No necesitás instalar ningún software en tu PC; todo se configura desde el navegador.

### 📥 Paso 1: Descargar el Mapa
Necesitás el archivo de configuración para que VIA reconozca tu dispositivo.

👉 **[Hacé click acá para descargar el archivo .json](https://raw.githubusercontent.com/Antarestai/AntaKnob/refs/heads/main/antaknob/knob_via.json)** *(Si se abre como texto: Hacé Click Derecho > "Guardar como..." y guardalo en tu PC)*

---

### ⚙️ Paso 2: Configurar en VIA

1.  **Conectá** tu Anta Knob a la PC usando el cable USB-C.
2.  Ingresá a **[usevia.app](https://usevia.app)** (usar Google Chrome o Edge).
3.  Hacé click en el ícono de **Settings** (⚙️) arriba a la derecha.
4.  Activá la opción **"Show Design Tab"**.
5.  Hacé click en el ícono de **Design** (🖌️) que apareció a la izquierda.
6.  Hacé click en cargar y subi el archivo `.json` que descargaste.
7.  Vincula el AntKnob.

¡Listo! 🎉 Ahora deberías ver el diseño del Anta Knob en pantalla y podrás modificar las luces y funciones.

---

## 💡 Efectos de Iluminación

El Anta Knob incluye efectos exclusivos RGB. Podés cambiarlos desde la pestaña Iluminación en VIA.

---

## 🆘 Soporte

¿Tenés alguna duda o problema?
Contactame por Discord: **antarestai**

<button onclick="descargarDelGitHub()">Descargar knob_via.json</button>

<script>
async function descargarDelGitHub() {
  const url = 'https://api.github.com/repos/Antarestai/AntaKnob-Instrucciones/contents/knob_via.json?ref=main';
  
  try {
    const response = await fetch(url);
    const data = await response.json();
    const content = atob(data.content); // Decodifica base64
    
    // Crear descarga
    const blob = new Blob([content], { type: 'application/json' });
    const link = document.createElement('a');
    link.href = URL.createObjectURL(blob);
    link.download = 'knob_via.json';
    link.click();
  } catch (error) {
    console.error('Error:', error);
  }
}
</script>

---
*Diseñado y Fabricado por Antares.*



