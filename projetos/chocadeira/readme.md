# `Chocadeira Automatizada`
# `Automatic Chicken Brooder`

## Apresentação
O presente projeto foi originado no contexto das atividades da disciplina de graduação *EA075 - Introdução ao Projeto de Sistemas Embarcados*, 
oferecida no segundo semestre de 2023, na Unicamp, sob supervisão da Profa. Dra. Paula Dornhofer Paro Costa, do Departamento de Engenharia de Computação e Automação (DCA) da Faculdade de Engenharia Elétrica e de Computação (FEEC).


 |Nome  | RA | Curso|
|--|--|--|
| Pedro Henrique Ricci Sesti  | 185734  | Eng. Elétrica|
| Matheus Acauã Dias          | 241617  | Eng. Elétrica|


## Descrição do Projeto
A indústria agrícola é um pilar essencial da nossa sociedade, alimentando bilhões de pessoas em todo o mundo. No entanto, enfrenta desafios significativos, como a necessidade de aumentar a eficiência, reduzir o desperdício de recursos e atender à crescente demanda por alimentos de qualidade. A incubação de ovos é uma parte fundamental desse processo, mas é notoriamente trabalhosa e propensa a variações que podem resultar em perdas significativas.

É aqui que entra a nossa Chocadeira Automatizada. Nosso projeto tem como objetivo principal resolver o problema da incubação de ovos de maneira eficiente, confiável e sustentável.

## Descrição Funcional
### Funcionalidades
A Chocadeira Automatizada é um dispositivo projetado para incubação artificial de ovos de aves, como galinhas, patos ou codornas, em um ambiente controlado. Ela automatiza e monitora o processo de incubação, fornecendo condições ideais de temperatura, umidade e viragem dos ovos para garantir taxas de eclosão bem-sucedidas. A Chocadeira Automatizada desse projeto consiste em:

1. **Sistema de aquecimento:** O projeto consiste em um sistema de aquecimento controlado através da dimmerização de uma lâmpada que mantém a temperatura interna da chocadeira na faixa ideal para a incubação dos ovos.

2. **Controle de umidade:** A chocadeira possui um sistema para manter níveis de umidade adequados.

3. **Viragem automática:** Para evitar que o embrião grude na casca e promover seu desenvolvimento uniforme, a Chocadeira Automatizada gira os ovos em intervalos regulares.

4. **Monitoramento e Exibição:** Os dados de temperatura, umidade e tempo restante de incubação serão exibidos em um display LCD para que os usuários possam acompanhar as condições internas da chocadeira.

5. **Notificação de Alarmes:** O sistema será capaz de detectar desvios significativos nas condições de temperatura e umidade e emitir alarmes visuais ou sonoros para alertar os usuários sobre problemas.

   
### Configurabilidade
**Temperatura:** O usuário deve configurar a temperatura da chocadeira de acordo com as especificações da espécie. Isso pode incluir a capacidade de ajustar a temperatura de incubação e uma tolerância (ex: 37°C +- 2°C)

**Umidade:** A configurabilidade da umidade é fundamental para criar as condições ideais para o desenvolvimento dos embriões. O usuário deve ajustar os níveis de umidade e tolerâncias de acordo com as necessidades da espécie.

**Viragem dos ovos:** A chocadeira permite que o usuário configure a frequência da viragem automática dos ovos e quantos dias essa deverá ficar ativa. Além disso, a viragem automática pode ser desativada, dando ao usuário a opção de virar os ovos manualmente.

**Tempo de incubação:** O usuário deverá especificar o tempo de incubação e esse será mostrado no display LCD.

**Alarmes de limite inferior e superior de temperatura e umidade:** O usuário deverá fornecer os limites mínimos e máximos de temperatura e umidade para os quais os alarmes devem ser ativados.

**
### Eventos
#### Periódicos:

1. **Viragem automática dos ovos:** A viragem dos ovos é um evento periódico que ocorre a cada hora durante os primeiros dias de incubação.

2. **Monitoramento da temperatura:** O monitoramento da temperatura é um evento periódico que ocorre continuamente, com leituras geralmente feitas a cada poucos minutos para garantir que a temperatura permaneça dentro da faixa ideal.

3. **Monitoramento da umidade:** O monitoramento da umidade é outro evento periódico que ocorre continuamente, com leituras geralmente feitas a cada poucos minutos para garantir que a umidade esteja dentro da faixa desejada.

#### Não-Periódicos:

1. **Inserção dos ovos:** Quando o usuário prepara a chocadeira para uma nova incubação, insere os ovos no início do processo.

2. **Configuração inicial:** O usuário configura os parâmetros iniciais, como temperatura, umidade e frequência de viragem, no início do processo.

3. **Fim da incubação:** Quando a incubação atinge seu término, ocorre o evento de eclosão, onde os pintinhos nascem dos ovos.

4. **Manutenção e limpeza:** A manutenção e a limpeza da chocadeira são eventos não-periódicos, mas importantes, que podem ocorrer em intervalos irregulares, dependendo da necessidade 

### Tratamento de Eventos

![Draw.io](https://github.com/pedrosesti/ea075-2023.2/blob/main/projetos/chocadeira/chocadeira.drawio.png)

## Referências
>Material da disciplina de graduação *EA075 - Introdução ao Projeto de Sistemas Embarcados*
>https://www.minutorural.com.br/noticia/2312/10-dicas-para-uma-boa-eclosao-na-chocadeira-#:~:text=Em%20chocadeiras%20mais%20simples%2C%20a,evapora%C3%A7%C3%A3o%20e%20menor%20a%20umidade).
>https://www.vetprofissional.com.br/artigos/incubacao-de-ovos-de-galinha-como-e-feito-esse-procedimento
>https://blog.eletrogate.com/wp-content/uploads/2018/12/DHT11-sumrom.pdf
>https://blog.eletrogate.com/sensores-dht11-dht22/

