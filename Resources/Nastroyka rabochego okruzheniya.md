---
created: 2026-03-26
type: research
tags: [setup, vault, workflow]
sources: []
status: active
---

# Настройка рабочего окружения

## Контекст
Документация по настройке связки Obsidian + Claude Code. Всё что сделано и как это работает.

## Ключевые выводы
1. Vault живёт на F:\ObsidianVault — SSD, быстро, надёжно
2. Claude Code управляется через CLAUDE.md в корне проекта
3. Скиллы лежат в .claude/skills/ — подхватываются автоматически
4. Git инициализирован, первый коммит сделан
5. Шаблоны подключены через Templates + Templater

## Структура Vault
- Resources — исследования, конспекты, референсы
- Tasks — задачи и чеклисты
- Ideas — идеи, гипотезы, черновики
- Projects — активные проекты
- Daily — ежедневные заметки
- Templates — шаблоны заметок
- Archive — завершённое и неактуальное

## Скиллы Claude Code
- maxim-communication.md — стиль общения (неформальный, прагматичный)
- research-to-obsidian.md — ресерч с сохранением в vault

## Как применить на практике
- Ctrl+P и Insert template для новых заметок
- Wiki-ссылки [[Ideas]] [[Projects]] связывают всё в граф
- Git коммиты через Conventional Commits (feat:, fix:, docs:)

## Связанные заметки
- [[README]]
- [[First Vault Test]]