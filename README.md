# Criação de Máquinas Virtuais no Microsoft Azure

Este documento descreve, de forma introdutória e seguindo o padrão da documentação oficial da Microsoft Azure, o processo de **criação de Máquinas Virtuais (Virtual Machines – VMs)**, abordando também conceitos importantes como **região**, **tipos de VM**, **modelo de cobrança** e **SLA (Service Level Agreement)**.

---

## O que é uma Máquina Virtual no Azure?

Uma **Máquina Virtual (VM)** no Azure é um recurso de computação sob demanda que fornece:

- Sistema operacional (Linux ou Windows)
- CPU, memória e disco configuráveis
- Rede virtual integrada
- Escalabilidade e controle total do ambiente

As VMs permitem executar aplicações, serviços, testes e ambientes educacionais sem a necessidade de hardware físico.

---

## Etapas para Criar uma Máquina Virtual

A criação de uma VM no Azure é feita através do **Azure Portal**, seguindo as etapas abaixo.

### 1️ Seleção da Assinatura e Grupo de Recursos

- **Assinatura**: define o modelo de cobrança e limites disponíveis.
- **Grupo de Recursos**: contêiner lógico que agrupa todos os recursos relacionados à VM (VM, disco, IP, rede).

>  Boas práticas: criar um grupo de recursos exclusivo para cada projeto ou laboratório.

---

### 2️ Escolha da Região

A **região** define o datacenter físico onde a VM será criada.

Exemplos de regiões:
- East US
- West Europe
- North Europe
- Brazil South

A região influencia:
- Disponibilidade de tamanhos de VM
- Latência
- Custo
- Aplicação de SLA

---

### 3️ Seleção da Imagem (Sistema Operacional)

O Azure oferece imagens prontas, como:
- Ubuntu Server
- Windows Server
- Red Hat Enterprise Linux

Para fins de baixo custo, recomenda-se:
- **Linux (ex: Ubuntu Server)**, por consumir menos recursos e crédito, mas para esse exercício em específico foi realizado na versão do Windows para seguir os passos da documentação disponibilizada na aula.

---

### 4️ Escolha do Tamanho da VM

O tamanho da VM define:
- Quantidade de vCPUs
- Memória RAM
- Capacidade de desempenho

>  Nem todos os tamanhos estão disponíveis em todas as regiões ou para todas as assinaturas.

---

### 5️ Configurações de Autenticação

É possível acessar a VM por:
- **Senha**
- **Chave SSH**

Essas credenciais permitem acesso remoto seguro à máquina.

---

### 6️ Revisão e Criação

Antes de criar a VM, o Azure apresenta:
- Validação das configurações
- Estimativa de custo mensal
- Informações sobre disponibilidade

Após a validação, o recurso é provisionado automaticamente.

---

## Conclusão

As Máquinas Virtuais do Azure oferecem flexibilidade, escalabilidade e controle total do ambiente computacional. Entender o processo de criação, as limitações de região e assinatura, bem como o funcionamento do SLA, é essencial para o uso correto da plataforma.

---

