# Anotações e Dicas sobre Microsoft Azure

# ✅ 1. Conceitos Básicos
Azure é a plataforma de nuvem pública da Microsoft, usada para criar, implantar e gerenciar serviços e aplicativos através de uma rede global de data centers.

É baseada em um modelo pay-as-you-go (pague pelo uso) e oferece serviços em Infraestrutura como Serviço (IaaS), Plataforma como Serviço (PaaS) e Software como Serviço (SaaS).

# ☁️ 2. Principais Serviços

Categoria	Serviços Relevantes	Função Principal
Computação	Azure Virtual Machines, App Services	Hospedar apps, VMs, APIs
Rede	Azure Virtual Network, Load Balancer	Conectividade, balanceamento
Armazenamento	Azure Blob, File, Disk Storage	Armazenar arquivos, dados
Banco de Dados	Azure SQL, Cosmos DB, PostgreSQL	Gerenciar dados
Segurança	Azure Active Directory, Key Vault	Autenticação, gestão de chaves

# 🔐 3. Segurança e Identidade
Use Azure Active Directory (AAD) para controle de identidade e autenticação.

Habilite MFA (autenticação multifator) para proteger contas críticas.

RBAC (Role-Based Access Control): Atribua permissões com base em funções, evitando permissões excessivas.

# 📊 4. Monitoramento e Diagnóstico
Utilize Azure Monitor e Log Analytics para acompanhar o desempenho e integridade dos recursos.

Configure Alertas para notificar falhas ou eventos específicos.

Ferramenta útil: Azure Application Insights para apps em produção.

# 💰 5. Custos e Planejamento
Use a calculadora de preços do Azure para estimar os custos: https://azure.microsoft.com/en-us/pricing/calculator/

Configure Orçamentos e Alertas de Custos no Cost Management.

Use reservas e instâncias spot para economizar em VMs.

# 🛠️ 6. Dicas Práticas

🌍 Região importa! Escolha a região mais próxima do seu usuário final para menor latência.

🧪 Testes gratuitos: Use os 12 meses de serviços gratuitos + créditos iniciais para aprendizado.

🔄 Backups: Sempre configure políticas de backup para dados críticos.

⚙️ Infra como Código (IaC): Use ARM Templates, Bicep ou Terraform para automação.

👥 Dev/Test Labs: Ideal para ambientes de teste sem afetar produção.

# 📚 7. Recursos de Aprendizado
Microsoft Learn – Plataforma oficial com trilhas gratuitas: https://learn.microsoft.com/

Certificações úteis para TI:

AZ-900: Fundamentos do Azure

AZ-104: Administrador do Azure

AZ-500: Segurança no Azure

# 💻 PASSO A PASSO: CRIAÇÃO DE MÁQUINA VIRTUAL NO MICROSOFT AZURE
🔹 1. Acessar o Portal Azure
Acesse: https://portal.azure.com

Faça login com sua conta Microsoft/Azure.

🔹 2. Navegar até “Máquinas Virtuais”
No menu à esquerda, clique em “Máquinas Virtuais”.

Clique em “+ Criar” > “Máquina Virtual”.

🔹 3. Configurar a Instância da VM (Aba “Básico”)
Preencha os seguintes campos:

##Campo            | O que preencher

Assinatura         | Selecione sua conta/assinatura ativa
Grupo de Recursos  | Crie um novo ou escolha um existente
Nome da VM         | Ex: vm-teste-windows
Região             | Escolha a mais próxima de você
Imagem (SO)        | Windows Server, Ubuntu, etc.
Tamanho da VM      | Selecione um tipo (ex: B1s para testes, D2s para produção)
Usuário/Admin      | Nome de usuário para acesso à VM
Senha/Chave SSH    | Defina a senha ou configure uma chave SSH


# 🔹 4. Discos (Aba “Discos”)
Escolha o tipo de disco para o sistema:

SSD Padrão (bom custo-benefício)

SSD Premium (melhor performance)

Pode adicionar discos adicionais depois, se necessário.

# 🔹 5. Rede (Aba “Rede”)
Configure ou use uma rede virtual (VNet) existente.

Se for um teste, pode manter as opções padrão.

Habilite ou não IP público, dependendo da necessidade.

Grupo de Segurança de Rede (NSG): use o padrão para abrir portas básicas (RDP/SSH).

# 🔹 6. Gerenciamento (Opcional)
Ative o monitoramento com Azure Monitor e Log Analytics, se quiser.

Defina regras de desligamento automático (útil para economizar em ambientes de teste).
# 🔹 7. Revisar + Criar
A aba final “Revisar + criar” mostra um resumo da configuração.

Verifique todos os campos e clique em “Criar”.

# 🔹 8. Aguarde a Provisão
Azure criará a VM e seus recursos associados (discos, IP, rede, etc.).

Em alguns minutos, a VM estará pronta.

# 🔹 9. Acessar a Máquina Virtual
Vá para a VM criada.

Clique em “Conectar”:

Windows: Baixe o arquivo .RDP e conecte com usuário/senha.

Linux: Use SSH com terminal (ex: ssh azureuser@IP_PUBLICO).

# 🛠️ Dicas Extras
🔐 Segurança: Após criar a VM, revise as regras NSG (Firewall) para expor apenas portas necessárias.

💸 Custo: VMs são cobradas por tempo ligado! Desligue-as quando não estiver usando.

📦 Snapshots e Backups: Configure backups automáticos se for produção.

☁️ Script PowerShell ou CLI: Após dominar o portal, tente automatizar usando Azure CLI ou PowerShell.

