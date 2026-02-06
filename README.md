# flujograma
flowchart TD
  A[Inicio: Decisión de formalizar TechFix Express] --> B{"Definir forma jurídica"}
  
  B -->|Persona Natural| C["Registrar actividad económica"]
  B -->|SAS / Cía. Ltda.| D["Definir socios, capital y administrador"]
  
  D --> E["Reserva/validación de nombre comercial"]
  E --> F["Redacción de estatutos\n(servicios técnicos informáticos a domicilio)"]
  F --> G["Firma del acto constitutivo en notaría"]
  G --> H["Inscripción en Registro Mercantil/Superintendencia"]
  
  C --> I["Obtención de RUC en SRI"]
  H --> I
  
  I --> J["Definir régimen tributario y\nsistema de facturación electrónica"]
  J --> K["Permisos municipales:\npatente y LUAE (según GAD)"]
  K --> L["Apertura de cuenta bancaria\npara el negocio"]
  
  L --> M{"¿Contratar personal?"}
  M -->|Sí| N["Registro en IESS\nContratos laborales\nSeguridad ocupacional"]
  M -->|No| O["Operación con equipo inicial\n(socios fundadores)"]
  
  N --> P["Inicio de operaciones formales:\nEmisión de comprobantes\nRegistro de clientes"]
  O --> P
  
  P --> Q[Fin del proceso de constitución]

  classDef decision fill:#f9f,stroke:#333,stroke-width:2px
  classDef process fill:#bbf,stroke:#333,stroke-width:1px
  classDef start fill:#9f6,stroke:#333,stroke-width:2px
  classDef final fill:#f96,stroke:#333,stroke-width:2px
  
  class A start
  class B,M decision
  class C,D,E,F,G,H,I,J,K,L,N,O,P process
  class Q final
