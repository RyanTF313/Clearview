# Clearview
Teams need a flexible way to visualize metrics without engineering help. InsightBoard allows users to build customizable dashboards using reusable widgets, saved layouts, and shared views—optimized for performance at scale.

## MVP
### Dashboard

- Create / edit / delete dashboards
- Multiple dashboards per user
- Dashboard permissions (owner / viewer)

### Widgets

- Chart widget (line, bar)
- Table widget
- KPI metric widget
- Widgets are configurable (title, data source, refresh interval)

### Layout

- Drag & drop widgets
- Responsive layouts (desktop / tablet / mobile)
- Persist layout per dashboard

### Data

- Mock API first (replaceable later)
- Support large datasets (1k–10k rows)

## Tech Stack

- React + TypeScript
- Vite
- Tailwind CSS
- Redux Toolkit
- RTK Query
- dnd-kit (drag/drop)?
- Chart.js
- React Router
- Storybook

## Folder Structure
```
src/
 ├── app/            # App setup, providers
 ├── features/       # Feature-based slices
 │   ├── dashboards/
 │   ├── widgets/
 │   └── auth/
 ├── components/     # Shared UI components
 ├── hooks/          # Reusable hooks
 ├── services/       # API layer
 ├── stores/store
 |   ├── index.ts
 |   ├── dashboardsSlice.ts
 |   ├── widgetsSlice.ts
 |   ├── layoutSlice.ts
 |   └── api/
 |       └── dashboardApi.ts# Redux stores
 ├── utils/
 └── types/
```

