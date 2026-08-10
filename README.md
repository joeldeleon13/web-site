# Lois Profesional

Página estática lista para publicar en Vercel y usar como enlace de Instagram.

## Publicar en Vercel

1. Sube esta carpeta a un repositorio nuevo de GitHub.
2. En Vercel, elige **Add New → Project** e importa ese repositorio.
3. No selecciones ningún framework: es una página estática.
4. Pulsa **Deploy** y copia la URL pública a la biografía de Instagram.

## Activar Stripe

En `index.html`, busca `stripePaymentLinks` y pega los dos enlaces públicos que Stripe genere:

```js
const stripePaymentLinks = {
  strategic: 'https://buy.stripe.com/...',
  immigration101: 'https://buy.stripe.com/...'
};
```

Guarda los cambios y haz `git push`; Vercel publicará la actualización automáticamente. Nunca incluyas claves secretas de Stripe.
