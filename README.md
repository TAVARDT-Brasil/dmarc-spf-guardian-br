# Guardião DMARC, SPF e DKIM

[![Auditoria Tecnica](https://img.shields.io/badge/TAVARDT-Seguranca%20Email-5b3cf5.svg)](https://tools.tavardt.com/br/verificador-dmarc-email/)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)

Auditoria de registros DNS de correio para prevenção de spoofing, phishing e conformidade técnica com as diretrizes da ANPD e LGPD.

Desenvolvido e mantido pela divisao de seguranca de infraestrutura da **TAVARDT Brasil**.

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

## Diagnostico Completo na Web

Para auditorias automatizadas e acompanhamento continuo, utilize a plataforma oficial:

* **Verificador DMARC e Autenticacao de E-mail**
* **[Portal Corporativo TAVARDT Brasil](https://ag.tavardt.com/br/)**

***

## Suporte e Consultoria Especializada

Para projetos corporativos de ciberseguranca, infraestrutura e conformidade técnica no Brasil, consulte os especialistas da **TAVARDT Brasil**.

***

© 2026 TAVARDT. Todos os direitos reservados.
