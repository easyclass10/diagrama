graph TD
    A[Inicio: Definir Unidad Homogénea] --> B{Recopilación de Datos};
    B --> C[Ensayo de Laboratorio: Modulo Resiliente AASHTO T307];
    B --> D[Correlaciones con otros Ensayos CBR, R-Value, etc.];
    C --> E[Obtener valores de Modulo Resiliente M_R de especímenes de la unidad];
    D --> F[Estimar valores de M_R a partir de correlaciones];
    E --> G{Análisis Estadístico};
    F --> G;
    G --> H[Calcular la media μ y la desviación estándar σ de los valores de M_R];
    H --> I{Seleccionar Nivel de Confiabilidad R};
    I --> J[Determinar el valor de la normal estándar Z_R asociado a la Confiabilidad];
    J --> K[Calcular el Modulo Resiliente de Diseño M_R.diseño];
    K --> L[Fin: Usar M_R.diseño en el diseño de la estructura del pavimento];

    subgraph "Fórmula de Cálculo"
        direction LR
        K --> M[M_R.diseño = μ - Z_R · σ];
    end

    style A fill:#D6EAF8,stroke:#333,stroke-width:2px
    style L fill:#D5F5E3,stroke:#333,stroke-width:2px
    style K fill:#FADBD8,stroke:#333,stroke-width:2px
