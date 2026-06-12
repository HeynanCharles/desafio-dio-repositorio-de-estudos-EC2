# ☁️ Desafio DIO - Gerenciamento de instâncias EC2 na AWS

Esté é um repositório criado para documentação de aprendizados e para futuras consultas em caso de uso em projetos.

Irei compartilhar o que aprendi e entendi do conteúdo por meio de explicações resumidas e algumas das fotos de anotações feitas ao longo das aulas, contendo explicação de conceitos, exemplos dados e ilustrações tanto mostradas em aula quanto criadas para melhor compreendimento.

---

## Tópicos a serem compartilhados:

- [Definição de EC2](https://github.com/HeynanCharles/desafio-dio-repositorio-de-estudos-EC2/tree/main#definição-de-ec2)
- Tipos de instância
- Cálculo de custos
  - AWS Pricing Calculator
  - Convencion name
  - Opções de pagamento
- Otimização de recursos
- Escalação de recursos
- Armazenamento em núvem
  - EBS
  - S3
- Tipos de classe de armazenamento
- Frequência de acesso
- AMI
- Snapshot EBS
- Comparação AMI e Snapshot

---

## Definição de EC2

Elastic Compute Cloud são máquinas virtuais, pendo ter como sistema operacional o Windows ou o Linux

- Com ela pode ser definido segurança básica ultilizando firewall incorporada ao AWS, utilizar grupo de segurança, protocolo, porta, IPs de origem, permite e nega o acesso às suas instâncias EC2;

- Quando criamos um EC2 estamos utilizando o tipo **Infraestrutura como Serviço**, nesse caso, sendo um IAAS (Infraestructure as a service)
  - Nossa responsabilidade seria a dos aplicativos, dados e conexões que fazemos.

A EC2 é composta por:
- CPU
- Rede
- Memória
- Disco
- Sistema operacional

---

## Tipos de instância


<img src="./images/família-instância-ec2.png" alt="Famílias de instâncias EC2" width="600px">

- A T2 é uma das mais ultilizadas, por ser ideal para servidores e banco de dados pequenos

## Cálculo de custos

### AWS Pricing Calculator

<img src="./images/aws-pricing-calculator.png" alt="Tela inicial do AWS Pricing Calculator" width="400px">

Com o AWS Pricing Calculator, você pode calcular o valor de uma instância, personalizando **máquina**(vCPUs, RAM, GB), **instâncias de cidades**, **instâncias compartilhadas**, **hosts dedicados** e até **carga de trabalho** da instância.

- Pode ser feito reservas de instância, compra de instância sob demanda, [entre outros]()

### Covencion name

O Convencion name é a descrição da máquina, como se fosse uma sigla, mas que descreve exatamente que máquina é aquela e um resumo de sua potência.

<img src="./images/convencion-name.png" alt="Tela inicial do AWS Pricing Calculator" width="400px">

### Opções de pagamento

- **Instâncias reservadas** - Costumam ser mais baratas qye a sob demanda, mas por outro lado deve ser paga anualmente, ao contrário da sob demanda. Se a instância não for muito usada, essa opção não é viável.

- **Sob demanda** - Instâncias compradas a uma taxa fixa por hora, sendo recomendada para aplicativos com cargas de trabalho irregulares de curto prazo que não podem ser interrompidas.

- **Instância spot** - Garante a disponibilidade das aplicações sob demanda com descontos de até 90%, mas elas podem ser encerradas a qualquer momento pela AWS, com aviso de dois minutos. Nesse caso, essa forma de pagamento é recomendada para aplicações que suportem falhas e interrupções sem ser prejudicada.

## Otimização de recursos

