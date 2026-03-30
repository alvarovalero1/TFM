# 🛡️ VulnPrioritizer: ¿Tu equipo de seguridad está agotado? 
> **Dejar de parchear por miedo para empezar a parchear por riesgo.**

![Cybersecurity](https://img.shields.io/badge/Sector-Cybersecurity-red)
![Automation](https://img.shields.io/badge/Tech-n8n%20%7C%20Python-orange)
![Framework](https://img.shields.io/badge/Framework-IPC%20Methodology-blue)

Si trabajas en ciberseguridad, conoces esta sensación: lunes por la mañana, abres el escáner de vulnerabilidades y te encuentras con un informe de 500 páginas. Según el estándar CVSS, casi todo es "Crítico" o "Alto". Tienes cientos de parches pendientes, pero solo tienes manos para un par de servidores al día.

**¿Por dónde empiezas?** ¿Por el servidor que tiene un 9.8 pero está en una red aislada? ¿O por ese 7.5 que está en la base de datos de pacientes y tiene un exploit público en GitHub?

Este es el problema que resuelve **VulnPrioritizer**.

---

## 🛑 El Problema: La "Fatiga de Alertas"
Hoy en día, las empresas sufren de saturación. El CVSS (el sistema estándar de gravedad) es útil, pero tiene un defecto: **no conoce tu negocio**. Para el CVSS, una vulnerabilidad en una cafetera inteligente tiene la misma nota que en el servidor principal de un hospital si el fallo técnico es idéntico.

En el mundo real, eso no tiene sentido. Por eso hemos creado una metodología que añade **contexto**.

## 🧠 La Solución: No parches más, parchea mejor
Para el caso de estudio de **MediTech Solutions** (una clínica sanitaria), desarrollamos un cerebro automatizado usando **n8n**, orquestando la seguridad de forma inteligente.

La magia reside en el **IPC (Índice de Priorización Contextual)**. En lugar de mirar solo la nota del fabricante, VulnPrioritizer aplica un algoritmo de 7 factores:

1. **Valor del Activo:** ¿Es crítico para la salud de los pacientes?
2. **Exposición:** ¿Está en la DMZ o en una red interna?
3. **Amenaza:** ¿Hay actividad real de atacantes?
4. **Armamentización (Weaponization):** ¿Existe un exploit ya fabricado?
5. **Cumplimiento:** ¿Nos enfrentamos a multas de GDPR?
6. **Estado:** ¿Lleva mucho tiempo sin resolverse?

---

## 📊 Resultados: De 100 "incendios" a 41 fuegos reales
Probamos el sistema con un dataset de **100 vulnerabilidades reales** (incluyendo fallos críticos como Log4Shell o Zerologon).

| Métrica | Sin VulnPrioritizer (CVSS Puro) | Con VulnPrioritizer (Filtro IPC) |
| :--- | :---: | :---: |
| **Alertas Críticas** | 100 | **41** |
| **Carga Operativa** | 100% | **41%** |
| **Reducción de Ruido** | 0% | **59%** |

> **Conclusión:** El equipo de seguridad redujo su carga de trabajo inmediata en más de la mitad, enfocándose solo en lo que realmente podía tumbar la clínica.

---

## 💰 Hablando en Euros, no solo en Bits
Uno de los mayores retos es explicar a la dirección por qué es necesario invertir en seguridad. **VulnPrioritizer traduce el riesgo a lenguaje de negocio.**

Calculamos automáticamente el **SLE (Single Loss Expectancy)**. En MediTech, pudimos demostrar que las vulnerabilidades críticas abiertas representaban un riesgo financiero de **1,77 millones de euros**. 

> *"Cuando le dices a un directivo que un parche de 10 minutos protege 1,7 millones de euros, la conversación sobre ciberseguridad cambia por completo."*

---

## 🚀 El Futuro
Este prototipo es el primer paso hacia una gestión de vulnerabilidades totalmente autónoma. Próximas líneas de trabajo:
* 🤖 **Integración de IA Generativa:** Para redactar resúmenes ejecutivos automáticos.
* 🔗 **Conectores Directos:** Integración con APIs de Tenable, Qualys y sistemas de ticketing como Jira.
* 📈 **Ajuste Dinámico:** Recalibración de pesos basada en el histórico de incidentes.

---
**Desarrollado como Trabajo Fin de Máster (TFM)** *Autor: Álvaro Valero Praena* *Tecnología: n8n, Python, GitHub API, Gmail API.*
