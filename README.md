# 🚗 Motor de Decisão TCO: Flex vs. Híbrido/Elétrico
### Inteligência de Mercado para Frotas Corporativas (São Paulo, 2026)

## 📌 O Problema de Negócio
Gestores de frota enfrentam um dilema financeiro recorrente: renovar com veículos Flex (menor custo de aquisição, tecnologia madura) ou migrar para Híbrido/Elétrico (menor custo operacional, maior investimento inicial e depreciação incerta)? 

A maioria das comparações de mercado limita-se ao custo de combustível (CPK). Este projeto propõe uma análise mais robusta baseada no **TCO (Total Cost of Ownership)**, integrando depreciação real, regras fiscais (IPVA-SP) e projeções de custo acumulado para oferecer uma visão clara do ponto de equilíbrio.

## 🛠 Stack Técnica
- **Linguagem:** Python (Pandas) para ETL e modelagem de custos.
- **Visualização:** Power BI (Dashboard em desenvolvimento - entrega prevista para 07/07/2026).
- **Fontes de Dados:** ANP (combustíveis), FIPE (valor de mercado), SEFAZ-SP (regras tributárias).

## ⚖️ Premissas e Limitações
*Análise baseada em dados reais de 2026.*
- **Escopo:** Análise restrita ao estado de São Paulo.
- **CAPEX:** Não inclui custo de instalação de infraestrutura de recarga.
- **Manutenção:** Utiliza benchmarks de mercado por categoria de veículo.
- **Depreciação:** Projetada via histórico FIPE; o mercado de usados para elétricos no Brasil ainda é volátil.

## 🏗 Arquitetura do Modelo (Star Schema)
O projeto foi estruturado em um *Star Schema* para garantir escalabilidade e fácil integração com ferramentas de BI:
- **Dimensões:** `dim_veiculo` (cadastro e especificações).
- **Fatos:** `fato_consumo` (eficiência) e `fato_simulacao` (cálculos de TCO acumulado).

## 📊 Dashboard Interativo
*Em desenvolvimento. A versão final será publicada na conclusão da série de análise.*

## 📈 Matriz de KPIs
- **TCO Unitário:** Custo total acumulado por tecnologia (Flex vs. Híbrido vs. Elétrico).
- **Break-even Point:** Quilometragem mensal necessária para compensar o investimento inicial.
- **Taxa de Depreciação Relativa:** Percentual de desvalorização comparado entre as categorias ao longo de 36 meses.

---
*Projeto desenvolvido como parte do portfólio de Inteligência de Mercado.*
