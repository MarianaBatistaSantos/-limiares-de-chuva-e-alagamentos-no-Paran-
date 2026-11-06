# Emissões de gases de efeito estufa em Balsa Nova, Campo Largo e Araucária (PR)

Análise de dados abertos para descobrir quais setores mais emitem gases de efeito estufa em municípios da região onde moro, como isso mudou desde 1990 e que ação básica poderia reduzir mais as emissões.

> **Status:** em andamento. Bloco 1 (pergunta e hipóteses) em revisão. Próximo: coletar os dados dos três municípios.

---

## 1. Pergunta do projeto

**Quais setores mais emitem gases de efeito estufa em Balsa Nova, Campo Largo e Araucária, como essas emissões mudaram ao longo dos anos e que ação básica reduziria mais as emissões em cada um?**

**Solução proposta:** uma ação básica, por município, voltada ao setor que mais pesa, com base em planos públicos já existentes (como o Plano de Ação Climática do Paraná).

## 2. Por que este projeto

Eu moro em Balsa Nova e quero entender, com dados reais e oficiais, de onde vêm as emissões da minha região. É um projeto pequeno e fácil de reproduzir, feito para praticar o processo completo de uma análise de dados: coletar, limpar, comparar, visualizar e concluir.

## 3. Fonte principal e escopo

- **Fonte:** SEEG, Sistema de Estimativas de Emissões e Remoções de Gases de Efeito Estufa, do Observatório do Clima (plataforma.seeg.eco.br). Dados por município, por setor, de 1990 em diante.
- **Municípios:** Balsa Nova (onde moro), Campo Largo e Araucária (vizinhos).
- **Setores do SEEG:** Energia, Mudança de Uso da Terra e Floresta, Agropecuária, Resíduos e Processos Industriais.
- **Complementos (previstos):** população dos municípios (IBGE), para comparar emissões por habitante, e o Inventário Estadual de Emissões do Paraná, como referência.

## 4. Definições

- **Emissões:** toneladas de CO₂ equivalente (tCO₂e), conforme o SEEG. A unidade e se o total é bruto ou líquido serão confirmados na documentação da plataforma.
- **Setor que mais pesa:** o setor com maior participação nas emissões totais do município em um ano.
- **Mudança ao longo do tempo:** comparação entre o início da série (1990) e o ano mais recente disponível.

## 5. Hipóteses

Escritas para serem testadas, e não para serem confirmadas. Transparência: eu já tinha visto o gráfico de Campo Largo antes de escrevê-las; os outros municípios ainda não.

1. O setor que mais pesa **não é o mesmo** em todos os municípios.
2. Em Campo Largo, as emissões de Uso da Terra caíram e as de Energia cresceram ao longo da série. Verificar se o mesmo acontece nos outros municípios.
3. A comparação **por habitante** muda o ranking entre os municípios em relação ao total.
4. Mudanças bruscas na série (por exemplo, o setor Energia de Campo Largo só aparecer a partir de 2007) podem ser **efeito do método de cálculo**, e não uma mudança real.

## 6. O que seria uma boa resposta

Uma comparação clara entre os municípios, com o setor dominante de cada um, a evolução desde 1990, os indicadores por habitante e uma ação básica sugerida para o setor que mais pesa.

## 7. Limitações já conhecidas

- Os números do SEEG são **estimativas** calculadas por metodologia, e não medições diretas.
- Os dados são por **setor**, e não por empresa. Dados de empresas só existem quando elas publicam o próprio inventário (por exemplo, no Registro Público de Emissões, que é voluntário), então este projeto não aponta empresas.
- Municípios pequenos têm séries mais sensíveis ao método de estimativa.
- Uma análise com poucos municípios não permite generalizar para o estado.

## 8. Blocos do projeto

1. Pergunta e hipóteses (este documento)
2. Fontes de dados e recorte
3. Coleta dos dados
4. Limpeza e padronização (transformar as colunas de anos em formato longo, com Python)
5. Juntar os municípios e a população (IBGE)
6. Análise exploratória e comparação entre municípios
7. Indicadores (por habitante, participação por setor, variação desde 1990)
8. Dashboard no Power BI
9. Conclusão, ação sugerida e limitações
10. Publicação (GitHub, portfólio e LinkedIn)

## 9. Ferramentas

Python (Pandas), SQL (opcional), Excel e Power BI.

## Autora

Mariana Batista dos Santos, estudante de Análise e Desenvolvimento de Sistemas (PUCPR).
