# AI App Builder — Product Vision & Delivery Roadmap

## ב-10 שניות: מה עושים עכשיו?
אנחנו **לא מתחילים מהתחלה**.
אנחנו ממשיכים ישר ל-**שלב 2**: בניית מסך Builder אמיתי עם Drag & Drop.

### המשימה המיידית (Sprint נוכחי)
1. ליצור `CanvasRenderer` (אזור בנייה חי).
2. ליצור `ElementSidebar` (רשימת אלמנטים לגרירה).
3. להוסיף `PropertiesPanel` (עריכת טקסט/צבע/מרווחים/תמונה).
4. לשמור הכול בתוך `appSchema.screens[*].blocks`.
5. לוודא ש-Preview/LiveApp מציגים את אותם blocks בצורה זהה.

אם 5 הסעיפים האלה עובדים — סגרנו את הליבה של שלב 2.

---

## Vision (Final Target)
We are building a **commercial AI-native App Builder platform** (not a single app), designed to let users describe a product idea in natural language and get:
- structured product blueprint,
- editable UI builder output,
- generated backend/data model,
- deployment-ready application.

The long-term product direction is to compete on UX + intelligence against modern no-code / low-code builders.

## Current Alignment
This repository captures the agreed direction:
1. We are **not** building a hobby demo.
2. The current phase focuses on strong foundations (stability, schema, preview, editing loop).
3. The roadmap intentionally moves from core reliability to advanced UI editor and commercialization.

## Phase Plan

### Phase 1 — Foundation Stability (near completion)
- project load/edit lifecycle,
- basic screen/schema management,
- base preview/public rendering,
- core persistence.

### Phase 2 — Drag & Drop UI Builder (active now)
- live canvas,
- element sidebar,
- properties panel,
- schema-backed UI blocks,
- image element support (manual upload mode + auto-image flag).

### Phase 3 — AI-native Builder Intelligence
- blueprint-aware generation,
- conversational edits,
- auto layout,
- context-aware image suggestions,
- code generation expansion.

### Phase 4 — Backend Automation
- collection/model generation,
- CRUD route generation,
- auth/roles,
- image storage integration (S3/Cloudinary-like flow).

### Phase 5 — Commercial SaaS Layer
- billing/subscriptions,
- tenant/project management,
- client dashboard.

### Phase 6 — Marketplace Ecosystem
- templates,
- components/plugins,
- vertical AI packs.

## Definition of "Professional"
To keep execution practical while targeting enterprise-grade quality, every phase should satisfy:
- clear acceptance criteria,
- measurable reliability,
- incremental user value,
- backward compatibility of core schemas,
- migration path for existing projects.

## Next Execution Focus (Concrete)
Immediate next focus remains **Phase 2 implementation** with production-oriented architecture choices:
1. canonical screen block schema,
2. robust DnD interactions,
3. deterministic rendering,
4. image block contract (source/manual/auto metadata),
5. clean extension points for upcoming AI operations.

### Definition of Done for this phase checkpoint
- אפשר לגרור לפחות: `Text`, `Input`, `Button`, `Image`, `Container`.
- אפשר לערוך מאפיינים בסיסיים לכל אלמנט.
- שינוי ב-Builder נשמר ומופיע ב-Live Preview לאחר רענון.
- אין שבירה של פרויקטים ישנים (fallback תקין אם אין `blocks`).

---

If this document exists in the repo, it should be treated as the current product alignment baseline until replaced by a newer version.
