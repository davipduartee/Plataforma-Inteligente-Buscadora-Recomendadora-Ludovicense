# Graph Report - plataforma-inteligente-buscadora-recomendadora-ludovicense  (2026-10-21)

## Corpus Check
- Corpus is ~45,795 words - fits in a single context window. You may not need a graph.

## Summary
- 104 nodes · 250 edges · 8 communities
- Extraction: 63% EXTRACTED · 36% INFERRED · 1% AMBIGUOUS · INFERRED: 90 edges (avg confidence: 0.82)
- Token cost: 635,714 input · 0 output

## Community Hubs (Navigation)
- Ranking de Fornecedores
- Projeto e Fluxo de Busca
- Home e Passo 1 (Produto)
- Prazo e Critérios
- Veredito e Score da IA
- Análise da IA
- Como Funciona e Confiabilidade
- Orçamento (Passo 3)

## God Nodes (most connected - your core abstractions)
1. `Fornecedores locais (lojas de Sao Luis)` - 22 edges
2. `Top 10 Supplier Ranking Table` - 17 edges
3. `Score de custo-beneficio` - 16 edges
4. `Busca Inteligente SLZ` - 15 edges
5. `IA de analise e auditoria de fornecedores` - 15 edges
6. `Tela 02 - Busca passo 1: produto` - 15 edges
7. `Criterio: preco` - 13 edges
8. `Fornecedores online (sites)` - 13 edges
9. `Fluxo de busca inteligente (telas)` - 13 edges
10. `Tela 01 - Tela inicial (Home)` - 13 edges

## Surprising Connections (you probably didn't know these)
- `Passo 01 - Diga o que quer (produto, prazo e orcamento)` --semantically_similar_to--> `Tela 02 - Busca passo 1: produto`  [INFERRED] [semantically similar]
  Assets/01-tela-inicial-home.png → README.md
- `Selo Menor Preço` --conceptually_related_to--> `Criterio: preco`  [INFERRED]
  Assets/06-resultados-recomendacao.png → README.md
- `Barra de Navegacao (Como Funciona, Fornecedores, Sobre, Entrar)` --conceptually_related_to--> `Fornecedores locais (lojas de Sao Luis)`  [INFERRED]
  Assets/01-tela-inicial-home.png → README.md
- `Barra de Navegação (Como Funciona, Fornecedores, Sobre, Entrar)` --references--> `Fornecedores locais (lojas de Sao Luis)`  [INFERRED]
  Assets/02-busca-passo1-produto.png → README.md
- `Opcao: Hoje mesmo (Retirada em loja fisica)` --conceptually_related_to--> `Fornecedores locais (lojas de Sao Luis)`  [INFERRED]
  Assets/03-busca-passo2-prazo.png → README.md

## Hyperedges (group relationships)
- **Criterios do score de custo-beneficio** — readme_score_custo_beneficio, readme_criterio_preco, readme_criterio_frete, readme_criterio_prazo, readme_criterio_confiabilidade [EXTRACTED 1.00]
- **Fluxo de navegacao das 7 telas da busca inteligente** — assets_01_tela_inicial_home_tela, assets_02_busca_passo1_produto_tela, assets_03_busca_passo2_prazo_tela, assets_04_busca_passo3_orcamento_tela, assets_05_ia_analisando_tela, assets_06_resultados_recomendacao_tela, assets_07_top_fornecedores_tela [EXTRACTED 1.00]
- **Pipeline de recomendacao: entrada do usuario -> auditoria IA -> veredito** — readme_entrada_usuario_produto_prazo_orcamento, readme_ia_auditoria_fornecedores, readme_fornecedores_locais, readme_fornecedores_online, readme_veredito_ia [EXTRACTED 1.00]
- **Fluxo de 3 passos: Diga o que quer -> IA analisa -> Compra ideal** — assets_01_tela_inicial_home_passo1_diga_o_que_quer, assets_01_tela_inicial_home_passo2_ia_analisa, assets_01_tela_inicial_home_passo3_compra_ideal, readme_fluxo_busca_inteligente [EXTRACTED 1.00]
- **Pontos de entrada da busca na home** — assets_01_tela_inicial_home_modos_busca, assets_01_tela_inicial_home_campo_busca, assets_01_tela_inicial_home_sugestoes_rapidas, assets_01_tela_inicial_home_explorar_categorias [INFERRED 0.85]
- **Wizard de Busca em 3 Passos** — assets_02_busca_passo1_produto_tela, assets_03_busca_passo2_prazo_tela, assets_02_busca_passo1_produto_wizard_stepper, readme_fluxo_busca_inteligente [INFERRED 0.85]
- **Captura da Consulta de Produto** — assets_02_busca_passo1_produto_modos_entrada, assets_02_busca_passo1_produto_campo_descricao, assets_02_busca_passo1_produto_buscas_populares, assets_02_busca_passo1_produto_cta_continuar [EXTRACTED 1.00]
- **Opcoes de prazo do passo 2** — assets_03_busca_passo2_prazo_opcao_hoje_mesmo, assets_03_busca_passo2_prazo_opcao_ate_3_dias, assets_03_busca_passo2_prazo_opcao_ate_1_semana, assets_03_busca_passo2_prazo_opcao_ate_2_semanas, assets_03_busca_passo2_prazo_opcao_sem_pressa [EXTRACTED 1.00]
- **Wizard de busca em 3 passos (produto, prazo, orcamento)** — assets_02_busca_passo1_produto_tela, assets_03_busca_passo2_prazo_tela, assets_04_busca_passo3_orcamento_tela, readme_fluxo_busca_inteligente [INFERRED 0.95]
- **Prazo pondera preco, frete e prazo no ranking** — assets_03_busca_passo2_prazo_tradeoff_prazo_preco, readme_criterio_prazo, readme_criterio_preco, readme_criterio_frete [INFERRED 0.75]
- **Wizard de Busca em 3 Passos até Análise IA** — assets_03_busca_passo2_prazo_tela, assets_04_busca_passo3_orcamento_tela, assets_05_ia_analisando_tela, readme_fluxo_busca_inteligente [INFERRED 0.85]
- **Captura de Orçamento (presets, personalizado, confirmação)** — assets_04_busca_passo3_orcamento_faixas_preco, assets_04_busca_passo3_orcamento_valores_personalizados, assets_04_busca_passo3_orcamento_confirmacao_orcamento, assets_04_busca_passo3_orcamento_botao_analisar_ia [EXTRACTED 1.00]
- **Pipeline sequencial de analise da IA (identificar -> benchmarking -> auditoria -> cruzamento orcamento/prazo)** — assets_05_ia_analisando_etapa_produto_identificado, assets_05_ia_analisando_etapa_benchmarking, assets_05_ia_analisando_etapa_auditoria_seguranca, assets_05_ia_analisando_etapa_cruzamento_orcamento_prazo [EXTRACTED 1.00]
- **Criterios avaliados durante a analise (preco, frete, prazo, confiabilidade)** — readme_criterio_preco, readme_criterio_frete, readme_criterio_prazo, readme_criterio_confiabilidade, assets_05_ia_analisando_checklist_etapas [INFERRED 0.75]
- **Fluxo de telas: orcamento -> IA analisando -> resultados** — assets_04_busca_passo3_orcamento_tela, assets_05_ia_analisando_tela, assets_06_resultados_recomendacao_tela, readme_fluxo_busca_inteligente [INFERRED 0.85]
- **Breakdown dos 4 critérios no fornecedor #1** — assets_06_resultados_recomendacao_barras_criterios, readme_criterio_preco, readme_criterio_frete, readme_criterio_prazo, readme_criterio_confiabilidade, fornecedor_techstore_sao_luis [EXTRACTED 1.00]
- **Ranking misto local vs online para Notebook Samsung** — assets_06_resultados_recomendacao_ranking_fornecedores, fornecedor_techstore_sao_luis, fornecedor_mercadodigital, fornecedor_loja_do_ze_eletronicos, fornecedor_americacom [EXTRACTED 1.00]
- **Decisão: restrições da busca, veredito da IA e score** — assets_06_resultados_recomendacao_resumo_busca, assets_06_resultados_recomendacao_card_veredito, assets_06_resultados_recomendacao_score_final, readme_veredito_ia [INFERRED 0.85]
- **Unified local vs online supplier leaderboard** — assets_07_top_fornecedores_ranking_table, assets_07_top_fornecedores_tipo_badge, readme_fornecedores_locais, readme_fornecedores_online, readme_score_custo_beneficio [INFERRED 0.85]
- **Supplier trust signals (verification, score, audit)** — assets_07_top_fornecedores_verified_badge, assets_07_top_fornecedores_score_coloring, readme_criterio_confiabilidade, readme_ia_auditoria_fornecedores [INFERRED 0.75]

## Communities (8 total, 0 thin omitted)

### Community 0 - "Ranking de Fornecedores"
Cohesion: 0.17
Nodes (23): Abas: Melhores Opções / Relacionados / Avaliações (5), CTA Ir ao Site (fornecedor online), CTA Ver no Mapa (fornecedor local), Ranking de Fornecedores (Melhores Opções), Selo Menor Preço, 'Atualizado agora' Live Update Indicator, Neighborhood Label for Local Suppliers, Category Count Cards (Eletronicos 2.4k, Moda 1.8k, Casa 3.1k, Esporte 920, Eletrodomesticos 1.2k, Saude & Beleza 1.5k) (+15 more)

### Community 1 - "Projeto e Fluxo de Busca"
Cohesion: 0.17
Nodes (21): Botão 'Continuar', Barra de Progresso (Passo 2 de 3), Botao Continuar, Header SLZ (Como Funciona, Fornecedores, Sobre, Entrar), Tela 03 - Busca passo 2: prazo, Indicador de Progresso Passo 3 de 3, Navbar Busca Inteligente São Luís · MA, Tela 04 - Busca passo 3: orcamento (+13 more)

### Community 2 - "Home e Passo 1 (Produto)"
Cohesion: 0.18
Nodes (15): Selo 'IA ativa - Benchmarking em tempo real', Campo de Busca + CTA 'Personalizar busca', Explorar Categorias (Eletronicos, Moda, Casa, Esporte, Eletrodomesticos, Saude & Beleza), Modos de Busca (Busca / Link / Imagem), Barra de Navegacao (Como Funciona, Fornecedores, Sobre, Entrar), Sugestoes Rapidas (iPhone 15, Notebook Samsung, Smart TV 50, Air Fryer, Tenis Nike), Tela 01 - Tela inicial (Home), Buscas Populares (chips de sugestão) (+7 more)

### Community 3 - "Prazo e Critérios"
Cohesion: 0.26
Nodes (12): Headline 'Compre mais inteligente em Sao Luis', Opcao: Ate 1 semana (Frete padrao ou retirada) - selecionada, Opcao: Ate 2 semanas (Melhores precos disponiveis), Opcao: Em ate 3 dias (Entrega expressa disponivel), Opcao: Hoje mesmo (Retirada em loja fisica), Opcao: Sem pressa (Priorizo o menor preco), Seletor de Prazo (radio cards), Trade-off Prazo x Preco (+4 more)

### Community 4 - "Veredito e Score da IA"
Cohesion: 0.31
Nodes (10): Card Veredito da IA - Compre localmente, IA Score por Fornecedor, Resumo da Busca (Notebook Samsung · 1 semana · R$ 0-1.000), Score Final 88/100, Selo Melhor Custo-Benefício, Tela 06 - Resultados e recomendacao, Color-coded Score Column, Ranking de opcoes / fornecedores (+2 more)

### Community 5 - "Análise da IA"
Cohesion: 0.25
Nodes (9): Anel de progresso circular (29% analisando), Checklist de etapas da analise da IA, Etapa: Benchmarking local vs online (varrendo fornecedores em Sao Luis), Etapa: Cruzando com seu orcamento e prazo (Ate R$ 1.000 - 1 semana), Etapa: Produto identificado (Notebook Samsung) - concluida, Header: logo SLZ Busca Inteligente Sao Luis-MA + nav (Como Funciona, Fornecedores, Sobre, Entrar), Produto buscado: Notebook Samsung, Tela 05 - IA analisando (+1 more)

### Community 6 - "Como Funciona e Confiabilidade"
Cohesion: 0.32
Nodes (8): Passo 01 - Diga o que quer (produto, prazo e orcamento), Passo 02 - IA analisa tudo (benchmarking local vs online), Passo 03 - Compra ideal (melhor opcao com seguranca), Secao 3 Passos (Como Funciona), Etapa: Auditoria de seguranca (verificando reputacao dos fornecedores), Verified Supplier Checkmark, Criterio: confiabilidade do vendedor, IA de analise e auditoria de fornecedores

### Community 7 - "Orçamento (Passo 3)"
Cohesion: 0.40
Nodes (6): Botão Analisar com IA, Confirmação Orçamento: R$0 – R$1.000, Faixas de Preço Pré-definidas, Pergunta: Qual o seu orçamento?, Sugestão Acima do Orçamento por Custo-Benefício, Valores Personalizados (Mínimo/Máximo R$)

## Ambiguous Edges - Review These
- `Fornecedores online (sites)` → `Opcao: Sem pressa (Priorizo o menor preco)`  [AMBIGUOUS]
  Assets/03-busca-passo2-prazo.png · relation: conceptually_related_to
- `IA de analise e auditoria de fornecedores` → `Modos de Entrada (Digitar / Link / Imagem)`  [AMBIGUOUS]
  Assets/02-busca-passo1-produto.png · relation: conceptually_related_to
- `Landing page` → `Tela 01 - Tela inicial (Home)`  [AMBIGUOUS]
  README.md · relation: conceptually_related_to

## Knowledge Gaps
- **12 isolated node(s):** `Ideia de negocio`, `Busca por texto, link ou imagem`, `Explorar Categorias (Eletronicos, Moda, Casa, Esporte, Eletrodomesticos, Saude & Beleza)`, `Indicador de Progresso 'Passo 1 de 3'`, `Pergunta 'O que você está procurando?'` (+7 more)
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 12 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `Fornecedores locais (lojas de Sao Luis)` connect `Ranking de Fornecedores` to `Projeto e Fluxo de Busca`, `Home e Passo 1 (Produto)`, `Prazo e Critérios`, `Veredito e Score da IA`, `Análise da IA`, `Como Funciona e Confiabilidade`?**
  _High betweenness centrality (0.166) - this node is a cross-community bridge._
- **Are the 8 inferred relationships involving `Fornecedores locais (lojas de Sao Luis)` (e.g. with `Barra de Navegacao (Como Funciona, Fornecedores, Sobre, Entrar)` and `Barra de Navegação (Como Funciona, Fornecedores, Sobre, Entrar)`) actually correct?**
  _`Fornecedores locais (lojas de Sao Luis)` has 8 INFERRED edges - model-reasoned connections that need verification._
- **What connects `Ideia de negocio`, `Busca por texto, link ou imagem`, `Explorar Categorias (Eletronicos, Moda, Casa, Esporte, Eletrodomesticos, Saude & Beleza)` to the rest of the system?**
  _12 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Why does `IA de analise e auditoria de fornecedores` connect `Como Funciona e Confiabilidade` to `Ranking de Fornecedores`, `Projeto e Fluxo de Busca`, `Home e Passo 1 (Produto)`, `Prazo e Critérios`, `Veredito e Score da IA`, `Análise da IA`, `Orçamento (Passo 3)`?**
  _High betweenness centrality (0.120) - this node is a cross-community bridge._
- **Are the 2 inferred relationships involving `Top 10 Supplier Ranking Table` (e.g. with `IA de analise e auditoria de fornecedores` and `Score de custo-beneficio`) actually correct?**
  _`Top 10 Supplier Ranking Table` has 2 INFERRED edges - model-reasoned connections that need verification._

### Low-confidence Hints
_AMBIGUOUS edges — the extractor was unsure. Verify before acting on these._

- **What is the exact relationship between `Fornecedores online (sites)` and `Opcao: Sem pressa (Priorizo o menor preco)`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **What is the exact relationship between `IA de analise e auditoria de fornecedores` and `Modos de Entrada (Digitar / Link / Imagem)`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._