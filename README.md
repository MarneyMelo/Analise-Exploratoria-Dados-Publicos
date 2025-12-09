
# Análise de Segurança Alimentar e População em Situação de Rua - BH

Este projeto foi desenvolvido como trabalho final da disciplina de **Introdução a Banco de Dados (2025/2)** da UFMG.

O objetivo foi integrar e analisar dados públicos sobre a população em situação de rua de Belo Horizonte e a disponibilidade de equipamentos de segurança alimentar (restaurantes comunitários), identificando lacunas na assistência social e padrões demográficos.

## 👥 Autores

- Marney Melo  
- Rafael Miranda  
- Theo Duarte  
- Victor Kaizer  
- Vinícius Rocha  

## Objetivos e Escopo

O sistema relaciona dados de moradores de rua (Cadastro Único), CRAS (Centro de Referência de Assistência Social) e restaurantes comunitários. O foco foi responder a perguntas como:

- Qual a disponibilidade de restaurantes para a população de rua em cada região administrativa?  
- Qual o perfil de permanência nas ruas (tempo x idade)?  
- Existe correlação entre raça, escolaridade e tempo de rua?  
- Qual a viabilidade de políticas de retorno à cidade de origem baseada em vínculos familiares?  

## Metodologia e Tecnologias

- **Banco de Dados:** PostgreSQL  
- **Modelagem:** Modelo Entidade-Relacionamento (ER) e Relacional normalizado  
- **Integração Espacial:** Utilização de Spatial Join para associar a posição geográfica dos restaurantes aos polígonos das Regiões Administrativas de BH  
- **ETL:** Limpeza de dados (sanitização), tratamento de chaves primárias compostas para CRAS com nomes duplicados e importação via tabelas temporárias  

## 📊 Principais Resultados da Análise

1. **Déficit Periférico:** Regiões como **Noroeste** e **Leste** apresentam maior sobrecarga (mais moradores de rua por restaurante), indicando urgência de políticas públicas nessas áreas.  
2. **Vínculos Familiares:** Cerca de **66%** dos moradores possuem vínculos familiares rompidos ou frágeis, tornando políticas de retorno à cidade natal pouco eficazes sem suporte prévio.  
3. **Perfil Etário e Racial:**
   - Jovens tendem a ter entrada recente na situação de rua (menos de 6 meses), enquanto idosos apresentam quadros crônicos.  
   - A população negra/parda em situação de rua apresenta índices de escolaridade significativamente menores que a população branca, evidenciando barreiras estruturais.  

## Estrutura do Repositório
```text
/
├── database/
│   └── backup.sql       # Dump completo do banco de dados (PostgreSQL)
├── docs/
│   ├── Relatorio_pt1.pdf
│   ├── Relatorio_pt2.pdf
│   └── Apresentacao_Final.pdf
└── README.md
```