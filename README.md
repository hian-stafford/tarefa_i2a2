# Cenário

A região amazônica enfrenta desafios crescentes relacionados à gestão dos recursos hídricos e seus impactos diretos na segurança alimentar de comunidades ribeirinhas e agricultores familiares. Nos últimos anos, estiagens prolongadas e enchentes severas alteraram os ciclos naturais, afetando a disponibilidade de água e a produtividade agrícola local.

As comunidades relatam mudanças no regime de chuvas e percebem redução na qualidade da água de igarapés e rios, comprometendo irrigação, consumo humano e atividades produtivas. Também há aumento de doenças transmitidas por água contaminada, afetando diretamente o bem-estar da população.

Dois líderes comunitários solicitaram apoio para entender, com base em dados, como as variações climáticas e os desafios hídricos estão afetando a produção agrícola e a qualidade de vida nas comunidades, buscando sair do campo da percepção para trabalhar com dados reais.

Foram coletadas duas bases de dados:

* **Base climática**: chuvas previstas, chuvas reais, temperatura média, presença de variações climáticas e índice de umidade do solo.
* **Base socioeconômica**: volume de produção agrícola, incidência de doenças relacionadas à água, acesso à água potável e indicadores de segurança alimentar.

Durante a coleta, surgiram desafios como registros duplicados, erros de grafia, formatos de datas diferentes e valores ausentes em variáveis-chave. Também foram identificados possíveis outliers, como registros de chuvas superiores a 700 mm em um único dia, exigindo investigação.

## O seu desafio

Como analista, você deverá transformar esses dados brutos em informações de qualidade. Suas etapas serão:

1. **Definir claramente o problema central**, formulando perguntas inteligentes e identificando métricas relevantes para guiar a análise.
2. **Limpeza e preparação dos dados**, incluindo:

   * Remover duplicatas
   * Padronizar categorias como “sim”, “não” e “nao”
   * Tratar dados ausentes
   * Padronizar formatos de data
   * Tratar outliers, considerando o contexto amazônico
3. **Análise Exploratória de Dados (EDA)**:

   * Explorar distribuições das variáveis
   * Analisar a correlação entre chuvas, produtividade agrícola e incidência de doenças
   * Criar visualizações (histogramas, gráficos de dispersão, heatmaps) para revelar padrões, clusters e relações entre clima, acesso à água e segurança alimentar
4. **Gerar um relatório** com os achados, gráficos, tabelas e uma narrativa explicando o que os dados revelam, servindo como base para possíveis modelos preditivos e ações comunitárias.

---

# Descrição das Variáveis

## Base Climática

* `data` (datetime): data do registro.
* `chuvas_previstas_mm` (float): precipitação prevista em mm (0–200).
* `chuvas_reais_mm` (float): precipitação medida em mm.
* `temperatura_media_C` (float): temperatura média diária em °C (20–35).
* `variacao_climatica` (string): indicador de variação climática (“sim”, “não”).
* `indice_umidade_solo` (float): umidade do solo (%) (10–90).

## Base Socioeconômica

* `data` (datetime): data do registro.
* `volume_producao_tons` (float): volume produzido em toneladas (0.5–20).
* `incidencia_doencas` (int/float): número de casos de doenças hídricas (Poisson λ=2).
* `acesso_agua_potavel` (string): acesso à água potável (“sim”, “não”).
* `indicador_seguranca_alimentar` (float): índice de segurança alimentar (0–100).

---

# Objetivo Pedagógico

* Desenvolver a capacidade de transformar dados brutos em informações confiáveis, aplicando técnicas de limpeza e tratamento de dados em um contexto real da Amazônia.
* Fortalecer o pensamento analítico e crítico por meio da definição clara de problemas, formulação de hipóteses e exploração de relações entre variáveis socioambientais e climáticas.
* Aprimorar habilidades práticas em Análise Exploratória de Dados (EDA), utilizando ferramentas digitais para visualizações, descoberta de padrões e criação de narrativas baseadas em dados.

---

# Critérios de Avaliação

* Clareza na definição do problema
* Coerência na análise dos dados
* Qualidade dos insights gerados
* Organização e apresentação da solução

---
