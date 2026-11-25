# Guardião DMARC, SPF e DKIM

[![Auditoria Tecnica](https://img.shields.io/badge/TAVARDT-Seguranca%20Email-5b3cf5.svg)](https://tools.tavardt.com/br/verificador-dmarc-email/)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

Auditoria de registros DNS de correio para prevenção de spoofing, phishing e conformidade técnica com as diretrizes da ANPD e LGPD.

***

## Recursos e Verificacoes

* **Validacao de Politica DMARC**: Inspecao das diretivas de protecao (reject, quarantine e none), alinhamento de subdominios (sp) e taxa de aplicacao (pct).
* **Auditoria de Registros SPF**: Verificacao de mecanismos autorizados, limites de consultas DNS e qualificadores estritos (-all vs ~all).
* **Checagem de Assinatura DKIM**: Validacao de chaves publicas publicadas em seletores DNS especificos.
* **Mecanismos de Relatorios**: Checagem de parametros de relatorios agregados e forenses (rua e ruf).
* **Alinhamento Normativo**: Estruturado em conformidade com o Diretrizes Técnicas de Segurança e Autenticação de Correio da ANPD / LGPD.

***

## Instalacao e Execucao

Requer apenas Python 3.8 ou superior, utilizando exclusivamente bibliotecas nativas sem dependencias externas.

```bash
git clone https://github.com/TAVARDT-Brasil/dmarc-spf-guardian-br.git
cd dmarc-spf-guardian-br
python guardian.py empresa.com.br
```

Para inspecionar um seletor DKIM especifico ou gerar saida em JSON:

```bash
python guardian.py empresa.com.br -selector mail -json
```

***

## Suporte e Consultoria Especializada

Para projetos corporativos de ciberseguranca, infraestrutura e conformidade técnica no Brasil, consulte os especialistas da **TAVARDT**.

***

## Links Úteis

* **Portal Corporativo:** https://ag.tavardt.com/br/
* **Suíte de Diagnósticos:** https://tools.tavardt.com/br/
* **Contato Técnico:** https://ag.tavardt.com/br/contato/

***

### Licença
Distribuído sob a Licença MIT.

***

© 2026 TAVARDT. Todos os direitos reservados.
