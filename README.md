## Tipos de Serviço de Nuvem - Configurando uma instância de Banco de Dados na Azure

Repositório criado como parte das atividades do **Bootcamp Java Cloud Native - Bradesco** na plataforma [DIO](https://www.dio.me/).  
Aqui exploramos conceitos fundamentais de cloud computing com foco nos serviços da **Microsoft Azure**.

## 🚀 Objetivos do Laboratório
- Compreender os **tipos de serviços de nuvem** (IaaS, PaaS, SaaS).
- Desvendar os principais **serviços do Azure**.
- Criar e configurar uma **máquina virtual (VM)** na Azure.
- Provisionar um **banco de dados SQL** em nuvem.

---

## 📌 Serviços de Nuvem no Azure

### 1. **Tipos de Serviços**
| Tipo          | Descrição                          | Exemplo no Azure               |
|---------------|------------------------------------|--------------------------------|
| **IaaS**      | Infraestrutura como Serviço        | Azure Virtual Machines (VMs)   |
| **PaaS**      | Plataforma como Serviço            | Azure SQL Database             |
| **SaaS**      | Software como Serviço              | Microsoft 365                  |

### 2. **Serviços Azure Utilizados**
- **Azure Virtual Machines (IaaS)**: Máquinas virtuais escaláveis.
- **Azure SQL Database (PaaS)**: Banco de dados gerenciado.
- **Azure Portal**: Interface para gerenciamento de recursos.

---

## 🔧 Passo a Passo do Laboratório

### **Criando uma Máquina Virtual (VM) no Azure**
1. **Acesse o [Portal Azure](https://portal.azure.com/)**.
2. Navegue até **"Virtual Machines"** → **"Criar"**.
3. Configure:
   - **Nome da VM**: `lab-dio-vm`
   - **Imagem**: Ubuntu Server 20.04 LTS
   - **Tamanho**: Standard B1s (1 vCPU, 1 GiB RAM)
   - **Região**: `East US`
4. Defina credenciais de acesso (usuário/senha ou SSH).
5. Revise e clique em **"Criar"**.

📌 **Dica**: Use o [Azure CLI](https://docs.microsoft.com/cli/azure/) para automação:
```bash
az vm create --name lab-dio-vm --image UbuntuLTS --size Standard_B1s --admin-username dio-user
