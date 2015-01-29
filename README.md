# SlimFlash
Autre système de notification flash pour Slim Framework 

## Utilisation
```php
$flash = new \Core\Flash();
$flash->flash('error', 'Impossible de vous connecter.');
```

### Twig
```html
{% if flash.type is defined %}
    <div class="{{ flash.type }}">
        <strong>{{ flash.title }} : </strong> {{ flash.message }}
    </div>
{% endif %}
```
