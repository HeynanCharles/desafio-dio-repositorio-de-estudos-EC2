# ☁️ Desafio DIO - Gerenciamento de instâncias EC2 na AWS

Esté é um repositório criado para documentação de aprendizados e para futuras consultas em caso de uso em projetos.

Irei compartilhar o que aprendi e entendi do conteúdo por meio de explicações resumidas e algumas das fotos de anotações feitas ao longo das aulas, contendo explicação de conceitos, exemplos dados e ilustrações tanto mostradas em aula quanto criadas para melhor compreendimento.

---

## Tópicos a serem compartilhados:

- Definição de EC2 
- Tipos de instância e algumas formas de uso
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
|
└─ Nossa responsabilidade seria a dos aplicativos, dados e conexões que fazemos.

A EC2 é composta por:
- CPU
- Rede
- Memória
- Disco
- Sistema operacional

## Tipos de instância e algumas formas de uso

!(images/família-instância-ec2.png)