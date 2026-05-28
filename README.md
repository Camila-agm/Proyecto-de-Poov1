# TESE | Posgrados — Proyecto Web

Sitio web informativo y portal de estudiantes del Tecnológico de Estudios Superiores de Ecatepec (TESE), desarrollado con HTML y CSS puro.

---

## Estructura de carpetas

```
TESE_Posgrados/
│
├── index.html                  ← Página de inicio
│
├── css/
│   └── estilos.css             ← Hoja de estilos global compartida
│
├── js/
│   └── main.js                 ← Lógica de acordeón y portal
│
├── image/                      ← Imágenes e íconos de programas
│   ├── logo_edomex.png
│   ├── logo_tese.jpg
│   ├── Imagen1.jpg
│   ├── Convocatoria.jpg
│   ├── quimica.png
│   ├── bioquimica.png
│   ├── energia.png
│   ├── gestion.png
│   ├── mecatronica.png
│   ├── sistemas.png
│   └── doctorado.png
│
├── pages/
│   ├── oferta.html             ← Catálogo de programas (grid)
│   ├── convocatoria.html       ← Calendario de admisión
│   ├── estudiantes.html        ← Login del portal
│   ├── portal_inicio.html      ← Datos generales del alumno
│   ├── portal_historial.html   ← Historial académico (kardex)
│   ├── portal_semestre.html    ← Semestre actual, horarios y tira
│   ├── quimica.html            ← M. en Ciencias en Ing. Química
│   ├── bioquimica.html         ← M. en Ciencias en Ing. Bioquímica
│   ├── energia.html            ← M. en Eficiencia Energética
│   ├── gestion.html            ← M. en Gestión Administrativa
│   ├── mecatronica.html        ← M. en Ciencias en Ing. Mecatrónica
│   ├── sistemas.html           ← M. en Ing. en Sistemas Comp.
│   └── doctorado.html          ← Doctorado en Ciencias en Ing. Bioquímica
│
└── database/
    └── tese_posgrados.sql      ← Script completo de la base de datos
```

---

## Cómo abrir el proyecto

1. Abrir `index.html` directamente en un navegador web.
2. Todas las páginas están enlazadas con rutas relativas; no requiere servidor.

## Credenciales de demostración (portal)

| Campo    | Valor     |
|----------|-----------|
| Usuario  | alumno01  |
| Contraseña | 1234    |

---

## Base de datos (GitHub / MySQL)

El archivo `database/tese_posgrados.sql` contiene:
- 13 tablas normalizadas (programas, materias, estudiantes, grupos, calificaciones, tesis…)
- 3 vistas de consulta frecuente
- Datos de ejemplo (seed)

Para importar en MySQL:
```sql
mysql -u root -p < database/tese_posgrados.sql
```

---

## Tecnologías usadas

- HTML5 semántico
- CSS3 con variables (`:root`)
- JavaScript vanilla (sin frameworks)
- Font Awesome 6 (iconos de redes sociales)
