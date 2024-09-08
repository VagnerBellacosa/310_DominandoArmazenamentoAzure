# O que são os Arquivos do Azure?

Neste artigo

[Por que o serviço Arquivos do Azure é útil](https://learn.microsoft.com/pt-br/azure/storage/files/storage-files-introduction#why-azure-files-is-useful)

[Principais benefícios](https://learn.microsoft.com/pt-br/azure/storage/files/storage-files-introduction#key-benefits)

[Treinamento](https://learn.microsoft.com/pt-br/azure/storage/files/storage-files-introduction#training)

[Arquitetura](https://learn.microsoft.com/pt-br/azure/storage/files/storage-files-introduction#architecture)

Os Arquivos do Azure oferecem compartilhamentos de arquivos totalmente gerenciados na nuvem que são acessíveis por meio do [protocolo SMB](https://learn.microsoft.com/pt-br/windows/win32/fileio/microsoft-smb-protocol-and-cifs-protocol-overview), do [protocolo NFS (Network File System)](https://en.wikipedia.org/wiki/Network_File_System) e da [API REST dos Arquivos do Azure](https://learn.microsoft.com/pt-br/rest/api/storageservices/file-service-rest-api) padrão do setor. Os compartilhamentos de arquivos do Azure podem ser montados de maneira simultânea por implantações locais ou na nuvem. É possível acessar os compartilhamentos de Arquivos do Azure do protocolo SMB em clientes Windows, Linux e macOS. É possível acessar os compartilhamentos de arquivo do Azure do protocolo NFS de clientes Linux. Além disso, os compartilhamentos de arquivos do Azure do protocolo SMB podem ser armazenados em cache em servidores Windows com a [Sincronização de Arquivos do Azure](https://learn.microsoft.com/pt-br/azure/storage/file-sync/file-sync-introduction) para acesso rápido perto de onde os dados estão sendo usados.

Veja alguns vídeos sobre os casos de uso comuns dos Arquivos do Azure:

- [Substitua o servidor de arquivos por um compartilhamento de arquivo do Azure sem servidor](https://youtu.be/H04e9AgbcSc)
- [Introdução a contêineres de perfil FSLogix nos Arquivos do Azure na Área de Trabalho Virtual do Azure usando a autenticação do AD](https://www.youtube.com/embed/9S5A1IJqfOQ)

Para começar a usar Arquivos do Azure, consulte [Início Rápido: criar e usar um compartilhamento de arquivos do Azure](https://learn.microsoft.com/pt-br/azure/storage/files/storage-how-to-use-files-portal).



## Por que o serviço Arquivos do Azure é útil

Você pode usar compartilhamentos de arquivos do Azure para:

- **Substituir ou complementar os servidores de arquivos locais**:
  Use os Arquivos do Azure para substituir ou complementar servidores de arquivos locais tradicionais ou dispositivos NAS (armazenamento anexado à rede). Sistemas operacionais conhecidos, como o Linux, Windows e macOS podem montar diretamente compartilhamentos de arquivos do Azure em qualquer lugar do mundo. Os compartilhamentos de arquivos do Azure do protocolo SMB também podem ser replicados com a Sincronização de Arquivos do Azure para servidores Windows, no local ou na nuvem, para armazenamento dos dados em cache distribuído e com desempenho. Com a [Autenticação do AD dos Arquivos do Azure](https://learn.microsoft.com/pt-br/azure/storage/files/storage-files-active-directory-overview), os compartilhamentos de arquivos do Azure do protocolo SMB podem funcionar com o Active Directory Domain Services (AD DS) hospedados localmente para controle de acesso.
- **Aplicativos de "Deslocamento e comparação"** :
  O serviço Arquivos do Azure facilita "comparar e deslocar" aplicativos para a nuvem que espera que o compartilhamento de arquivos armazene o aplicativo de arquivo ou os dados do usuário. O serviço Arquivos do Azure permite o cenário “clássico” de comparar e deslocar, em que o aplicativo e os dados são movidos para o Azure, e o cenário “híbrido”, em que os dados do aplicativo são movidos para o serviço Arquivos do Azure e o aplicativo continua a ser executado no local.
- **Simplificar o desenvolvimento na nuvem**:
  Você pode usar os Arquivos do Azure para simplificar os novos projetos de desenvolvimento em nuvem. Por exemplo:
  - **Configurações de aplicativo compartilhado**:
    Um padrão comum para aplicativos distribuídos é fazer com que os arquivos de configuração fiquem em um local centralizado, onde possam ser acessados de diversas instâncias de aplicativos. As instâncias do aplicativo podem carregar sua configuração por meio da [API REST dos Arquivos do Azure](https://learn.microsoft.com/pt-br/rest/api/storageservices/file-service-rest-api) e os usuários podem acessá-las montando o compartilhamento localmente.
  - **Compartilhamento de diagnóstico**:
    Um compartilhamento de arquivos do Azure é um local conveniente para aplicativos de nuvem gravarem seus logs, métricas e despejos de memória. Os logs podem ser gravados pelas instâncias do aplicativo por meio da API REST de Arquivo e os desenvolvedores podem acessá-los ao montar o compartilhamento de arquivos em seu computador local. Isso permite maior flexibilidade, já que os desenvolvedores podem adotar o desenvolvimento em nuvem sem a necessidade de abandonar as ferramentas existentes que conhecemos e amamos.
  - **Desenv/Teste/Depuração**:
    Quando desenvolvedores ou administradores estão trabalhando em máquinas virtuais na nuvem, eles frequentemente precisam de um conjunto de ferramentas ou utilitários. Copiar tais ferramentas e utilitários em cada VM pode ser uma atividade demorada. Ao montar um compartilhamento de arquivos do Azure localmente nas máquinas virtuais, o desenvolvedor e o administrador podem acessar rapidamente suas ferramentas e utilitários sem precisar copiá-las.
- **Transporte em contêineres**:
  Você também pode usar compartilhamentos de arquivos do Azure como volumes persistentes para contêineres com estado. Os contêineres oferecem recursos do tipo "compilar uma vez, executar em qualquer lugar", que permitem aos desenvolvedores acelerar a inovação. Para os contêineres que acessam dados brutos a cada início, é necessário um sistema de arquivos compartilhado para permitir que esses contêineres acessem o sistema de arquivos, independentemente da instância em que eles são executados.



## Principais benefícios

- **Fácil de usar**. Quando um compartilhamento de arquivos do Azure é montado em seu computador, você não precisa fazer nada especial para acessar os dados: basta navegar até o caminho em que o compartilhamento de arquivos está montado e abrir/modificar um arquivo.
- **Acesso compartilhado**. Os compartilhamentos de arquivos do Azure são compatíveis com os protocolos SMB e NFS padrão. Isso significa que você pode substituir facilmente seus compartilhamentos de arquivos locais pelos do Azure sem se preocupar com a compatibilidade do aplicativo. Poder compartilhar um sistema de arquivos em vários computadores, aplicativos e instâncias de aplicativo é uma vantagem significativa para aplicativos que precisam de compartilhamento.
- **Totalmente gerenciado**. Os compartilhamentos de arquivos do Azure podem ser criados sem a necessidade de gerenciar um sistema operacional ou hardware. Isso significa que você não precisa lidar com a correção do sistema operacional do servidor com atualizações críticas de segurança ou com a substituição de discos rígidos com defeito.
- **Scripts e ferramentas**. Você pode usar os cmdlets do PowerShell e a CLI do Azure para criar, montar e gerenciar compartilhamentos de arquivos do Azure como parte da administração de aplicativos do Azure. Crie e gerencie compartilhamentos de arquivos do Azure usando o portal do Azure e o Gerenciador de Armazenamento do Azure.
- **Resiliência**. Os Arquivos do Azure são criados para estar sempre disponíveis. Substituir os compartilhamentos de arquivos locais pelos Arquivos do Azure significa que não é preciso estar ativado para lidar com interrupções locais de energia ou problemas de rede.
- **Programação familiar**. Os aplicativos executados no Azure podem acessar dados no compartilhamento por meio de [APIs de E/S do sistema](https://learn.microsoft.com/pt-br/dotnet/api/system.io.file) de arquivos. Os desenvolvedores podem, portanto, utilizar seus códigos e habilidades existentes para migrar aplicativos existentes. Além das APIs de E/S do sistema, você pode usar as [Bibliotecas de Clientes do Armazenamento do Azure](https://learn.microsoft.com/pt-br/previous-versions/azure/dn261237(v=azure.100)) ou a [API REST dos Arquivos do Azure](https://learn.microsoft.com/pt-br/rest/api/storageservices/file-service-rest-api).



## Treinamento

Para obter treinamentos individuais, consulte os seguintes módulos:

- [Introdução aos Arquivos do Azure](https://learn.microsoft.com/pt-br/training/modules/introduction-to-azure-files/)
- [Configurar os Arquivos do Azure e a Sincronização de Arquivos do Azure](https://learn.microsoft.com/pt-br/training/modules/configure-azure-files-file-sync/)



## Arquitetura

Para obter diretrizes sobre como projetar soluções nos Arquivos do Azure usando padrões e práticas estabelecidas, consulte o seguinte:

- [Compartilhamento de arquivo em nuvem do Azure Enterprise](https://learn.microsoft.com/pt-br/azure/architecture/hybrid/azure-files-private)
- [Serviços de arquivo híbrido](https://learn.microsoft.com/pt-br/azure/architecture/hybrid/hybrid-file-services)
- [Usar compartilhamentos de arquivos do Azure em um ambiente híbrido](https://learn.microsoft.com/pt-br/azure/architecture/hybrid/azure-file-share)
- [Compartilhamento de arquivo híbrido com recuperação de desastre para funcionários de filiais locais e remotas](https://learn.microsoft.com/pt-br/azure/architecture/example-scenario/hybrid/hybrid-file-share-dr-remote-local-branch-workers)
- [Arquivos do Azure acessados localmente e protegidos pelo AD DS](https://learn.microsoft.com/pt-br/azure/architecture/example-scenario/hybrid/azure-files-on-premises-authentication)



## Estudos de caso

- Organizações em todo o mundo estão aproveitando os Arquivos do Azure e a Sincronização de Arquivos do Azure para otimizar o acesso e o armazenamento de arquivos. [Verifique os estudos de caso delas aqui](https://learn.microsoft.com/pt-br/azure/storage/files/azure-files-case-study).



## Próximas etapas

- [Planejar uma implantação de Arquivos do Azure](https://learn.microsoft.com/pt-br/azure/storage/files/storage-files-planning)
- [Criar um compartilhamento de arquivos do Azure](https://learn.microsoft.com/pt-br/azure/storage/files/storage-how-to-create-file-share)
- [Conectar e montar um compartilhamento SMB no Windows](https://learn.microsoft.com/pt-br/azure/storage/files/storage-how-to-use-files-windows)
- [Conectar e montar um compartilhamento SMB no Linux](https://learn.microsoft.com/pt-br/azure/storage/files/storage-how-to-use-files-linux)
- [Conectar e montar um compartilhamento SMB no macOS](https://learn.microsoft.com/pt-br/azure/storage/files/storage-how-to-use-files-mac)
- [Conectar e montar um compartilhamento do protocolo NFS no Linux](https://learn.microsoft.com/pt-br/azure/storage/files/storage-files-how-to-mount-nfs-shares)
- [Perguntas frequentes sobre os Arquivos do Azure](https://learn.microsoft.com/pt-br/azure/storage/files/storage-files-faq)