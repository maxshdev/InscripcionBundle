# InscripcionBundle

## Objetivos
- Proveer de un modulo para distintos tipos de inscripciones.
- Usuario editor, podrá crear inscripciones y cada editor agregará un nuevo modulo de inscripción según sea conveniente.
- Los usuarios deberan completar un formulario para inscribirse aceptando todas las condiciones.
- El usuario admin tendra acceso a todos los reportes.

## Installation

### Usando Composer

Agregar la siguiente linea a tú `composer.json` archivo:

### Support Symfony 2.7.* + Include Boostrap 3

```json
"require": {
    ...
    "maxshdev/inscripcion": "1.0.*@dev",
}
```

Executar:

```cli
php composer.phar update "maxshdev/inscripcion"
```
o
```cli
php composer update
```

Registrar el paquete dentro de la clase `AppKernel.php`:

```php
// ...
new maxshdev\Bundle\InscripcionBundle\InscripcionBundle(),
```

Registrar el bundle:

```php
// app/AppKernel.php
public function registerBundles()
{
    $bundles = array(
        // ...
        new maxshdev\Bundle\InscripcionBundle\InscripcionBundle(),
    );
    // ...
}
```

## Configura tú config.yml
```yaml

imports:
    # MaxSHDevInscripcionBundle services
    - { resource: "@InscripcionBundle/Resources/config/services.yml" }

    ...

```

## Author

MaxSHDev - max.shtefec@gmail.com