# SyncUT - Árbol de Carpetas para Junta

## Vista simple

```text
SyncUT/
├── apps/web/app/
│   ├── (auth)            Squad 2 - Autenticación y auditoría
│   ├── (citas)           Squad 3 - Citas
│   ├── (justificaciones) Squad 1 - Justificaciones
│   ├── (notificaciones)  Squad 4 - Notificaciones
│   └── (dashboard)       Staff - Dashboard compartido
├── packages/             Código compartido
├── supabase/             Base de datos y tests
├── docs/                 Documentación por módulo
└── scripts/              Automatización y utilidades
```

## Vista detallada

```text
SyncUT/
├── apps/
│   └── web/
│       ├── app/
│       │   ├── (auth)/
│       │   │   ├── login/page.tsx
│       │   │   ├── signup/page.tsx
│       │   │   └── profile/page.tsx
│       │   ├── (citas)/
│       │   │   ├── page.tsx
│       │   │   ├── components/
│       │   │   ├── hooks/
│       │   │   └── types/
│       │   ├── (justificaciones)/
│       │   │   ├── page.tsx
│       │   │   ├── components/
│       │   │   ├── hooks/
│       │   │   ├── services/
│       │   │   └── types/
│       │   ├── (notificaciones)/
│       │   │   ├── page.tsx
│       │   │   ├── components/
│       │   │   ├── hooks/
│       │   │   ├── services/
│       │   │   └── types/
│       │   └── (dashboard)/
│       │       ├── page.tsx
│       │       ├── components/
│       │       ├── hooks/
│       │       └── types/
│       ├── components/
│       │   ├── ui/
│       │   └── modules/
│       ├── lib/
│       └── public/
├── packages/
│   ├── config/
│   ├── sdk/
│   │   └── src/
│   ├── shared/
│   │   └── src/
│   ├── types/
│   │   └── src/
│   └── ui/
├── supabase/
│   ├── migrations/
│   └── tests/
├── docs/
│   ├── GOOGLE_STITCH_PROMPT.md
│   ├── GOOGLE_STITCH_PROMPT_CORE.md
│   ├── GOOGLE_STITCH_PROMPT_MODULE_1_JUSTIFICATIONS.md
│   ├── GOOGLE_STITCH_PROMPT_MODULE_2_AUTHENTICATION_AUDIT.md
│   ├── GOOGLE_STITCH_PROMPT_MODULE_3_APPOINTMENTS.md
│   ├── GOOGLE_STITCH_PROMPT_MODULE_4_NOTIFICATIONS.md
│   ├── GOOGLE_STITCH_PROMPT_MODULE_5_STAFF_DASHBOARD.md
│   ├── squad-1-justificaciones/
│   ├── squad-2-auditoría/
│   ├── squad-3-citas/
│   ├── squad-4-notificaciones/
│   └── staff-dashboard/
└── scripts/
```

## Dónde trabaja cada squad

### Squad 2 - Autenticación y auditoría

Trabaja en:
- [apps/web/app/(auth)](apps/web/app/%28auth%29)
- [apps/web/middleware.ts](apps/web/middleware.ts)
- [supabase/migrations](supabase/migrations)
- [packages/sdk](packages/sdk)
- [packages/types](packages/types)

### Squad 3 - Citas

Trabaja en:
- [apps/web/app/(citas)](apps/web/app/%28citas%29)
- [apps/web/components/modules](apps/web/components/modules)

### Squad 4 - Notificaciones

Trabaja en:
- [apps/web/app/(notificaciones)](apps/web/app/%28notificaciones%29)
- [packages/shared](packages/shared)
- [supabase/migrations](supabase/migrations)

### Squad 1 - Justificaciones

Trabaja en:
- [apps/web/app/(justificaciones)](apps/web/app/%28justificaciones%29)
- [supabase/migrations](supabase/migrations)
- [supabase/tests](supabase/tests)

### Staff - Dashboard compartido

Trabaja en:
- [apps/web/app/(dashboard)](apps/web/app/%28dashboard%29)
- [apps/web/components/modules](apps/web/components/modules)

## Regla de uso para la junta

1. Mostrar primero la vista simple.
2. Después mostrar la vista detallada solo si piden más profundidad.
3. Usar los docs de Stitch por módulo como soporte visual.
4. No mezclar rutas antiguas con las rutas reales del repositorio.