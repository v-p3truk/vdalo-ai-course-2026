# Доступ до AI-агентів — гайд

Швидкий огляд 4 інструментів. Який обрати — в кінці.

---

## TL;DR

| Tool | Free? | Підписка | Trial |
|------|-------|----------|-------|
| **Codex CLI** (OpenAI) | ❌ | ChatGPT Plus $20/міс або Team/Enterprise | Іноді 7-14 днів для нових юзерів |
| **Claude Code** (Anthropic) | ❌ | Claude Pro $20/міс або pay-per-use API | Без офіційного trial |
| **Antigravity** (Google) | ✅ | Безкоштовно з Gemini 2.5 | n/a |
| **Cursor** | ✅ Free tier | Pro $20/міс | 14-day Pro trial |

---

## Codex CLI

```bash
# macOS
brew install openai/codex/codex

# Універсально (npm)
npm install -g @openai/codex

# Залогін
codex login
```

**Підписка:** ChatGPT Plus ($20/міс), Team або Enterprise. Free акаунт не дає доступу до Codex CLI.
**Trial:** OpenAI періодично пропонує 7-14 днів для нових юзерів. У різних країнах непередбачувано.
**Файл контексту:** `AGENTS.md`

---

## Claude Code

```bash
# macOS / Linux
npm install -g @anthropic-ai/claude-code

# Залогін
claude login
```

**Підписка:** Claude Pro $20/міс (з лімітами на день), Max $100-200/міс (без лімітів), або через API ключ pay-per-use ($5-30/міс залежно від використання).
**Trial:** офіційного нема, але є **invite-based trials** — періодично доступні через спільноту.
**Файл контексту:** `CLAUDE.md`

---

## Antigravity

1. Скачати: https://antigravity.google.com (або через Google AI Studio)
2. Залогінитись через Google акаунт
3. Відкрити папку проєкту в IDE
4. Створити `GEMINI.md` як файл контексту

**Free tier:** Gemini 2.5 Flash і Pro з rate limits (для 1-2 годин роботи на день вистачає)
**Файл контексту:** `GEMINI.md`

---

## Cursor

1. Скачати: https://cursor.com
2. Залогін через Google або email
3. Pro trial — 14 днів автоматично

**Free tier:** обмежений (slower models, обмежена кількість запитів)
**Pro:** $20/міс
**Файл контексту:** `.cursorrules`

---

## Що обрати

| Сценарій | Рекомендація |
|----------|--------------|
| Команда має корпоративну ChatGPT Team/Enterprise | Codex CLI під корпоративним логіном |
| Хочу однакову екосистему за свої гроші | Codex Plus ($20) або Claude Pro ($20) |
| Хочу спочатку безкоштовно | Antigravity (free) або Cursor (14-day trial) |
| Гнучко (mix) | OK — техніки переносяться. `AGENTS.md` / `CLAUDE.md` / `GEMINI.md` / `.cursorrules` мають однаковий зміст |

**Принцип:** інструмент — другорядне. Контекст (`AGENTS.md`) — наскрізне. Якщо контекст хороший — будь-який з 4 буде працювати на 80%.

---

## Питання які варто уточнити в адміна workspace

- [ ] Чи є корпоративна ChatGPT Team / Enterprise підписка?
- [ ] Якщо так — як команда логіниться (через Workspace?)
- [ ] Якщо ні — чи готові оплатити $20/міс ChatGPT Plus?
- [ ] Чи можна списувати на корпоративний рахунок особисті Plus-підписки (для початку)?

---

## Якщо щось не працює

1. Спершу — спитай в команді з конкретною помилкою (скрін чи текст)
2. Якщо питання логіну/підписки — звертайся до адміна workspace
3. Якщо питання роботи з агентом — звертайся до інструктора курсу

---

*Last updated: 2026-05-07*
