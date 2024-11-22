# GS-1-Sem---Edge-Computing
Integrantes:
Alan De Castro De Archangelo RM: 560152
Lucas Cortizo Carvalho RM: 559734

Visando o projeto da Global Solution proposto relacionado a Energia Limpa e Sustentável para um futuro melhor, nosso grupo desenvolveu uma idéia baseada nos conceitos de Smart Farm.
Smart Farm traduzindo significa Fazenda Inteligente, ou seja, através do uso da tecnologia e inteligências artificiais automatizar processos diários de uma fazenda que facilitam o trabalho e também ajudam a economizar energia e consequentemente gastos.
Em nosso projeto com os componentes apresentados nós apresentamos uma solução para o desperdício de água e energia em equipamentos que ficam constantemente ligados para manter o solo em perfeito estado para cultivação, dessa forma utilizando um sensor de distância para identificar a altura da água em relação ao solo e também um DHT22 para realizar a leitura da umidade e temperatura do solo nós conseguimos ordenar o ativamento de uma bomba de água apenas em niveis extremos em que o solo se encontra muito quente e pouco umido consequentemente também tornando a distância maior. Utilizamos o LCD 20x4(I2C) para demonstrar as informações em tempo real para melhor monitoramento do circuito.

Os componentes seguem o seguintes parâmetros

Led Verde - Representa o Nivel Controlado
Acende com as seguintes condições:
Temperatura <= 20°C
Umidade >= 50%
Distância  <= 50cm

Led Amarelo - Representa o Nivel de Alerta
Acende com as seguintes condições:
Temperatura > 20°C e Temperatura < 40°C
Umidade > 30% e Umidade < 50%
Distânca < 100cm e Distância > 50cm

Led Vermelho - Representa o Nivel Crítico
Acende com as seguintes condições:
Temperatura >= 40°C
Umidade <= 30%
Distância >= 100cm

Led Azul - Representa a Bomba da Água
Se ativa quando o sistem está em nivel crítico:
Buzzer - Se ativa e desativa por 2 segundos para alertar a emergência
Representa o bombeamento de água para controlar os niveis de umidade e temperatura.
