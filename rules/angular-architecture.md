---
trigger: always_on
description: When you write new angular code
---

# Base rule
- Use standalone components
- State shering only by ngrx
- Business logic store in Services not in components
- Prefer signal instead of subscription

# Naming convention
- *.component.ts/html/css - Angular component
- *.service.ts - common services
- *.facade.ts - sercice with business logic
