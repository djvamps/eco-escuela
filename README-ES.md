# Eco Escuela Soy Libre - Landing Page

Landing page persuasiva desarrollada con Astro para la Eco Escuela Soy Libre.

## 🎨 Características de Diseño

Esta landing page ha sido desarrollada siguiendo estrictamente el **Manual de Identidad Corporativa** de Eco Escuela Soy Libre:

### Colores Corporativos
- **Verde Oscuro** (#16673D) - PANTONE 3425 C
- **Verde Claro** (#7DA53C) - PANTONE 7744 C
- **Amarillo** (#FAB732) - PANTONE 1235 C
- **Rojo Tierra** (#C66A4D) - PANTONE 7594 C

### Tipografías
- **Poppins** (Light, Regular, Bold) - Para textos generales
- **Baloo Bhai 2** (Regular, Bold) - Para títulos y encabezados

### Elementos Incluidos
- ✅ Logo corporativo con slogan
- ✅ Navegación fija con efecto hover
- ✅ Hero section con gradiente corporativo
- ✅ Sección Misión y Visión con tarjetas
- ✅ Metodologías educativas (Waldorf, Montessori, Reggio Emilia)
- ✅ 16 actividades extraescolares con iconos
- ✅ Call-to-action persuasivo
- ✅ Footer completo con información de contacto
- ✅ Diseño responsive para móviles y tablets
- ✅ Animaciones y transiciones suaves
- ✅ Efectos hover en botones y enlaces

## 🚀 Instalación y Uso

### Requisitos Previos
- Node.js 18+ instalado
- npm o pnpm

### Comandos Disponibles

```bash
# Instalar dependencias (si es necesario)
npm install

# Iniciar servidor de desarrollo
npm run dev

# Construir para producción
npm run build

# Vista previa de la versión de producción
npm run preview
```

### Desarrollo Local

1. Navega al directorio del proyecto:
```bash
cd soy-libre-landing
```

2. Inicia el servidor de desarrollo:
```bash
npm run dev
```

3. Abre tu navegador en `http://localhost:4321`

## 📁 Estructura del Proyecto

```
soy-libre-landing/
├── public/
│   ├── Logoconslogan@144x.png    # Logo con slogan
│   └── Logoblanco@144x.png       # Logo blanco para fondos oscuros
├── src/
│   └── pages/
│       └── index.astro           # Página principal
├── astro.config.mjs              # Configuración de Astro
└── package.json
```

## 🎯 Secciones de la Landing Page

1. **Header/Navegación**: Logo + menú + botón CTA
2. **Hero**: Título principal con llamado a la acción
3. **Nuestra Esencia**: Misión y Visión en tarjetas
4. **Metodologías**: Badges de pedagogías utilizadas
5. **Actividades Extraescolares**: Grid con 16 actividades
6. **CTA Final**: Llamado a la acción para contacto
7. **Footer**: Información de contacto y redes sociales

## 🌐 Despliegue

### Opción 1: Vercel (Recomendado)
```bash
npm install -g vercel
vercel
```

### Opción 2: Netlify
```bash
npm run build
# Sube la carpeta dist/ a Netlify
```

### Opción 3: GitHub Pages
```bash
npm run build
# Configura GitHub Pages para usar la carpeta dist/
```

## 📝 Personalización

Para modificar el contenido:
1. Edita `/src/pages/index.astro`
2. Los colores están definidos en las variables CSS (`:root`)
3. Las fuentes se cargan desde Google Fonts

## 🎨 Manual de Identidad

El diseño respeta completamente el manual de identidad corporativa:
- Uso correcto de colores corporativos
- Tipografías Poppins y Baloo Bhai 2
- Zona de protección del logo respetada
- Versiones del logo utilizadas apropiadamente

## 📧 Contacto

Para más información sobre la escuela:
- Email: contacto@ecoescuelasoyllibre.edu.pe
- Teléfono: +51 999 999 999
- Ubicación: Lima Este, Perú

---

**Desarrollado con ❤️ usando Astro**
