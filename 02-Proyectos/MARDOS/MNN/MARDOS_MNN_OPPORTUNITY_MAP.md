---
tipo: sistema
proyecto: MNN
estado: activo
actualizado: 2026-09-23
---

# MARDOS MNN Opportunity Map

## Propósito

Este documento no es un área más: es el mapa de cómo se conectan todas las áreas de MNN entre sí. El objetivo es poder pasar de una frase como *"esta empresa está relacionada con MNN"* a una frase como:

> "Esta empresa está desarrollando X, trabaja con Y, tiene presencia en Z, está entrando en determinada fase y puede tener una necesidad que MARDOS podría resolver."

Eso solo es posible si las notas están conectadas, no aisladas. La cadena de relación es:

```
PERSONAS
   ↓
EMPRESAS
   ↓
PROYECTOS
   ↓
LUGARES
   ↓
EVENTOS
   ↓
OPORTUNIDADES
   ↓
ACCIONES
   ↓
RELACIONES
```

## Cómo se traduce en la bóveda

| Eslabón | Dónde vive |
|---|---|
| Personas | [[04_contactos/00_contactos]] — una nota por persona cuando el volumen lo justifique |
| Empresas | [[08_mapa_empresarial/00_mapa_empresarial]] |
| Proyectos | [[02_inteligencia/00_inteligencia]] (proyectos del propio desarrollo) y notas de empresa cuando el proyecto es de un actor concreto |
| Lugares | [[07_mapa_fisico/00_mapa_fisico]] y sus notas por zona |
| Eventos | [[06_agenda/00_agenda]] |
| Oportunidades | [[05_oportunidades/00_oportunidades]] |
| Acciones | [[09_reuniones_acciones/00_reuniones_acciones]] |
| Relaciones | enlaces `[[...]]` entre las notas anteriores — no es una carpeta propia, es el resultado de enlazar bien |

## Regla de enlazado

Cuando una nota nueva (un contacto, una empresa, una oportunidad, una acción) tiene relación con otra ya existente, se enlaza con `[[...]]` en el momento de crearla, no después. Una oportunidad sin empresa enlazada, o una acción sin contacto enlazado, es una nota incompleta.

## Estado

Sistema definido el 23/09/2026, sin datos todavía — se irá poblando a medida que 02 a 09 tengan contenido real. Revisar este mapa cada vez que se detecte un patrón (varias oportunidades apuntando al mismo actor, varios contactos en la misma empresa) y dejarlo explícito aquí como **INTERPRETACIÓN**, no solo en las notas individuales.
