# DIO-AZ104

# 💻 Gerenciamento de Máquinas Virtuais no Microsoft Azure

Este repositório contém resumos, anotações e dicas sobre o gerenciamento de máquinas virtuais (VMs) no Microsoft Azure. Foi criado como parte de um laboratório prático, com o objetivo de servir como material de apoio para estudos e futuras implementações em ambientes de nuvem.

---

## 📘 Sumário

- [Introdução](#introdução)
- [Criação de uma Máquina Virtual](#criação-de-uma-máquina-virtual)
- [Gerenciamento de Acesso](#gerenciamento-de-acesso)
- [Redes e Segurança](#redes-e-segurança)
- [Extensões e Automação](#extensões-e-automação)
- [Dicas Úteis](#dicas-úteis)
- [Recursos Complementares](#recursos-complementares)

---

## 📖 Introdução

O Azure oferece uma plataforma robusta para criar e gerenciar máquinas virtuais com alta disponibilidade, escalabilidade e integração com outros serviços. As VMs são ideais para executar aplicativos, bancos de dados, serviços de backend e ambientes de desenvolvimento.

---

## 🚀 Criação de uma Máquina Virtual

### Etapas básicas:
1. **Escolher uma imagem (SO):** Ubuntu, Windows Server, Red Hat, etc.
2. **Selecionar o tamanho da VM:** baseada em CPU, memória e armazenamento.
3. **Configurar autenticação:** chave SSH (Linux) ou usuário/senha (Windows).
4. **Definir rede virtual, sub-rede e grupo de segurança (NSG).**
5. **Atribuir um disco gerenciado e opcionalmente discos adicionais.**
6. **Revisar e criar.**

---

## 🔐 Gerenciamento de Acesso

- **Melhor prática para Linux:** Autenticação por **chave SSH**, com restrições de IP.
- **Para segurança adicional:** Utilize o **Azure Bastion** para acesso remoto via navegador sem expor portas (como SSH ou RDP).
- **Permissões e RBAC:** Gerencie o acesso à VM usando **Controle de Acesso Baseado em Função (RBAC)** do Azure.

---

## 🌐 Redes e Segurança

- **NSG (Network Security Group):** Controla o tráfego de entrada e saída.
- **IPs públicos vs. privados:** Avalie se a VM precisa estar exposta à internet.
- **DNS e nome da VM:** Configurável para facilitar a conexão e o monitoramento.

---

## ⚙️ Extensões e Automação

- **Extensões da VM:** Permitem executar scripts, instalar agentes, configurar softwares.
- **Custom Script Extension:** Útil para instalar pacotes e configurar a VM durante ou após a criação.
- **Azure CLI / PowerShell:** Automação via scripts para provisionar e gerenciar VMs.
- **Imagens personalizadas:** Crie uma imagem base com pré-configuração para replicar facilmente outras VMs.

---

## 💡 Dicas Úteis

- **Evite expor portas como SSH (22) e RDP (3389) diretamente à internet.**
- **Crie snapshots de discos para backup ou replicação.**
- **Use tags em recursos para facilitar a organização e faturamento.**
- **Configure alertas e monitoramento com Azure Monitor e Log Analytics.**
