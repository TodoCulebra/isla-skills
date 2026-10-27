# Isla Skills

**English** · [Español](#español)

Six Claude skills for running a small business: the same written rules our own e-bike rental business in Culebra,
Puerto Rico, works by every day. Free to use and change (MIT licence).

Isla Tech runs AI for small businesses in Puerto Rico. These are the routines underneath that work, written so
anyone can use them.

## The skills

| Skill | What it does | Use it when |
|---|---|---|
| [clear-texts](skills/clear-texts/SKILL.md) | Texts people read in one glance: headline, one blank line per item, at most 5 items, one ask | you text a customer, partner or your crew |
| [three-sentence-email](skills/three-sentence-email/SKILL.md) | Three sentences, best proof first, one ask on its own line, follow-ups on day 4 and day 10 | you write outreach or a follow-up |
| [three-visit-habit](skills/three-visit-habit/SKILL.md) | Turns first-timers into regulars in three visits (the red napkin) | you plan a promo, a thank-you message or a loyalty idea |
| [price-before-you-run](skills/price-before-you-run/SKILL.md) | Says the dollar price, who pays and whether it hits a card before any paid AI run | you are about to spend API credits |
| [one-tone-carousel](skills/one-tone-carousel/SKILL.md) | Carousel posts with one tone per slide: rule, proof, mistake, cost, fix, payoff | you make an Instagram or LinkedIn carousel |
| [page-check](skills/page-check/SKILL.md) | A phone-first page check with numbers: tap targets, text sizes, nothing clipped or covered | you ship or edit a web page |

## Install

**Claude Code** (all six at once):

```
/plugin marketplace add TodoCulebra/isla-skills
/plugin install isla-skills@isla-skills
```

**Claude Code** (one skill): copy its folder into `~/.claude/skills/` (all your projects) or `.claude/skills/`
(one project).

**Claude app** (claude.ai or Claude Desktop): zip one skill folder, then upload the `.zip` in Settings, under Skills.

Then ask in plain words: "draft a text to my crew about tomorrow's schedule", "check this page on a phone",
"how much will this run cost?". Claude picks the skill that fits.

## How each skill is built

Each folder holds one `SKILL.md`: a short header (`name`, `description`) that tells Claude when to use it, then the
rules, a template and a worked example. The format follows the open [Agent Skills spec](https://agentskills.io/specification),
so other assistants that read `SKILL.md` can use them too.

## Change them

Fork the repo and make the rules yours: your prices, your gifts, your voice. If a rule helped you, or failed you,
open an issue and tell us what happened.

---

## Español

**[English](#isla-skills)** · Español

Seis skills de Claude para operar un negocio pequeño: las mismas reglas escritas que usa todos los días nuestro propio
negocio de alquiler de e-bikes en Culebra, Puerto Rico. Gratis para usar y cambiar (licencia MIT).

Isla Tech opera la IA de los pequeños negocios de Puerto Rico. Estas son las rutinas detrás de ese trabajo, escritas
para que cualquiera las pueda usar.

### Las skills

| Skill | Qué hace | Úsala cuando |
|---|---|---|
| [clear-texts](skills/clear-texts/SKILL.md) | Mensajes que se leen de un vistazo: un titular, una línea en blanco entre puntos, máximo 5 puntos, un pedido | le escribes a un cliente, un socio o tu equipo |
| [three-sentence-email](skills/three-sentence-email/SKILL.md) | Tres oraciones, la mejor prueba primero, un pedido en su propia línea, seguimiento el día 4 y el día 10 | escribes un email a alguien nuevo o das seguimiento |
| [three-visit-habit](skills/three-visit-habit/SKILL.md) | Convierte clientes nuevos en clientes fijos en tres visitas (la servilleta roja) | planificas una promoción, un mensaje de gracias o una idea de lealtad |
| [price-before-you-run](skills/price-before-you-run/SKILL.md) | Dice el precio en dólares, quién paga y si toca una tarjeta antes de cualquier corrida de IA que cueste | vas a gastar créditos de API |
| [one-tone-carousel](skills/one-tone-carousel/SKILL.md) | Carruseles con un solo tono por lámina: regla, prueba, error, costo, arreglo, resultado | haces un carrusel de Instagram o LinkedIn |
| [page-check](skills/page-check/SKILL.md) | Revisión de páginas pensada para el teléfono, con números: botones, tamaños de letra, nada cortado ni tapado | publicas o cambias una página web |

### Instalar

**Claude Code** (las seis a la vez):

```
/plugin marketplace add TodoCulebra/isla-skills
/plugin install isla-skills@isla-skills
```

**Claude Code** (una sola): copia su carpeta a `~/.claude/skills/` (todos tus proyectos) o a `.claude/skills/`
(un proyecto).

**App de Claude** (claude.ai o Claude Desktop): comprime la carpeta de una skill en `.zip` y súbela en Ajustes, en Skills.

Después pide en palabras normales: "escríbele un mensaje a mi equipo sobre el horario de mañana", "revisa esta página
en el teléfono", "¿cuánto va a costar esta corrida?". Claude escoge la skill que aplica.

Las skills están escritas en inglés y funcionan igual en español: pídele a Claude la respuesta en español.

### Cámbialas

Haz un fork y hazlas tuyas: tus precios, tus regalos, tu voz. Si una regla te ayudó, o te falló, abre un issue y
cuéntanos qué pasó.

---

Isla Tech LLC · [islatechpr.com](https://islatechpr.com)
