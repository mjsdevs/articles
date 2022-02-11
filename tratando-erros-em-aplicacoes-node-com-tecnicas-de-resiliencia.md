# Tratando erros em aplicações Node com práticas de resiliência

Escrever aplicações que são prontas para produção exige mais do que apenas funcionar. Num contexto em que cloud computing e modelos distribuídos são regra, é importante pensar em como o sistema irá tratar eventuais falhas de rede, picos de tráfego e lentidão na rede, apenas para citar alguns problemas recorrentes.

## Introdução

Para começarmos, vamos pensar em um cenário hipotético, mas, ao mesmo tempo, bastante real.

É a última sexta-feira de Novembro, a famosa Black Friday, e você é uma engenheira de software da maior empresa varejista do país a qual, para incentivar ainda mais as compras no seu *novo site*, liberou cupons de desconto válidos somente para hoje.

Como tratar os inúmeros casos de falha, como:
- pagamentos que dão errado;
- cupons inválidos;
- leituras e escritas em escala no banco de dados, ficando cada vez mais lentas,
- perdas de pacotes por conta da grande quantidade de tráfego na rede.

Enfim, a lista continua e ela é imensa. Tudo que pode dar errado em seu sistema, em algum momento de sua vida útil, irá acontecer, já dizia nosso amigo Murphy e sua lei. Só vamos torcer para que as coisas não quebrem em uma data tão importante!

A questão é que não existe uma fórmula mágica. É preciso tentar se precaver dos problemas conhecidos e, por meio de diferentes técnicas de monitoramento e testes, atuar em cima de problemas desconhecidos assim que eles forem descobertos, antes que se tornem monstros impossíveis de conter.


# Referências
- [1] [Transient fault handling (Microsoft Docs)](https://docs.microsoft.com/en-us/azure/architecture/best-practices/transient-faults)

- [2] [Transient fault handling and proactive resilience engineering (Polly Wiki)](https://github.com/App-vNext/Polly/wiki/Transient-fault-handling-and-proactive-resilience-engineering)

- [3] [Cockatiel Readme](https://github.com/connor4312/cockatiel#readme)
