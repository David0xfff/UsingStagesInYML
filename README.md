
Este archivo azure-pipelines.yml describe el funcionamiento del pipeline definido en YAML para la integración y entrega continua (CI/CD) de un proyecto. El pipeline se ejecuta automáticamente cuando hay cambios en la rama `main`.

---

## 📁 Estructura General

El pipeline se organiza en **3 stages** principales:

1. **Compilación (Build)**
2. **Pruebas (Test)**
3. **Despliegue (Deploy)**

Cada stage contiene uno o más jobs con tareas específicas.

---

## 🚀 Disparador (Trigger)

```yaml
trigger:
  branches:
    include:
      - main
