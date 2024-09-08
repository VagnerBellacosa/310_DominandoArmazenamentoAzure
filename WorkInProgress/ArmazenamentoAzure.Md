# Introdução ao Armazenamento do Azure



Neste artigo

[Benefícios do Armazenamento Azure](https://learn.microsoft.com/pt-br/azure/storage/common/storage-introduction#benefits-of-azure-storage)

[Serviços de dados de armazenamento do Azure](https://learn.microsoft.com/pt-br/azure/storage/common/storage-introduction#azure-storage-data-services)

[Examinar as opções para armazenar dados no Azure](https://learn.microsoft.com/pt-br/azure/storage/common/storage-introduction#review-options-for-storing-data-in-azure)

[Cenários de exemplo para serviços de Armazenamento do Microsoft Azure](https://learn.microsoft.com/pt-br/azure/storage/common/storage-introduction#sample-scenarios-for-azure-storage-services)

A plataforma do Armazenamento do Microsoft Azure é a solução de armazenamento em nuvem da Microsoft para cenários de armazenamento de dados modernos. O Armazenamento do Microsoft Azure oferece armazenamento altamente disponível, altamente escalonável, durável e seguro para uma variedade de objetos de dados na nuvem. Os objetos de dados do Armazenamento do Microsoft Azure podem ser acessados de qualquer lugar do mundo por HTTP ou HTTPS por meio de uma API REST. O Armazenamento do Microsoft Azure também oferece bibliotecas de clientes para desenvolvedores que criam aplicativos ou serviços com .NET, Java, Python, JavaScript, C++ e Go. Desenvolvedores e profissionais de TI podem usar o Azure PowerShell e a CLI do Azure para escrever scripts para gerenciamento de dados ou tarefas de configuração. O portal do Azure e o Gerenciador de Armazenamento do Azure fornecem as ferramentas de interface do usuário para interagir com o Armazenamento do Microsoft Azure.



## Benefícios do Armazenamento Azure

Os serviços de Armazenamento do Microsoft Azure oferecem os seguintes benefícios aos desenvolvedores de aplicativos e profissionais de TI:

- **Durável e altamente disponível.** A redundância garante a segurança dos seus dados no caso de falhas de hardware transitórias. Você também pode optar por replicar os dados em data centers ou regiões geográficas para obter mais proteção contra catástrofes locais ou desastres naturais. Os dados replicados dessa maneira permanecem altamente disponíveis no caso de uma interrupção inesperada.
- **Segura.** Todos os dados gravados em uma conta de armazenamento do Azure são criptografados pelo serviço. O Armazenamento do Azure oferece um controle refinado sobre quem possui acesso aos seus dados.
- **Escalonável.** O Armazenamento do Azure foi concebido para ser altamente escalonável e atender às necessidades de desempenho e armazenamento de dados dos aplicativos atuais.
- **Gerenciado.** o Azure cuida da manutenção de hardware, das atualizações e dos problemas críticos para você.
- **Acessível.** Os dados no Armazenamento do Azure são acessíveis de qualquer lugar no mundo por HTTP ou HTTPS. A Microsoft fornece bibliotecas de clientes para o Armazenamento do Microsoft Azure em várias linguagens, incluindo .NET, Java, Node.js, Python, Go, entre outras, bem como uma API REST bem desenvolvida. O Armazenamento do Azure oferece suporte para scripts no Azure PowerShell ou na CLI do Azure. E o Portal do Azure e o Gerenciador de Armazenamento do Azure oferecem soluções visualmente fáceis para o trabalho com os seus dados.



## Serviços de dados de armazenamento do Azure

A plataforma de Armazenamento do Microsoft Azure inclui os seguintes serviços de dados:

- [Blobs do Azure](https://learn.microsoft.com/pt-br/azure/storage/blobs/storage-blobs-introduction): um repositório de objetos altamente escalonável para texto e dados binários. Ela também inclui suporte para análise de Big Data por meio do Data Lake Storage Gen2.
- [Arquivos do Azure](https://learn.microsoft.com/pt-br/azure/storage/files/storage-files-introduction): compartilhamentos de arquivos gerenciados para implantações locais e em nuvem.
- [Azure Elastic SAN](https://learn.microsoft.com/pt-br/azure/storage/elastic-san/elastic-san-introduction): uma solução totalmente integrada que simplifica a implantação, a escala, o gerenciamento e a configuração de uma SAN no Azure.
- [Filas do Azure](https://learn.microsoft.com/pt-br/azure/storage/queues/storage-queues-introduction): um armazenamento de mensagens para um sistema de mensagens confiável entre componentes do aplicativo.
- [Tabelas do Azure](https://learn.microsoft.com/pt-br/azure/storage/tables/table-storage-overview): Um armazenamento NoSQL para um armazenamento sem esquemas de dados estruturados.
- [Azure Managed Disks](https://learn.microsoft.com/pt-br/azure/virtual-machines/managed-disks-overview): volumes de armazenamento no nível do bloco para VMs do Azure.
- [Armazenamento de Contêineres do Azure](https://learn.microsoft.com/pt-br/azure/storage/container-storage/container-storage-introduction): um serviço de gerenciamento de volume, implantação e orquestração criado nativamente para contêineres.

Cada serviço é acessado por meio de uma conta de armazenamento com um endereço exclusivo. Para usá-los, consulte [Criar uma conta de armazenamento](https://learn.microsoft.com/pt-br/azure/storage/common/storage-account-create).

Além disso, o Azure fornece o seguinte armazenamento especializado:

- [Azure NetApp Files](https://learn.microsoft.com/pt-br/azure/azure-netapp-files/azure-netapp-files-introduction): armazenamento de arquivos empresariais com NetApp – facilita para que profissionais de armazenamento e LOB (linha de negócios) de empresas e façam a migração e a execução de aplicativos complexos baseados em arquivo, sem alteração de código. O Azure NetApp Files é gerenciado por meio de contas do NetApp e pode ser acessado por meio de volumes NFS, SMB e protocolo duplo. Para começar a usá-lo, confira [Criar uma conta do NetApp](https://learn.microsoft.com/pt-br/azure/azure-netapp-files/azure-netapp-files-create-netapp-account).

Para obter ajuda ao decidir quais serviços de dados usar para o cenário, confira [Examinar as opções de armazenamento](https://learn.microsoft.com/pt-br/azure/cloud-adoption-framework/ready/considerations/storage-options) no Microsoft Cloud Adoption Framework.



## Examinar as opções para armazenar dados no Azure

O Azure fornece uma variedade de ferramentas e serviços de armazenamento. Para determinar qual tecnologia do Azure é mais adequada para seu cenário, consulte [Revisar suas opções de armazenamento](https://learn.microsoft.com/pt-br/azure/cloud-adoption-framework/ready/considerations/storage-options) na Cloud Adoption Framework do Azure.



## Cenários de exemplo para serviços de Armazenamento do Microsoft Azure

A tabela a seguir compara os serviços do Armazenamento do Microsoft Azure e mostra exemplos de cenários para cada um.

Expandir a tabela

| Recurso                                   | Descrição                                                    | Quando usar                                                  |
| :---------------------------------------- | :----------------------------------------------------------- | :----------------------------------------------------------- |
| **Arquivos do Azure**                     | Oferece compartilhamentos de arquivos na nuvem totalmente gerenciados que você pode acessar em qualquer lugar por meio do [protocolo SMB](https://learn.microsoft.com/pt-br/windows/win32/fileio/microsoft-smb-protocol-and-cifs-protocol-overview), do [protocolo NFS (Network File System)](https://en.wikipedia.org/wiki/Network_File_System) e da [API REST dos Arquivos do Azure](https://learn.microsoft.com/pt-br/rest/api/storageservices/file-service-rest-api) padrão do setor.  Monte compartilhamentos de arquivos do Azure a partir de implantações locais ou na nuvem do Windows, do Linux e do macOS. | Você quer migrar por lift-and-shift um aplicativo para a nuvem que já usa as APIs do sistema de arquivos nativo a fim de compartilhar dados entre ele e outros aplicativos em execução no Azure.  Você quer substituir ou complementar os servidores de arquivos locais ou dispositivos NAS.  Quando desejar armazenar ferramentas de desenvolvimento e depuração que precisam ser acessadas em várias máquinas virtuais. |
| **Azure NetApp Files**                    | Oferece um serviço de NAS totalmente gerenciado, altamente disponível e de nível empresarial capaz de lidar com as cargas de trabalho mais exigentes, de alto desempenho e de baixa latência que demandam recursos avançados de gerenciamento de dados. | Você tem uma carga de trabalho difícil de migrar, como aplicativos Linux e Windows compatíveis com POSIX, SAP HANA, bancos de dados, aplicativos e infraestrutura HPC (computação de alto desempenho) e aplicativos Web empresariais.  Você precisa de suporte para vários protocolos de armazenamento de arquivos em apenas um serviço, incluindo NFSv3, NFSv4.1 e SMB3.1.x, que permita uma ampla gama de cenários de lift-and-shift de aplicativos, sem a necessidade de alterações de código. |
| **Blobs do Azure**                        | Permite que os dados não estruturados sejam armazenados e acessados em grande escala em blobs de blocos.  Também dá suporte ao [Azure Data Lake Storage Gen2](https://learn.microsoft.com/pt-br/azure/storage/blobs/data-lake-storage-introduction) para soluções de análise de big data do enterprise. | Quando desejar que o aplicativo dê suporte a cenários de streaming e de acesso aleatório.  Quando desejar poder acessar dados do aplicativo em qualquer lugar.  Quando desejar criar um lago de dados empresariais no Azure e executar análise de big data. |
| **Azure Elastic SAN**                     | O Azure Elastic SAN é uma solução totalmente integrada que simplifica a implantação, a escala, o gerenciamento e a configuração de uma SAN, oferecendo funcionalidades de nuvem internas, como alta disponibilidade. | Você deseja obter um armazenamento em grande escala que seja interoperável com vários tipos de recursos de computação (como o SQL, o MariaDB, as máquinas virtuais do Azure e o Serviços de Kubernetes do Azure) acessados por meio do protocolo iSCSI ([Internet Small Computer Systems Interface](https://en.wikipedia.org/wiki/ISCSI)). |
| **Discos do Azure**                       | Permite que os dados sejam armazenados de forma persistente e acessados de um disco rígido virtual anexado. | Quando desejar migrar por lift-and-shift aplicativos que usam APIs do sistema de arquivos nativo para ler e gravar dados em discos persistentes.  Você quer armazenar dados que não precisam ser acessados de fora da máquina virtual à qual o disco está anexado. |
| **Armazenamento de Contêineres do Azure** | O Armazenamento de Contêineres do Azure é um serviço de gerenciamento de volume, implantação e orquestração que se integra ao Kubernetes e é criado nativamente para contêineres. | Você quer provisionar volumes persistentes de forma dinâmica e automática para armazenar dados de aplicativos com estado em execução nos clusters do Kubernetes. |
| **Filas do Azure**                        | Permite o enfileiramento de mensagens assíncronas entre componentes do aplicativo. | Quando desejar desacoplar componentes de aplicativos e usar mensagens assíncronas para se comunicar entre elas.  Confira orientações sobre quando usar o armazenamento de Filas versus filas do Barramento de Serviço em [Filas de armazenamento e filas do Barramento de Serviço – comparações e contrastes](https://learn.microsoft.com/pt-br/azure/service-bus-messaging/service-bus-azure-and-service-bus-queues-compared-contrasted). |
| **Tabelas do Azure**                      | Permite a você armazenar dados NoSQL estruturados na nuvem, fornecendo um repositório chave/atributo com um design sem esquema. | Quando desejar armazenar conjuntos de dados flexíveis, como dados de usuário para aplicativos Web, catálogos de endereços, informações sobre dispositivos ou outros tipos de metadados exigidos pelo serviço.  Confira orientações sobre quando usar o Armazenamento de Tabelas versus o Azure Cosmos DB for Table em [Desenvolvimento com o Azure Cosmos DB for Table e o Armazenamento de Tabelas do Azure](https://learn.microsoft.com/pt-br/azure/cosmos-db/table-support). |



## Armazenamento de Blobs

O Armazenamento de Blobs do Azure é uma solução de armazenamento de objetos da Microsoft para a nuvem. O armazenamento de Blobs é otimizado para armazenar grandes quantidades de dados não estruturados, como texto ou dados binários.

O Armazenamento de Blobs é ideal para:

- Fornecimento de imagens ou de documentos diretamente a um navegador.
- Armazenamento de arquivos para acesso distribuído.
- Transmissão por streaming de áudio e vídeo.
- Armazenamento de dados de backup e restauração, recuperação de desastres e arquivamento.
- Armazenamento de dados para análise por um serviço local ou hospedado no Azure.

Os objetos no Armazenamento de Blobs podem ser acessados de qualquer lugar do mundo por meio de HTTP ou HTTPS. Usuários ou aplicativos cliente podem acessar blobs por meio de URLs, da [API REST do Armazenamento do Azure](https://learn.microsoft.com/pt-br/rest/api/storageservices/blob-service-rest-api), do [Azure PowerShell](https://learn.microsoft.com/pt-br/powershell/module/azure.storage), da [CLI do Azure](https://learn.microsoft.com/pt-br/cli/azure/storage) ou de uma biblioteca de cliente de Armazenamento do Azure. As bibliotecas de clientes de armazenamento estão disponíveis para várias linguagens, incluindo [.NET](https://learn.microsoft.com/pt-br/dotnet/api/overview/azure/storage), [Java](https://learn.microsoft.com/pt-br/java/api/overview/azure/storage), [Node.js](https://azure.github.io/azure-storage-node) e [Python](https://learn.microsoft.com/pt-br/python/api/overview/azure/storage).

Os clientes também podem se conectar com segurança ao Armazenamento de Blobs usando o Protocolo SSH de Transferência de Arquivo (SFTP) e montar contêineres de Armazenamento de Blobs usando o protocolo NFS (Sistema de Arquivos de Rede) 3.0.

Para mais informações sobre o Armazenamento de Blobs, confira [Introdução ao Armazenamento de Blobs](https://learn.microsoft.com/pt-br/azure/storage/blobs/storage-blobs-introduction).



## Arquivos do Azure

Os [Arquivos do Azure](https://learn.microsoft.com/pt-br/azure/storage/files/storage-files-introduction) permitem que você configure compartilhamentos de arquivos de rede altamente disponíveis que podem ser acessados por meio do [protocolo SMB](https://learn.microsoft.com/pt-br/windows/win32/fileio/microsoft-smb-protocol-and-cifs-protocol-overview) padrão do setor, do [protocolo NFS (Network File System)](https://en.wikipedia.org/wiki/Network_File_System) e da [API REST dos Arquivos do Azure](https://learn.microsoft.com/pt-br/rest/api/storageservices/file-service-rest-api). Isso significa que várias VMs podem compartilhar os mesmos arquivos com acesso de leitura e gravação. Você também pode ler os arquivos usando a interface REST ou as bibliotecas de cliente de armazenamento.

Uma coisa que diferencia os Arquivos do Azure dos arquivos em um compartilhamento de arquivos corporativo é a capacidade de acessar os arquivos de qualquer lugar do mundo usando uma URL que aponte para o arquivo, e que inclua um token SAS (Assinatura de Acesso Compartilhado). Você pode gerar tokens SAS; eles permitem o acesso específico a um ativo privado durante período especificado.

Os compartilhamentos de arquivos podem ser usados para muitos cenários comuns:

- Muitos aplicativos locais usam compartilhamentos de arquivos. Esse recurso facilita a migração dos aplicativos que compartilham dados com o Azure. Se você montar o compartilhamento de arquivos na mesma letra de unidade usada pelo aplicativo local, a parte de seu aplicativo que acessa o compartilhamento de arquivos deverá funcionar com o mínimo de, ou nenhuma, alteração.
- Os arquivos de configuração podem ser armazenados em um compartilhamento de arquivos e acessados de várias VMs. As ferramentas e utilitários usados por vários desenvolvedores em um grupo podem ser armazenados em um compartilhamento de arquivos, garantindo que todas as pessoas possam encontrá-los, e que usem a mesma versão.
- Logs de recurso, métricas e despejos de memória são apenas três exemplos de dados que podem ser gravados em um compartilhamento de arquivos e processados ou analisados posteriormente.

Para obter mais informações sobre Arquivos do Azure, consulte [Introdução aos Arquivos do Azure](https://learn.microsoft.com/pt-br/azure/storage/files/storage-files-introduction).

Alguns recursos do SMB não são aplicáveis à nuvem. Para obter mais informações, consulte [Recursos sem suporte no serviço Arquivo do Azure](https://learn.microsoft.com/pt-br/rest/api/storageservices/features-not-supported-by-the-azure-file-service).



## Azure Elastic SAN

O Azure Elastic SAN (rede de área de armazenamento) é a resposta da Microsoft para o problema de otimização de carga de trabalho e integração entre os bancos de dados em grande escala e aplicativos críticos de desempenho intensivo. O Elastic SAN é uma solução totalmente integrada que simplifica a implantação, a escala, o gerenciamento e a configuração de uma SAN, oferecendo funcionalidades de nuvem internas, como alta disponibilidade.

O Elastic SAN foi criado para cargas de trabalho com uso intensivo de E/S em grande escala e bancos de dados de nível superior, como SQL e MariaDB, e suporte a hospedagem de cargas de trabalho em máquinas virtuais ou contêineres, como o Serviço de Kubernetes do Azure. Os volumes do Elastic SAN são compatíveis com uma ampla variedade de recursos de computação por meio do protocolo [iSCSI](https://en.wikipedia.org/wiki/ISCSI). Alguns outros benefícios do Elastic SAN incluem uma interface de gerenciamento e implantação simplificada. Como você pode gerenciar o armazenamento para vários recursos de computação em uma só interface e otimização de custo.

Para obter mais informações sobre o Azure Elastic SAN, confira [O que é o Azure Elastic SAN?](https://learn.microsoft.com/pt-br/azure/storage/elastic-san/elastic-san-introduction).



## Armazenamento de Contêineres do Azure

O Armazenamento de Contêineres do Azure se integra ao Kubernetes e utiliza as ofertas existentes do Armazenamento do Microsoft Azure para o armazenamento de dados real, oferecendo uma solução de gerenciamento e orquestração de volumes criada especialmente para contêineres. Você pode escolher qualquer uma das opções de armazenamento de reserva com suporte para criar um pool de armazenamento para seus volumes persistentes.

O Armazenamento de Contêineres do Azure oferece benefícios substanciais:

- Escalonamento horizontal rápido dos pods com estado
- Desempenho aprimorado para cargas de trabalho com estado
- Orquestração de volumes nativa do Kubernetes

Para obter mais informações sobre o Armazenamento de Contêineres do Azure, confira [O que é o Armazenamento de Contêineres do Azure?](https://learn.microsoft.com/pt-br/azure/storage/container-storage/container-storage-introduction).



## Armazenamento de Filas

O serviço Fila do Azure é usado para armazenar e recuperar mensagens. A fila de mensagens pode ser de até 64 KB de tamanho e uma fila pode conter milhões de mensagens. Filas são geralmente usadas para armazenar as listas de mensagens a serem processadas de forma assíncrona.

Por exemplo, digamos que você deseja que seus clientes possam carregar imagens e você deseja criar miniaturas para cada imagem. Você pode fazer com que o cliente aguarde que você crie miniaturas ao carregar as imagens. Uma alternativa seria usar uma fila. Quando o cliente concluir o carregamento, grave uma mensagem na fila. Em seguida, faça com que uma Função do Azure recupere a mensagem da fila e crie as miniaturas. Cada uma das partes desse processamento pode ser dimensionada separadamente oferecendo mais controle durante o ajuste para seu uso.

Para obter mais informações sobre Filas do Azure, consulte [Introdução às Filas do Azure](https://learn.microsoft.com/pt-br/azure/storage/queues/storage-queues-introduction).



## Armazenamento de Tabelas

O armazenamento de Tabelas do Azure agora faz parte do Azure Cosmos DB. Para ver a documentação do armazenamento de Tabelas do Azure, veja a [Visão geral do Armazenamento de Tabelas do Azure](https://learn.microsoft.com/pt-br/azure/storage/tables/table-storage-overview). Além do serviço de Armazenamento de Tabelas do Azure existente, há uma nova oferta do Azure Cosmos DB for Table que fornece tabelas otimizadas para taxa de transferência, distribuição global e índices secundários automáticos. Para saber mais e testar a experiência premium, confira o [Azure Cosmos DB for Table](https://learn.microsoft.com/pt-br/azure/cosmos-db/table-introduction).

Para saber mais informações sobre o armazenamento de tabelas, consulte [Visão geral do armazenamento de Tabelas do Azure](https://learn.microsoft.com/pt-br/azure/storage/tables/table-storage-overview).



## Armazenamento em Disco

Um disco gerenciado do Azure é um disco rígido virtual (VHD). Você pode pensar nisso como um disco físico em um servidor local, mas virtualizado. Os discos gerenciados do Azure são armazenados como blobs de página, que são um objeto de armazenamento de E/S aleatório no Azure. Chamamos um disco gerenciado de 'gerenciado' porque ele é uma abstração em relação aos blobs de páginas, aos contêineres de blob e às contas de armazenamento do Azure. Com discos gerenciados, tudo o que você precisa fazer é provisionar o disco e o Azure cuidará do resto.

Confira mais informações sobre discos gerenciados em [Introdução aos discos gerenciados do Azure](https://learn.microsoft.com/pt-br/azure/virtual-machines/managed-disks-overview).



## Azure NetApp Files

O [Azure NetApp Files](https://learn.microsoft.com/pt-br/azure/azure-netapp-files/azure-netapp-files-introduction) é um serviço de armazenamento de arquivos limitado, de alto desempenho e classe empresarial. O Azure NetApp Files dá suporte a qualquer tipo de carga de trabalho e é altamente disponível por padrão. Você pode selecionar níveis de serviço e desempenho, criar contas do NetApp, pools de capacidade, volumes e gerenciar a proteção de dados.

Para obter mais informações sobre o Azure NetApp Files, confira [Introdução ao Azure NetApp Files](https://learn.microsoft.com/pt-br/azure/azure-netapp-files/azure-netapp-files-introduction).

Para obter uma comparação de Arquivos do Azure e Azure NetApp Files, confira [Comparação entre Arquivos do Azure e Azure NetApp Files](https://learn.microsoft.com/pt-br/azure/storage/files/storage-files-netapp-comparison).



## Tipos de contas de armazenamento

O Armazenamento do Azure oferece diversos tipos de contas de armazenamento. Cada tipo é compatível com recursos diferentes e tem um modelo de preços próprio. Para obter mais informações sobre os tipos de conta de armazenamento, consulte [Visão geral da conta de armazenamento do Azure](https://learn.microsoft.com/pt-br/azure/storage/common/storage-account-overview).



## Acesso seguro às contas de armazenamento

Toda solicitação para o Armazenamento do Microsoft Azure deve ser autorizada. O Armazenamento do Microsoft Azure dá suporte aos seguintes métodos de autorização:

- **Integração do Microsoft Entra para dados de tabelas, blobs, arquivos e filas de espera.** O Armazenamento do Microsoft Azure dá suporte à autenticação e autorização com o Microsoft Entra ID para os serviços de Tabela, Blobs, Arquivos e Filas de Espera por meio do controle de acesso baseado em função (RBAC) do Azure. É recomendável a autorização de solicitações com o Microsoft Entra ID para ter segurança e facilidade de uso superiores. Para saber mais, confira [Autorizar o acesso a dados no Armazenamento do Azure](https://learn.microsoft.com/pt-br/azure/storage/common/authorize-data-access). Confira [Autorizar o acesso aos dados de arquivos no portal do Azure](https://learn.microsoft.com/pt-br/azure/storage/files/authorize-data-operations-portal) para autorizar o acesso aos dados do arquivo usando sua conta do Microsoft Entra.
- **Autenticação baseada em identidade por SMB para Arquivos do Azure.** Os Arquivos do Azure dão suporte à autorização baseada em identidade por SMB (Bloco de Mensagens do Servidor), por meio do Active Directory Domain Services (AD DS), do Microsoft Entra Domain Services ou do Kerberos do Microsoft Entra (somente contas de usuário híbridas). Confira mais informações em [Visão geral do suporte à autenticação baseada em identidade dos Arquivos do Azure para acesso SMB](https://learn.microsoft.com/pt-br/azure/storage/files/storage-files-active-directory-overview) e [Planejamento de uma implantação de Arquivos do Azure](https://learn.microsoft.com/pt-br/azure/storage/files/storage-files-planning#identity).
- **Autorização com Chave Compartilhada.** Os serviços do Azure Storage Blob, Arquivos, Fila e Tabela dão suporte à autorização com Chave Compartilhada. Um cliente que usa uma autorização de Chave Compartilhada transmite um cabeçalho com cada solicitação assinada usando a chave de acesso da conta de armazenamento. Para obter mais informações, consulte [Autorizar com Chave Compartilhada](https://learn.microsoft.com/pt-br/rest/api/storageservices/authorize-with-shared-key).
- **Autorização com SAS (assinaturas de acesso compartilhado).** Uma SAS (assinatura de acesso compartilhado) é uma cadeia de caracteres que contém um token de segurança que pode ser anexado ao URI de um recurso de armazenamento. O token de segurança encapsula restrições, como permissões e o intervalo de acesso. Saiba mais em [Usar SAS (Assinaturas de Acesso Compartilhado)](https://learn.microsoft.com/pt-br/azure/storage/common/storage-sas-overview).
- **Active Directory Domain Services com Azure NetApp Files.** Os recursos do Azure NetApp Files, como volumes SMB, volumes de protocolo duplo e volumes Kerberos NFSv4.1 foram projetados para serem usados com o AD DS. Para obter mais informações, confira [Noções básicas sobre as diretrizes de design de site do Active Directory Domain Services e planejamento do Azure NetApp Files](https://learn.microsoft.com/pt-br/azure/azure-netapp-files/understand-guidelines-active-directory-domain-service-site) ou saiba como [Configurar o ADDS LDAP via TLS para o Azure NetApp Files](https://learn.microsoft.com/pt-br/azure/azure-netapp-files/configure-ldap-over-tls).



## Criptografia

Há dois tipos básicos de criptografia disponíveis para o Armazenamento do Microsoft Azure. Para saber mais sobre segurança e criptografia, consulte o [Guia de segurança do Armazenamento do Azure](https://learn.microsoft.com/pt-br/azure/storage/blobs/security-recommendations).



### Criptografia em repouso

A criptografia do Armazenamento do Microsoft Azure protege seus dados para atender aos compromissos de conformidade e segurança de sua organização. O Armazenamento do Microsoft Azure criptografa automaticamente todos os dados antes de persistir para a conta de armazenamento e os descriptografa antes da recuperação. Os processos de criptografia, descriptografia e gerenciamento de chaves são transparentes para os usuários. Os clientes também podem optar por gerenciar as próprias chaves usando o Azure Key Vault. Para obter mais informações, consulte [Criptografia do Armazenamento do Azure para dados em repouso](https://learn.microsoft.com/pt-br/azure/storage/common/storage-service-encryption).

Todos os volumes do Azure NetApp Files são criptografados usando o padrão FIPS 140-2. Confira as [Perguntas frequentes sobre segurança do Azure NetApp Files](https://learn.microsoft.com/pt-br/azure/azure-netapp-files/faq-security#can-the-storage-be-encrypted-at-rest).



### Criptografia do cliente

As bibliotecas de cliente do Armazenamento do Microsoft Azure fornecem métodos de criptografia de dados antes do envio e descriptografam a resposta. Os dados criptografados por meio da criptografia do lado do cliente também são criptografados em repouso pelo Armazenamento do Microsoft Azure. Saiba mais sobre [Criptografia no lado do cliente com o .NET para o Armazenamento do Microsoft Azure](https://learn.microsoft.com/pt-br/azure/storage/common/storage-client-side-encryption).

O tráfego de dados do Azure NetApp Files é inerentemente seguro por design, pois não fornece um ponto de extremidade público e o tráfego de dados permanece dentro da VNet de propriedade do cliente. Os dados em trânsito não são criptografados por padrão. No entanto, o tráfego de uma VM do Azure (executando um cliente NFS ou SMB) para o Azure NetApp Files é tão seguro quanto qualquer outro tráfego entre VMs do Azure. A criptografia de dados em trânsito NFSv4.1 e SMB3 pode ser habilitada opcionalmente. Confira as [Perguntas frequentes sobre segurança do Azure NetApp Files](https://learn.microsoft.com/pt-br/azure/azure-netapp-files/faq-security#can-the-network-traffic-between-the-azure-vm-and-the-storage-be-encrypted).



## Redundância

Para garantir que seus dados sejam duráveis, o Armazenamento do Microsoft Azure armazena várias cópias de seus dados. Quando você configura sua conta de armazenamento, você seleciona uma opção de redundância. Para obter mais informações, confira [Redundância do Armazenamento do Microsoft Azure](https://learn.microsoft.com/pt-br/azure/storage/common/storage-redundancy?toc=/azure/storage/blobs/toc.json) e [Redundância de dados dos Arquivos do Azure](https://learn.microsoft.com/pt-br/azure/storage/files/files-redundancy).

O Azure NetApp Files fornece armazenamento com redundância local com [disponibilidade de 99,99%](https://azure.microsoft.com/support/legal/sla/netapp/v1_1/).



## Transferir dados do e para o Armazenamento do Microsoft Azure

Você tem várias opções para movimentar dados para dentro ou para fora do Armazenamento do Azure. A opção escolhida depende do tamanho de seu conjunto de dados e da largura de banda da rede. Para obter mais informações, consulte [Escolher uma solução do Azure para transferência de dados](https://learn.microsoft.com/pt-br/azure/storage/common/storage-choose-data-transfer-solution).

O Azure NetApp Files oferece volumes NFS e SMB. Você pode usar qualquer ferramenta de cópia baseada em arquivo para migrar os dados para o serviço. Para obter mais informações, confira [Perguntas frequentes sobre migração e proteção de dados para o Azure NetApp Files](https://learn.microsoft.com/pt-br/azure/azure-netapp-files/faq-data-migration-protection).



## Preços

Ao tomar decisões sobre como os dados são armazenados e acessados, você também deve considerar os custos envolvidos. Confira mais informações em [Preços do Armazenamento do Microsoft Azure](https://azure.microsoft.com/pricing/details/storage/).

O serviço de armazenamento de arquivos de nuvem do Azure NetApp Files é cobrado por hora, com base na capacidade provisionada do [pool de capacidade](https://learn.microsoft.com/pt-br/azure/azure-netapp-files/azure-netapp-files-understand-storage-hierarchy#capacity_pools). Para obter mais informações, confira [Preços de armazenamento do Azure NetApp Files](https://azure.microsoft.com/pricing/details/netapp/).



## APIs, bibliotecas e ferramentas de armazenamento

Acesse recursos em uma conta de armazenamento através de qualquer linguagem que possa fazer solicitações HTTP/HTTPS. Além disso, o Armazenamento do Microsoft Azure oferece bibliotecas de programação para várias linguagens populares. Essas bibliotecas simplificam muitos aspectos do trabalho com o Armazenamento do Azure manipulando detalhes, como invocação síncrona e assíncrona, processamento em lotes de operações, gerenciamento de exceções, novas tentativas automáticas, comportamento operacional e assim por diante. Atualmente, as bibliotecas estão disponíveis para as seguintes linguagens e plataformas, com outras no pipeline:



### Bibliotecas de referência e API de dados do Armazenamento do Azure

- [API REST de Armazenamento do Azure](https://learn.microsoft.com/pt-br/rest/api/storageservices/)
- [Bibliotecas de clientes do Armazenamento do Microsoft Azure para .NET](https://learn.microsoft.com/pt-br/dotnet/api/overview/azure/storage)
- [Bibliotecas de clientes do Armazenamento do Microsoft Azure para Java](https://learn.microsoft.com/pt-br/java/api/overview/azure/storage)
- [Bibliotecas de clientes do Armazenamento do Microsoft Azure para JavaScript](https://learn.microsoft.com/pt-br/javascript/api/overview/azure/storage)
- [Bibliotecas de clientes do Armazenamento do Microsoft Azure para Python](https://learn.microsoft.com/pt-br/python/api/overview/azure/storage)
- [Bibliotecas de clientes do Armazenamento do Microsoft Azure para Go](https://github.com/Azure/azure-sdk-for-go/tree/main/sdk/storage/)
- [Bibliotecas de clientes do Armazenamento do Microsoft Azure para C++](https://github.com/Azure/azure-sdk-for-cpp/tree/main/sdk/storage)



### Bibliotecas de referência e API de gerenciamento do Armazenamento do Azure

- [API REST do Provedor de Recursos de Armazenamento](https://learn.microsoft.com/pt-br/rest/api/storagerp/)
- [Biblioteca do Cliente do Provedor de Recursos de Armazenamento para .NET](https://learn.microsoft.com/pt-br/dotnet/api/overview/azure/resourcemanager.storage-readme)
- [API REST do Gerenciamento de Serviços de Armazenamento (clássico)](https://learn.microsoft.com/pt-br/previous-versions/azure/reference/ee460790(v=azure.100))
- [API REST dos Arquivos do Azure](https://learn.microsoft.com/pt-br/rest/api/storageservices/file-service-rest-api)
- [API REST do Azure NetApp Files](https://learn.microsoft.com/pt-br/azure/azure-netapp-files/azure-netapp-files-develop-with-rest-api)



### API de movimentação de dados do armazenamento do Microsoft Azure

- [Biblioteca do Cliente de Movimentação de Dados do Armazenamento para .NET](https://learn.microsoft.com/pt-br/azure/storage/common/storage-use-data-movement-library)



### Ferramentas e utilitários

- [Cmdlets do Azure PowerShell para Armazenamento](https://learn.microsoft.com/pt-br/powershell/module/az.storage)
- [Cmdlets da CLI do Azure para Armazenamento](https://learn.microsoft.com/pt-br/cli/azure/storage)
- [Utilitário de linha de comando AzCopy](https://learn.microsoft.com/pt-br/azure/storage/common/storage-use-azcopy-v10)
- [O Gerenciador de Armazenamento do Azure](https://azure.microsoft.com/features/storage-explorer/) é um aplicativo autônomo e gratuito da Microsoft que possibilita o trabalho visual com os dados do Armazenamento do Azure no Windows, MacOS e Linux.
- [Modelos do ARM para o Armazenamento do Microsoft Azure](https://azure.microsoft.com/resources/templates/?resourceType=Microsoft.Storage)