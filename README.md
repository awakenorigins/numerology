# Numerology — Motivational Number System

> Calculate and interpret core numerology numbers from name + birth date: Destiny, Personality, Soul Urge, Hidden Agenda, Divine Purpose, and more.

[![OpenClaw Skill](https://img.shields.io/badge/OpenClaw-Skill-blueviolet)](https://github.com/NachaFromMars)
[![Languages](https://img.shields.io/badge/Lang-EN%20%7C%20VI%20%7C%20FR%20%7C%20DE%20%7C%20JP-informational)](/)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)

## Overview

**Numerology** is an OpenClaw skill that derives and interprets the seven core motivational numbers from a person's full name and date of birth. It supports multiple languages and provides concise, AI-ready personality and destiny profiles.

## Core Numbers

| Number | Source | Meaning |
|---|---|---|
| **Destiny** | Birth date digits summed | Core drive, career direction (strongest lifelong influence) |
| **Personality** | All name letters (reduced) | Inner character, how you process the world |
| **Attitude** | Month + Day digits | First impression, dominant in ages 0–35 |
| **Character** | Consonants of full name | Public persona, social face |
| **Soul Urge** | Vowels of full name | Deepest desire, what you truly want |
| **Hidden Agenda** | Hidden motivations | Unconscious wants others don't see |
| **Divine Purpose** | Destiny + Character | Life's overarching mission |

## Calculation Logic

```
Destiny    = reduce(sum(digits(MM + DD + YYYY)))  → 1–9 or master 11/22
Character  = reduce(sum(consonant_values(full_name)))
Soul Urge  = reduce(sum(vowel_values(full_name)))
Hidden     = reduce(sum(hidden_letter_values(full_name)))
Divine     = reduce(Destiny + Character)
```

Master numbers 11 and 22 are **not** reduced further.

## Usage (OpenClaw)

Trigger with natural language:

> "Tính thần số học cho Nguyễn Văn Hùng sinh 15/03/1990"
> "Numerology reading for John Smith born April 7, 1985"

The skill returns all seven numbers with concise interpretations.

## Language Support

Vietnamese · English · French · German · Japanese · Spanish · (+ extensible)

## Files

| File | Purpose |
|---|---|
| `SKILL.md` | OpenClaw entrypoint |
| `index.html` | Main calculator (English) |
| `index-vietnamese.html` | Calculator with Vietnamese name support |
| `scripts/` | Calculation scripts |

## Trigger Keywords (OpenClaw)

`thần số học`, `numerology`, `số chủ đạo`, `destiny number`, `soul urge`, `life path`, `con số vận mệnh`, `divine purpose`, `hidden agenda`

## Credits

Based on the open-source [motivational-numerology](https://github.com/evoluteur/motivational-numerology) project by Olivier Giulieri (MIT License). Extended with Vietnamese language support and OpenClaw agent integration.

---

Part of the [NachaFromMars](https://github.com/NachaFromMars) OpenClaw skill ecosystem.
