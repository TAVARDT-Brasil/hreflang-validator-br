# Validador e Auditor de Tags Hreflang e SEO Internacional

[![Validador Hreflang](https://img.shields.io/badge/TAVARDT-Hreflang-5b3cf5.svg)](https://tools.tavardt.com/br/validador-hreflang/)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

Auditoria de reciprocidade de ligacoes alternativas, anotacoes de idioma, mapeamento regional ISO e tags de fallback x-default.

Desenvolvido e mantido pela divisao de engenharia de busca internacional e infraestrutura web da **TAVARDT**.

***

## Capacidades de Auditoria de Hreflang e SEO Internacional

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

## Diagnostico Completo na Web

Para testes visuais e validacao interativa de anotacoes de idioma:

* [Validador Hreflang](https://tools.tavardt.com/br/validador-hreflang/)
* [Portal Corporativo](https://ag.tavardt.com/br/)

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
