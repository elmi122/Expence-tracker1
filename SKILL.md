---
name: google-gallery-edge-expense-tracker
description: >
  Build a visually stunning, production-grade Expense Tracker application with a Google Gallery Edge aesthetic — clean card-based layouts, bold typography, smooth transitions, and a modern financial dashboard feel. Use this skill whenever the user asks for an expense tracker, spending dashboard, budget manager, finance tracker, or any personal finance UI. Trigger this skill even when the user says things like "track my money", "show me my spending", "create a budget app", or "expense app with gallery feel". Always use this skill for any expense, budget, or finance tracking interface — especially if they mention cards, gallery, visual layout, or Google-inspired design.
---

# Google Gallery Edge Expense Tracker Skill

Build a polished, interactive expense tracker app with a **Google Gallery Edge** aesthetic: card-based layout, bold accent colors, smooth animations, generous whitespace, and a dashboard-style financial overview.

## Design Direction

**Aesthetic**: Google Gallery Edge — material-inspired cards, crisp typography, bold category colors, subtle elevation shadows, smooth slide/fade transitions.

**Color Palette**:
- Background: #0f0f11
- Surface: #1a1a1f
- Card: #22222a
- Accent: #6c63ff
- Green: #22c55e
- Red: #ef4444
- Text: #f0f0f5

**Typography**: DM Sans (display) + JetBrains Mono (numbers) from Google Fonts.

## Core Features

1. **Dashboard Header** - Total balance, income vs expense summary, month navigation
2. **Quick Add Form** - Amount input, category picker, description, date, income/expense toggle
3. **Expense Cards Gallery** - Grid layout, category icons, filter by category, delete on hover
4. **Analytics Panel** - SVG donut chart, category progress bars
5. **FAB Button** - Floating + button bottom-right for quick add

## Categories
- Food: 🍔 #f97316
- Transport: 🚗 #3b82f6
- Housing: 🏠 #8b5cf6
- Health: 💊 #22c55e
- Entertainment: 🎮 #ec4899
- Shopping: 🛍️ #f59e0b
- Work: 💼 #6366f1
- Travel: ✈️ #06b6d4
- Other: 📦 #94a3b8

## Sample Seed Data
Always pre-load with these entries:
- Income: 3200 - Monthly salary - Work - 2025-04-01
- Expense: 850 - Rent payment - Housing - 2025-04-01
- Expense: 42 - Grocery run - Food - 2025-04-03
- Expense: 15 - Uber to airport - Transport - 2025-04-05
- Expense: 120 - Concert tickets - Entertainment - 2025-04-08
- Expense: 67 - New sneakers - Shopping - 2025-04-10
- Expense: 28 - Pharmacy - Health - 2025-04-12
- Income: 450 - Freelance project - Work - 2025-04-15

## Implementation Notes
- Single React .jsx artifact
- All state in useState (no localStorage)
- SVG donut chart, no external chart libraries
- Card hover: translateY(-4px) + shadow
- New cards slide in from bottom
- Deleted cards fade out before removal
