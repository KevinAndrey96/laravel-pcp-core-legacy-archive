# PCP: núcleo Laravel 8 de la plataforma mayorista (archivo histórico)

![Estado: archivo histórico](https://img.shields.io/badge/Estado-archivo%20hist%C3%B3rico-lightgrey) ![Laravel 8](https://img.shields.io/badge/Laravel%208-FF2D20) ![PHP 7.3+](https://img.shields.io/badge/PHP%207.3%2B-777BB4) ![MySQL](https://img.shields.io/badge/MySQL-4479A1)

> [!NOTE]
> Proyecto base en Laravel 8 de la plataforma mayorista PCP (marzo de 2021), del que se derivaron el portal de distribuidores y el de clientes. El producto continúa en **[pcp-industrial-wholesale-ecommerce](https://github.com/KevinAndrey96/pcp-industrial-wholesale-ecommerce)**, que reúne todos sus componentes con documentación actualizada.

## Qué contiene

- Esqueleto de Laravel 8 con configuración de CORS, proxy y Guzzle.
- Migraciones iniciales de usuarios, restablecimiento de contraseña y trabajos fallidos.
- Estructura de rutas, vistas y pruebas de PHPUnit de la plantilla.

## Stack original

| Componente | Tecnología |
| :--- | :--- |
| Framework | Laravel 8 |
| Lenguaje | PHP 7.3 u 8.0 |
| Base de datos | MySQL |
| Assets | Laravel Mix |

## Ejecutarlo localmente

```bash
cp .env.example .env    # completa DB_* y MAIL_* con valores locales
composer install        # vendor/ no se versiona
php artisan key:generate
php artisan migrate
php artisan serve       # http://localhost:8000
```

Requiere PHP 7.4 u 8.0, Composer 2 y MySQL. Laravel 8 dejó de recibir parches de seguridad en enero de 2023.

## Estado del repositorio

- Se conserva sin cambios funcionales como referencia del código original (2021).
- No recibe actualizaciones de dependencias; el mantenimiento ocurre en [pcp-industrial-wholesale-ecommerce](https://github.com/KevinAndrey96/pcp-industrial-wholesale-ecommerce).
- En noviembre de 2026 se depuró el historial completo: se retiraron `vendor/` (6.854 archivos de Composer) y el `.env` con la `APP_KEY`. Todos los commits conservan su fecha original.

## Autoría

Kevin Andrey Herrera Silva ([@KevinAndrey96](https://github.com/KevinAndrey96)).

## Licencia

Código desarrollado para un cliente y publicado como muestra de portafolio. No incluye licencia de código abierto: todos los derechos reservados.
