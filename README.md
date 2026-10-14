# Organigrama — Emprendimiento familiar (alimentos aptos para celíacos)

Emprendimiento familiar de 5 personas. Misión: abastecer a personas celíacas con productos seguros y de calidad. Controles: no ingreso de TACC, auditorías ASAL y manual de buenas prácticas.

```mermaid
flowchart TD
  owner["Dueña / Responsable\nSupervisión general"]
  mama["Mamá / Co-responsable\nControl de calidad"]
  prod["Producción"]
  cocina["Cocina\nRellenos y purés"]
  maquinas["Máquinas y Hornos\nAmasado y cocción"]
  envasado["Envasado\nEtiquetado y empaques"]

  owner --> prod
  mama --> prod

  prod --> cocina
  prod --> maquinas
  prod --> envasado

  subgraph info [Información clave]
    mision["Misión: Abastecer a celíacos con productos seguros y de calidad"]
    controles["Controles: No ingreso TACC · 2 auditorías ASAL/año · Manual de buenas prácticas"]
    pedidos["Pedidos: Semanal (dom) · Diarios tardes (pan/pizza)"]
    productos["Productos (ej.): Pan · Pizza · Ravioles · Alfajores · Budines · Pan dulce (estacional)"]
  end

  owner -.-> controles
  mama -.-> controles
  envasado -.-> pedidos
  cocina -.-> productos

Agregar organigrama en Mermaid al README
Formato PNG