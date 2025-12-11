# 📝 Instrucciones de Personalización

## Cómo Editar el Mapa de Google Maps

El mapa está ubicado en la sección "Encuéntranos" antes del footer. Para cambiarlo a tu ubicación específica:

### Paso 1: Obtener el código de inserción de Google Maps

1. Ve a [Google Maps](https://www.google.com/maps)
2. Busca la ubicación exacta de tu escuela
3. Haz clic en el botón **"Compartir"**
4. Selecciona la pestaña **"Insertar un mapa"**
5. Copia el código `<iframe>` que aparece

### Paso 2: Reemplazar el código en el archivo

1. Abre el archivo `/src/pages/index.astro`
2. Busca la línea que contiene: `<!-- Google Maps Embed - Reemplaza con tu ubicación específica -->`
3. Reemplaza el `src` del iframe con el que copiaste de Google Maps

**Ejemplo:**

```html
<iframe 
    src="TU_URL_DE_GOOGLE_MAPS_AQUI"
    allowfullscreen="" 
    loading="lazy" 
    referrerpolicy="no-referrer-when-downgrade"
    title="Ubicación de Eco Escuela Soy Libre">
</iframe>
```

---

## Cómo Editar el Botón Flotante de WhatsApp

El botón flotante de WhatsApp aparece en la esquina inferior derecha de todas las páginas.

### Cambiar el Número de Teléfono

1. Abre el archivo `/src/pages/index.astro`
2. Busca la línea que contiene: `<!-- Botón flotante de WhatsApp -->`
3. Encuentra el enlace que comienza con: `https://wa.me/51999999999`
4. Reemplaza `51999999999` con tu número de WhatsApp (incluye el código de país sin el símbolo +)

**Ejemplo para Perú (+51):**
- Si tu número es: +51 987 654 321
- Debes escribir: `https://wa.me/51987654321`

### Cambiar el Mensaje Predeterminado

El mensaje que aparece cuando alguien hace clic en el botón también se puede personalizar:

```html
<a href="https://wa.me/51987654321?text=Hola%2C%20me%20gustaría%20obtener%20más%20información%20sobre%20Eco%20Escuela%20Soy%20Libre"
```

- `%2C` = coma (,)
- `%20` = espacio
- Puedes usar un [codificador de URL](https://www.urlencoder.org/) para convertir tu mensaje personalizado

**Ejemplo:**
- Mensaje: "Hola, quiero información sobre las inscripciones"
- Codificado: `Hola%2C%20quiero%20informaci%C3%B3n%20sobre%20las%20inscripciones`

### Cambiar el Tooltip (Texto que aparece al pasar el mouse)

Busca esta línea:
```html
<span class="whatsapp-tooltip">¡Escríbenos por WhatsApp!</span>
```

Y cámbiala por el texto que prefieras:
```html
<span class="whatsapp-tooltip">¡Contáctanos ahora!</span>
```

---

## Otros Elementos Personalizables

### Cambiar Colores Corporativos

Si necesitas ajustar los colores, edita las variables CSS en la sección `:root` del archivo `/src/pages/index.astro`:

```css
:root {
    --verde-oscuro: #16673D;
    --verde-claro: #7DA53C;
    --amarillo: #FAB732;
    --rojo-tierra: #C66A4D;
}
```

### Cambiar Información de Contacto

Busca y reemplaza en todo el archivo:
- Email: `contacto@ecoescuelasoyllibre.edu.pe`
- Teléfono: `+51 999 999 999`
- Ubicación: `Lima Este, Perú`

### Agregar Enlaces de Redes Sociales

En la sección del footer, reemplaza los `#` con tus URLs reales:

```html
<a href="https://facebook.com/tuescuela">Facebook</a>
<a href="https://instagram.com/tuescuela">Instagram</a>
<a href="https://youtube.com/@tuescuela">YouTube</a>
```

---

## 🔧 Comandos Útiles

Después de hacer cambios:

```bash
# Ver los cambios en tiempo real
npm run dev

# Construir para producción
npm run build

# Vista previa de la versión de producción
npm run preview
```

---

## 💡 Consejos

1. **Siempre prueba los cambios localmente** con `npm run dev` antes de desplegar
2. **Guarda copias de seguridad** antes de hacer cambios importantes
3. **Verifica que los números de WhatsApp funcionen** haciendo clic en el botón
4. **Prueba el mapa en diferentes dispositivos** para asegurar que se vea bien en móviles

---

¿Necesitas ayuda? Consulta el archivo `README-ES.md` para más información.
