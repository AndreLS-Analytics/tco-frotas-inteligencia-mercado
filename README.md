# 🚗 Motor de Decisão TCO: Flex vs. Híbrido/Elétrico

**Inteligência de Mercado para Frotas Corporativas (São Paulo, 2026)**

---

## 📌 O Problema de Negócio
Gestores de frota enfrentam um dilema financeiro recorrente: renovar com veículos **Flex** (menor custo de aquisição, tecnologia madura) ou migrar para **Híbrido/Elétrico** (menor custo operacional, mas com maior investimento inicial e depreciação incerta)?

A maioria das comparações limita-se ao custo por quilômetro (CPK) de combustível. Este projeto entrega uma análise robusta baseada no **TCO (Total Cost of Ownership)**, integrando depreciação real, regras fiscais (IPVA-SP) e projeções de custo acumulado para identificar o ponto de equilíbrio (*break-even point*) real da eletrificação.

---

## 🛠 Stack Técnica
* **Linguagem:** Python (Pandas) para ETL e modelagem de custos.
* **Visualização:** Power BI (Dashboard em desenvolvimento).
* **Fontes de Dados:** ANP (combustíveis), FIPE (valor de mercado), SEFAZ-SP (tributação).

---

## 🏗 Arquitetura do Modelo (Star Schema)
O projeto utiliza uma modelagem em **Star Schema** para garantir escalabilidade e facilitar a integração com ferramentas de BI:

* **Dimensões:** `dim_veiculo` (cadastro e especificações técnicas).
* **Fatos:** `fato_consumo` (eficiência energética) e `fato_simulacao` (cálculos de TCO acumulado).

*Os arquivos processados e as imagens da modelagem estão disponíveis na pasta `/ativos`.*

---

## ⚖️ Premissas e Limitações
* Análise baseada em dados de mercado de 2026.
* Escopo restrito ao estado de São Paulo.
* CAPEX não inclui instalação de infraestrutura de recarga.
* Manutenção utiliza benchmarks de mercado por categoria.

---

## 📊 Matriz de KPIs
* **TCO Unitário:** Custo total acumulado por tecnologia.
* **Ponto de Equilíbrio:** Quilometragem mensal necessária para compensar o investimento inicial.
* **Taxa de Depreciação Relativa:** Desvalorização comparada entre as categorias ao longo de 36 meses.

---

## ✅ Status do Projeto
* ✅ **Modelagem de Dados (Python/Pandas):** Concluída.
* ✅ **Estrutura de Arquivos (Star Schema):** Organizada na pasta `/ativos`.
* ⏳ **Dashboard (Power BI):** Em desenvolvimento.

---
*Projeto desenvolvido como parte do portfólio de Inteligência de Mercado.*
