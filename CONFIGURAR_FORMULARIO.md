# 📧 Configuración del Formulario de Contacto

El formulario de contacto está configurado para funcionar con **Formspree**, un servicio gratuito que envía los mensajes del formulario directamente a tu email.

## 🚀 Pasos para Activar el Formulario

### 1. Crear Cuenta en Formspree

1. Ve a [https://formspree.io/register](https://formspree.io/register)
2. Regístrate con tu email (puedes usar Google/GitHub)
3. Verifica tu cuenta de email

### 2. Crear un Nuevo Formulario

1. Una vez dentro, haz clic en **"+ New Form"**
2. Dale un nombre: `Fundación Santo Angel - Contacto`
3. Se generará un **Form ID** que se ve así: `mxxxxxxx`

### 3. Configurar el Formulario en tu Sitio

1. Abre el archivo `index.html`
2. Busca la línea que dice:
   ```html
   <form id="contactForm" action="https://formspree.io/f/TU_FORM_ID" method="POST">
   ```
3. Reemplaza `TU_FORM_ID` con el ID que te dio Formspree
4. Ejemplo:
   ```html
   <form id="contactForm" action="https://formspree.io/f/mxxxxxxx" method="POST">
   ```

### 4. Guardar y Subir los Cambios

```bash
git add index.html
git commit -m "Configurar formulario de contacto con Formspree"
git push
```

### 5. Probar el Formulario

1. Ve a tu sitio web
2. Llena el formulario de contacto
3. Envía el mensaje
4. La primera vez, Formspree te pedirá confirmar tu email
5. ¡Los siguientes mensajes llegarán directamente a tu bandeja de entrada!

## ✨ Características Incluidas

✅ **Validación de campos** - Nombre, email y mensaje son obligatorios  
✅ **Protección anti-spam** - Campo honeypot oculto  
✅ **Mensajes de estado** - Confirmación visual de éxito/error  
✅ **Responsive** - Funciona en móvil y desktop  
✅ **Sin recarga de página** - Envío con AJAX  
✅ **Asunto personalizado** - Los emails llegan con un asunto claro  

## 📊 Plan Gratuito de Formspree

- ✅ 50 envíos por mes (gratis)
- ✅ Sin tarjeta de crédito requerida
- ✅ Notificaciones por email
- ✅ Sin marca de agua

## 🔄 Alternativas (si prefieres otra opción)

### EmailJS
- Hasta 200 emails/mes gratis
- URL: [https://www.emailjs.com](https://www.emailjs.com)

### Web3Forms
- Sin límites de envíos
- URL: [https://web3forms.com](https://web3forms.com)

### GetForm
- Hasta 50 envíos/mes gratis
- URL: [https://getform.io](https://getform.io)

## 🛠️ Personalización Adicional

En el panel de Formspree puedes:
- Cambiar el email de destino
- Configurar auto-respuestas
- Agregar webhooks
- Exportar datos a Google Sheets
- Ver estadísticas de envíos

## ❓ Problemas Comunes

**El formulario no envía:**
- Verifica que hayas reemplazado `TU_FORM_ID` correctamente
- Asegúrate de haber verificado tu email en Formspree

**No recibo los emails:**
- Revisa tu carpeta de spam
- Confirma que el email en Formspree sea el correcto

**Límite de 50 mensajes alcanzado:**
- Actualiza a un plan pago de Formspree ($10/mes)
- O cambia a Web3Forms (sin límites)

## 📞 Soporte

Si tienes problemas, puedes:
- Revisar la documentación: [https://help.formspree.io](https://help.formspree.io)
- Contactar soporte de Formspree
- Modificar el código para usar otra alternativa
