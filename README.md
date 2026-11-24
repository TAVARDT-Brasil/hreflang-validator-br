# Validador e Auditor de Tags Hreflang e SEO Internacional

[![Validador Hreflang](https://img.shields.io/badge/TAVARDT-Hreflang-5b3cf5.svg)](https://tools.tavardt.com/br/validador-hreflang/)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

Auditoria de reciprocidade de ligacoes alternativas, anotacoes de idioma, mapeamento regional e tags x-default.

Desenvolvido e mantido pela divisao de engenharia de busca e arquitetura semantica internacional da **TAVARDT**.

***

## Capacidades de Auditoria de Hreflang e SEO Internacional

* **Validacao de Reciprocidade de Links**: Inspeciona se cada URL de destino possui link de retorno correspondente (reciprocal alternate link), evitando desqualificacao pelo Googlebot.
* **Checagem de Codigos ISO 639-1 e ISO 3166-1**: Validacao rigorosa de combinacoes de idioma e regiao (ex: `pt-BR`, `es-ES`, `en-US`), alertando sobre codigos invalidos ou invertidos.
* **Verificacao da Tag x-default**: Assegura a presenca correta de fallback para usuarios de localidades nao segmentadas diretamente.
* **Deteccao de Conflito com Tag Canonica**: Identifica divergencias criticas onde a tag canonical aponta para URL distinta da anotacao hreflang autorreferencial.
* **Indice de Integridade Internacional**: Metrica tecnica de 0 a 100 com relacao detalhada de alertas e passos de mitigacao.

***

## Instalacao e Execucao

Requer Python 3.8 ou superior sem dependencias externas obrigatorias.

```bash
git clone https://github.com/TAVARDT-Brasil/hreflang-validator-br.git
cd hreflang-validator-br
python hreflang_validator.py https://empresa.com.br
```

Para gerar a saida em formato estruturado JSON para integracao em pipelines de CI/CD:

```bash
python hreflang_validator.py https://empresa.com.br -json
```

***

## Diagnostico Completo na Web

Para auditorias profundas e teste visual de matrizes complexas de internacionalizacao:

* **Validador de Hreflang Oficial**
* **[Portal Corporativo TAVARDT](https://ag.tavardt.com/br/)**

***

## Consultoria em SEO Internacional e Arquitetura Global

Para expansao de mercados globais e conformidade com Diretrizes de SEO Internacional e W3C, consulte a equipe da **TAVARDT**.

***

## Links Úteis

* **Portal Corporativo:** https://ag.tavardt.com/br/
* **Suíte de Diagnósticos:** https://tools.tavardt.com/br/
* **Contato Técnico:** https://ag.tavardt.com/br/contato/

***

### Licença
Distribuído sob a Licença MIT. Consulte o arquivo [LICENSE](LICENSE) para obter detalhes completos.

***

© 2026 TAVARDT. Todos os direitos reservados.
