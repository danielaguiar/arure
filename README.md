# 📘 Guia para Criação de Máquina Virtual na Microsoft Azure

Este guia tem como objetivo descrever passo a passo como criar uma máquina virtual (VM) no Microsoft Azure, utilizando o portal web. Ideal para desenvolvedores, administradores ou qualquer pessoa que deseje iniciar com infraestrutura em nuvem na Azure.

---

## ✅ Pré-requisitos

Antes de começar, certifique-se de:

- Possuir uma [conta Microsoft Azure](https://azure.microsoft.com/)
- Estar logado no [portal Azure](https://portal.azure.com/)
- Ter uma **assinatura ativa** (subscription)

---

## 🚀 Etapas para Criar uma VM

### 1. Acesse o Portal Azure

1. Vá até [https://portal.azure.com](https://portal.azure.com)
2. No menu lateral, clique em **"Máquinas virtuais"** ou procure por "Virtual Machines" na barra de pesquisa.

---

### 2. Inicie a Criação da VM

1. Clique em **"Criar" > "Máquina virtual"**
2. Preencha as informações básicas:

2.1 - Detalhes do projeto
   - **Assinatura**: escolha sua assinatura ativa
   - **Grupo de recursos**: crie um novo ou selecione um existente
  
2.2 - Detalhes da instância
   - **Nome da máquina virtual**: escolha um nome descritivo
   - **Região**: selecione a localização geográfica
   - **Opções de disponibilidade**: zona de disponibilizada
   - **Tipo de segurança**: tipo de segurança na inicilização
   - **Imagem (SO)**: escolha o sistema operacional (ex: Ubuntu, Windows Server)
   - **Arquitetura de VM**: escolha entre arm64 ou x64
   - **Tamanho**: escolha o tamanho da VM com base em CPU/RAM

2.3 - Conta de administrador
   - **Tipo de Autenticação**: tipo de autenticação: chave publica de ssh ou senha
   - **nome de usuário**: nome do usuário administrador de vm

### 3. Configurações de Disco

- Escolha entre discos SSD padrão, SSD premium ou HDD
- Você pode adicionar discos adicionais após a criação

---

### 4. Configurações de Rede

- **Rede virtual**: selecione ou crie uma nova
- **Sub-rede**: selecione ou crie uma nova
- **IP público**: configure para acesso externo (caso necessário)
- **Portas de entrada**: habilite portas como:
  - SSH (22) para Linux
  - RDP (3389) para Windows

### 5. Revisar e Criar

1. Revise todas as configurações
2. Clique em **"Criar"**
3. Aguarde a implantação ser concluída

