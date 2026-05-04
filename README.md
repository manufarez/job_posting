# Take-home assignment: job posting feature

## Contexto
Construye un mini-feature desde cero. Empieza con `rails new`.

## Stack obligatorio
- Rails 8, Ruby 3.3+
- PostgreSQL
- Tailwind CSS
- Hotwire (Turbo + Stimulus) — sin React
- Devise o auth nativa de Rails 8 — tu elección, justifícala en el Loom

## Funcionalidad
Una empresa autenticada (Employer) debe poder:
1. Crear un Job con: título, descripción rich-text (ActionText), salario min/max, ubicación, tipo de contrato (enum: full-time / contract / part-time), skills (array, JSONB o tabla, tu elección), fecha de cierre.
2. Subir un logo (Active Storage, local, sin S3).
3. Ver la lista de sus propios jobs (activos y cerrados).
4. Editar y desactivar (soft delete) un job.
5. Vista pública sin auth en `/jobs/:slug` (usa friendly_id o equivalente — no IDs en URL).

## Requisitos técnicos
- Validaciones server-side con feedback inline claro en el form
- UX cuidada: errores inline, preview antes de publicar, confirmación de acciones destructivas
- 2–3 model specs cubriendo validaciones y estados
- Seeds para 1 Employer y 3 Jobs de ejemplo
- README con setup en menos de 5 minutos

## Qué evaluamos
- Diseño del modelo: validaciones, índices, asociaciones
- Código idiomático Rails, sin sobre-ingeniería
- UX del formulario
- Tests donde realmente importan
- Setup limpio: migraciones, seeds, README

## Entrega
- PR a `main`
- Loom de máximo 5 minutos: app funcionando + 2–3 decisiones técnicas que tomaste + qué dejaste fuera y por qué
- Plazo: 48 horas desde el final de la entrevista
