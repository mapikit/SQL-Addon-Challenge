# Regras do Desafio

Neste arquivo estão descritas as regras e o funcionamento do Desafio. Certifique-se de ler tudo com atenção para garantir que sua submissão tenha uma boa pontuação e você não perca os prazos de envio!

## Etapas e Prazos
O desafio está dividido em 3 etapas, com os prazos ainda a serem definidos:

1. ATUAL -> **Inscrição** - Os participantes registram seu grupo.
2. **Desenvolvimento** - Os participantes desenvolvem seus Addons e enviam a solução do desafio.
3. **Avaliação** - Os juízes darão suas notas para as submissões, e uma votação da comunidade será realizada.
4. **Apresentação** - A votação é encerrada, os resultados do desafio serão revelados e os prêmios distribuídos.

## O Que Você Vai Criar
Aqui estão algumas informações básicas sobre o que seu Addon precisará lidar. Alguns desses detalhes vêm do Meta-System e são explicados detalhadamente na documentação. A seguir, um resumo rápido do que mais importa para este desafio.

> Você pode se juntar ao [Discord do Meta-System](https://discord.gg/ndGsnbTW7V) ou enviar uma DM para Zelcion no [X](https://twitter.com/ZelcionV) ou Discord para esclarecer qualquer dúvida que possa ter.

#### Informações
- 👉 **Schemas** podem ter qualquer formato, incluindo serem profundos. Os schemas usados para avaliar o Addon não serão revelados até o fim do período de submissão do desafio. [Veja aqui sobre os Schemas](https://mapikit.github.io/meta-system-docs/docs/api-docs/configuring/schema-config).
- 👉 **Funções de Schema** têm apenas um único parâmetro, que é um objeto. O addon pode especificar qual é o formato desse objeto. A saída também deve ser um objeto. [Veja aqui sobre Funções de Schema](https://mapikit.github.io/meta-system-docs/docs/guides/broker#entity-schema-functions---brokerschemafunctions).
- 👉 **Schemas** podem mudar de formato entre inicializações.
- 👉 **O Addon** não deve validar a entrada de suas Funções de Schema. Isso é feito no Meta-System através de suas configurações.
#### Requisitos
- ❗**O Addon** deve ser capaz de lidar com N quantidade de schemas.
- ❗**O Addon** deve ser capaz de lidar com um Schema que muda de formato entre inicializações sem quebrar a tabela. É aceitável que dados em chaves alteradas sejam deletados.
- ❗**O Addon** deve ter pelo menos uma Função de Schema para cada um dos seguintes:
  - **(C)** Criar uma entidade
  - **(R)** Recuperar entidades com uma consulta
  - **(U)** Atualizar entidades com uma consulta
  - **(D)** Deletar entidades com uma consulta
