# Tratando erros em aplicações Node com práticas de resiliência

Escrever aplicações que são prontas para produção exige mais do que apenas funcionar. Num contexto em que cloud computing e modelos distribuídos são regra, é importante pensar em como o sistema irá tratar eventuais falhas de rede, picos de tráfego e sobrecarga, apenas para citar alguns problemas recorrentes.

Nesse artigo, vamos entender um pouco sobre principios de arquietetura e padrões de projeto que são úteis nesse contexto, além de como implementá-los em soluções usando uma stack baseada em Node.js. 

## Introdução

Para começarmos, vamos pensar em um cenário hipotético, porem recorrente.

Suponha que você é uma engenheira de software da maior empresa varejista do país. É a última sexta-feira de Novembro, a famosa Black Friday, e para incentivar ainda mais as compras no seu *novo e-commerce*, foram disponibilizados cupons de desconto válidos somente para hoje. Tendo em vista essa situação, pagamentos que dão errado, cupons inválidos, leituras e escritas em escala no banco de dados (que podem trazer lentidão) ou ainda perdas de pacotes por conta da grande quantidade de tráfego na rede são o início de uma lista de problemas que devem ser levados em conta. De forma geral, tudo que pode dar errado em seu sistema, em algum momento de sua vida útil, irá acontecer - já dizia nosso amigo Murphy e sua lei.

A questão é que não existe uma fórmula mágica para evitar dores de cabeça. É preciso ter proatividade quanto aos problemas conhecidos e por meio de diferentes técnicas de monitoramento e testes, atuar nos problemas desconhecidos, assim que eles forem descobertos - antes que se tornem monstros impossíveis de conter.

## Como evitar que minha aplicação falhe
### Detectando pontos únicos de falha
### Testes de código, resiliência, carga e de caos
### Detecção e mitigação de falhas de forma automática
### Procedimentos padronizados e documentados para ação em catástrofes

## Fallbacks, falhando com elegância
### O que é uma política de fallback

## Fallbacks, do macro ao micro
### Fallbacks no fluxo do produto
### Fallbacks na sua arquitetura
### Fallbacks na sua aplicação
#### Retry
#### Circuit Breaker
#### Timeout

## Chaos Engineering

## Resumindo, tratamento de erros é difícil, mas possível

# Referências
- [1] [Transient fault handling (Microsoft Docs)](https://docs.microsoft.com/en-us/azure/architecture/best-practices/transient-faults)

- [2] [Transient fault handling and proactive resilience engineering (Polly Wiki)](https://github.com/App-vNext/Polly/wiki/Transient-fault-handling-and-proactive-resilience-engineering)

- [3] [Cockatiel Readme](https://github.com/connor4312/cockatiel#readme)

- [4] [Microsserviços prontos para produção](https://www.amazon.com.br/Microsservi%C3%A7os-Prontos-Para-Produ%C3%A7%C3%A3o-Padronizados/dp/8575226215)
