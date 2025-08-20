## 🎯 Introducción
El objetivo fue construir un modelo de Machine Learning para predecir la evasión de clientes. Se entrenaron dos modelos: Regresión Logística y Random Forest.

El modelo **Random Forest demostró un rendimiento superior**, destacando por su alto **Recall**. Esto significa que es significativamente más eficaz para su propósito principal: **identificar correctamente a la mayoría de los clientes que están en riesgo real de cancelar el servicio**.

---

## 💡 Principales Factores que Impulsan la Evasión (Churn)
Ambos modelos coincidieron en que la decisión de un cliente de cancelar el servicio está fuertemente influenciada por un pequeño grupo de factores clave. El perfil del cliente con mayor probabilidad de evasión es:

*   **1. Tipo de Contrato:** Tener un contrato **mes a mes (`Month-to-month`)** es, por un amplio margen, el predictor más fuerte de cancelación. La falta de un compromiso a largo plazo representa el mayor riesgo.

*   **2. Antigüedad del Cliente (`customer_tenure`):** Los **clientes nuevos son los más vulnerables**. El riesgo de cancelación es más alto durante los primeros meses y disminuye drásticamente a medida que el cliente permanece más tiempo con la empresa.

*   **3. Cargos Mensuales (`account_Charges_Monthly`):** Los clientes con **facturas mensuales más elevadas** son más propensos a cancelar, probablemente buscando ofertas más competitivas. Esto está estrechamente relacionado con tener servicios como `Fibra Óptica`.

---

## 🚀 Estrategias de Retención Recomendadas
Basado en los hallazgos del modelo, se proponen las siguientes estrategias de retención dirigidas:

1.  **Fidelizar a Clientes con Contratos Flexibles:**
    *   **Acción:** Crear campañas proactivas para ofrecer a los clientes de `Month-to-month` descuentos o beneficios exclusivos si migran a un contrato de 1 o 2 años.

2.  **Fortalecer la Relación con Clientes Nuevos:**
    *   **Acción:** Implementar un programa de "bienvenida" o "onboarding" durante los primeros 3 meses, ofreciendo soporte prioritario, tutoriales o un pequeño beneficio para fortalecer la lealtad inicial.

3.  **Añadir Valor a los Planes de Alto Costo:**
    *   **Acción:** Para los clientes con facturas altas (especialmente de `Fibra Óptica`), crear paquetes de valor añadido (bundles) que incluyan servicios como soporte técnico avanzado o seguridad online para justificar el costo y reducir la tentación de cambiar de proveedor.
