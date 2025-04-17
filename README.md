#Anotações e Dicas sobre Microsoft Azure

✅ 1. Conceitos Básicos
Azure é a plataforma de nuvem pública da Microsoft, usada para criar, implantar e gerenciar serviços e aplicativos através de uma rede global de data centers.

É baseada em um modelo pay-as-you-go (pague pelo uso) e oferece serviços em Infraestrutura como Serviço (IaaS), Plataforma como Serviço (PaaS) e Software como Serviço (SaaS).

☁️ 2. Principais Serviços

Categoria	Serviços Relevantes	Função Principal
Computação	Azure Virtual Machines, App Services	Hospedar apps, VMs, APIs
Rede	Azure Virtual Network, Load Balancer	Conectividade, balanceamento
Armazenamento	Azure Blob, File, Disk Storage	Armazenar arquivos, dados
Banco de Dados	Azure SQL, Cosmos DB, PostgreSQL	Gerenciar dados
Segurança	Azure Active Directory, Key Vault	Autenticação, gestão de chaves
🔐 3. Segurança e Identidade
Use Azure Active Directory (AAD) para controle de identidade e autenticação.

Habilite MFA (autenticação multifator) para proteger contas críticas.

RBAC (Role-Based Access Control): Atribua permissões com base em funções, evitando permissões excessivas.

📊 4. Monitoramento e Diagnóstico
Utilize Azure Monitor e Log Analytics para acompanhar o desempenho e integridade dos recursos.

Configure Alertas para notificar falhas ou eventos específicos.

Ferramenta útil: Azure Application Insights para apps em produção.

💰 5. Custos e Planejamento
Use a calculadora de preços do Azure para estimar os custos: https://azure.microsoft.com/en-us/pricing/calculator/

Configure Orçamentos e Alertas de Custos no Cost Management.

Use reservas e instâncias spot para economizar em VMs.

🛠️ 6. Dicas Práticas
🌍 Região importa! Escolha a região mais próxima do seu usuário final para menor latência.

🧪 Testes gratuitos: Use os 12 meses de serviços gratuitos + créditos iniciais para aprendizado.

🔄 Backups: Sempre configure políticas de backup para dados críticos.

⚙️ Infra como Código (IaC): Use ARM Templates, Bicep ou Terraform para automação.

👥 Dev/Test Labs: Ideal para ambientes de teste sem afetar produção.

📚 7. Recursos de Aprendizado
Microsoft Learn – Plataforma oficial com trilhas gratuitas: https://learn.microsoft.com/

Certificações úteis para TI:

AZ-900: Fundamentos do Azure

AZ-104: Administrador do Azure

AZ-500: Segurança no Azure


