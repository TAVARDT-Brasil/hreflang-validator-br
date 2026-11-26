<p align="center">
  <a href="https://ag.tavardt.com/br/">
    <img src="https://ag.tavardt.com/img/tavardt-banner.png" alt="TAVARDT" width="1024" />
  </a>
</p>

# Validador e Auditor de Tags Hreflang e SEO Internacional

[![Validador Hreflang](https://img.shields.io/badge/TAVARDT-Hreflang-5b3cf5.svg)](https://tools.tavardt.com/br/validador-hreflang/)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

Auditoria de reciprocidade de ligacoes alternativas, anotacoes de idioma, mapeamento regional ISO e tags de fallback x-default.

Desenvolvido e mantido pela divisao de engenharia de busca internacional e infraestrutura web da **TAVARDT**.

***

## Vetores de Risco e Impacto Operacional em SEO Internacional

Falhas na configuracao de tags hreflang provocam anomalias severas de rastreamento e canibalizacao de indexacao organica. Quando as anotacoes regionais nao possuem links reciprocos ou autorreferenciais, os buscadores descartam silenciosamente a segmentacao internacional.

Essa quebra expoe plataformas brasileiras a perdas graves de conversao e exibicao indevida de paginas internacionais nos resultados de busca locais. A auditoria continua assegura que o publico do Brasil encontre landing pages adequadas com total integridade tecnica.

***

## Capacidades Centrais de Auditoria Tecnica

* **Verificacao de Tag Autorreferencial**: Checagem automatica de presenca da URL atual nas anotacoes de idioma, prevenindo descarte de sinais internacionais pelos buscadores.
* **Inspecao de Fallback x-default**: Validacao da presenca da rota padrao para usuarios globais fora das regioes explicitamente mapeadas.
* **Validacao de Padroes ISO 639-1 e ISO 3166-1**: Checagem de conformidade de codigos de idioma e regiao (como pt-BR), identificando formatos invalidos ou invertidos.
* **Deteccao de Conflito com Canonical**: Identificacao de divergencias criticas onde a tag canonical aponta para URL diferente da anotacao alternativa analisada.
* **Extracao em Dupla Fonte**: Leitura de anotacoes tanto em elementos HTML `<head>` quanto no cabecalho HTTP Link da resposta.
* **Indice de Saude Internacional**: Calculo quantitativo de 0 a 100 classificando o site em COMPLIANT, WARNING ou CRITICAL com alertas objetivos.

***

## Instalacao e Execucao

Requer Python 3.8 ou superior sem dependencias externas adicionais.

```bash
git clone https://github.com/TAVARDT-Brasil/hreflang-validator-br.git
cd hreflang-validator-br
python hreflang_validator.py https://empresa.com.br
```

Para gerar a saida em formato estruturado JSON em esteiras de CI/CD:

```bash
python hreflang_validator.py https://empresa.com.br -j
```

***

## Perguntas Frequentes (FAQ Tecnico)

### 1. O que leva os motores de busca a desconsiderarem as anotacoes hreflang?
A omissao de tags de retorno reciproco e a ausencia da URL autorreferencial invalidam todo o conjunto de anotacoes perante o Googlebot. Este validador detecta a quebra de simetria antes que ocorra prejuizo na indexacao internacional.

### 2. Por que a anotacao x-default e indispensavel em portais globais?
A diretiva x-default define a rota autoritativa de fallback para usuarios provenientes de territorios sem versao linguistica dedicada. Sem ela, os motores de busca tentam deduzir o destino, prejudicando taxas de conversao globais.

### 3. Como a ferramenta identifica conflitos entre canonical e hreflang?
O script processa tanto a tag canonical declarada quanto a lista de ligacoes alternativas para certificar correspondencia absoluta. Qualquer divergencia entre os destinos gera um alerta critico e penaliza a pontuacao em 20 pontos.

### 4. O validador analisa cabecalhos HTTP Link alem de elementos HTML?
Sim, o algoritmo realiza o parsing de diretivas tanto na tag HTML head quanto no cabecalho HTTP Link da resposta. Essa flexibilidade viabiliza a auditoria de documentos nao-HTML, como arquivos PDF e endpoints de API.

### 5. Quais padroes internacionais regulam a validade dos codigos de idioma e regiao?
A ferramenta valida a norma ISO 639-1 para identificadores de idioma de dois caracteres e ISO 3166-1 alpha-2 para qualificadores de pais. Codigos invalidos ou estruturas invertidas resultam em deducao imediata na pontuacao final.

***

## Consultoria em SEO Internacional e Arquitetura Global

Para estruturacao tecnica de portais multirregionais e conformidade com diretrizes do W3C, consulte a equipe da **TAVARDT**.

***

## Links Uteis

* **Portal Corporativo:** https://ag.tavardt.com/br/
* **Suite de Diagnosticos:** https://tools.tavardt.com/br/
* **Contato Tecnico:** https://ag.tavardt.com/br/contato/

***

### Licenca
Distribuido sob a Licenca MIT. Consulte o arquivo LICENSE para termos completos.

***

© 2026 TAVARDT. Todos os direitos reservados.
