Resumo - IAM
O AWS Identity and Access Management (IAM) é um serviço da AWS que ajuda a controlar quem está autenticado (assinado) e autorizado (tem permissões) para usar os recursos da AWS.

Aqui estão os principais pontos sobre o IAM:



Controle Granular de Acesso a AWS: Com o IAM, você pode criar usuários, grupos, papéis e políticas de permissão para controlar o acesso aos serviços e recursos da AWS de uma maneira granular. Por exemplo, você pode permitir que um usuário tenha acesso somente leitura ao Amazon S3 e acesso total ao EC2.

Compartilhamento Seguro de Acesso: O IAM permite compartilhar o acesso à sua conta AWS de maneira segura. Em vez de compartilhar suas credenciais de root, você pode criar vários usuários IAM, cada um com suas próprias credenciais e permissões.

Identidade Federada: Com o IAM, você também pode permitir usuários que já tenham senhas em outros lugares, como na sua rede corporativa ou em um provedor de identidade baseado em SAML, a obter acesso temporário à sua conta AWS.

Compatível com Multi-Fator Authentication (MFA): O IAM é compatível com a autenticação de vários fatores para fornecer uma camada adicional de proteção de segurança ao gerenciar o acesso aos serviços e recursos da AWS.

Integrado com AWS Services: O IAM está integrado com todos os serviços da AWS, o que significa que você pode definir permissões para qualquer serviço que desejar.

Auditoria com AWS CloudTrail: Com o AWS CloudTrail, você pode registrar todas as ações de usuários e APIs IAM para fins de auditoria.

Gratuito: O IAM é um recurso gratuito da AWS; você só paga pelos outros recursos da AWS que seus usuários acessam.

Em suma, o AWS IAM é um serviço de segurança crítico que ajuda a proteger o acesso aos recursos da AWS, permitindo que você controle quem pode fazer o quê em sua conta AWS.

Resumo - MFA
A Autenticação Multifator (MFA) é um método de controle de acesso que exige que um usuário verifique sua identidade usando duas ou mais evidências (fatores) antes que o acesso seja concedido. Estes fatores podem ser algo que o usuário sabe (como uma senha), algo que o usuário tem (como um telefone celular ou um token de hardware) e algo que o usuário é (como uma impressão digital ou reconhecimento facial).

Aqui estão alguns pontos-chave sobre MFA:



Segurança Aprimorada: O principal benefício da MFA é que ela aumenta significativamente a segurança, tornando muito mais difícil para os invasores ganharem acesso não autorizado a um sistema. Mesmo que um fator de autenticação seja comprometido (por exemplo, se uma senha for roubada), os outros fatores ainda protegem o sistema.

Diversos Métodos de Autenticação: A MFA pode usar uma variedade de métodos de autenticação, como códigos de verificação por SMS, aplicativos de autenticação, tokens de hardware, impressões digitais, reconhecimento facial e muito mais.

Compatibilidade: A MFA é compatível com muitos sistemas e serviços, incluindo a maioria das plataformas de nuvem (como AWS, Google Cloud e Azure), serviços de email, redes sociais, plataformas de pagamento online, entre outros.

AWS MFA: A AWS suporta MFA e recomenda que os usuários a utilizem para proteger suas contas. Com a MFA ativada, quando um usuário se conecta à AWS, ele é solicitado a inserir seu nome de usuário e senha (primeiro fator) e um código de autenticação de um dispositivo MFA (segundo fator).

Resumindo, a Autenticação Multifator é uma medida de segurança essencial que protege os sistemas de acesso não autorizado, exigindo que os usuários verifiquem sua identidade com vários fatores de autenticação.


Resumo - Organizações
O AWS Organizations é um serviço da AWS que permite a você centralizar e gerenciar de forma unificada várias contas AWS. Com o AWS Organizations, você pode criar uma organização para administrar suas contas da AWS a partir de um único local.

Aqui estão algumas características principais do AWS Organizations:



Gerenciamento Centralizado de Contas: O AWS Organizations permite agrupar e gerenciar todas as suas contas AWS de um único local centralizado. Isso facilita o gerenciamento de contas e recursos em uma organização.

Controle de Acesso Hierárquico: Com o AWS Organizations, você pode criar uma estrutura hierárquica de Unidades Organizacionais (OUs) para agrupar suas contas. Isso ajuda a organizar suas contas em uma estrutura que melhor se alinhe com o uso dos recursos em sua organização.

Políticas de Controle de Serviço: O AWS Organizations oferece políticas de controle de serviço (SCPs) que permitem que você controle as permissões para as contas em sua organização. Isso permite que você aplique regras de acesso uniformes em todas as suas contas.

Consolidação de Cobrança: O AWS Organizations também oferece a capacidade de consolidar sua cobrança em todas as suas contas AWS, o que pode simplificar a gestão de custos e permitir um melhor rastreamento e controle dos gastos da AWS.

Automação: Com o AWS Organizations, você pode automatizar a criação e o gerenciamento de contas por meio de APIs e integrações com outras ferramentas da AWS, como o AWS CloudFormation.

Em suma, o AWS Organizations é uma ferramenta poderosa para empresas e equipes que gerenciam várias contas da AWS, permitindo o gerenciamento centralizado de contas, a aplicação de políticas em todas as contas, a consolidação de cobranças e a automação de tarefas de gerenciamento de contas.

Resumo - Infra Global
A infraestrutura global da AWS é a base sobre a qual os serviços da AWS são construídos. Ela consiste em uma série de Regiões e Zonas de Disponibilidade espalhadas pelo mundo, projetadas para fornecer um serviço seguro, confiável e escalável.

Regiões: Uma região da AWS é uma área geográfica que contém pelo menos duas Zonas de Disponibilidade. Cada região é completamente independente das outras regiões, o que ajuda a isolar falhas e evitar a propagação de problemas de uma região para outra. Em setembro de 2021, a AWS tinha 25 regiões geográficas ao redor do mundo.

Zonas de Disponibilidade (AZs): Cada região da AWS é dividida em Zonas de Disponibilidade. Cada AZ é um centro de dados separado dentro de uma região, mas todas as AZs dentro de uma região estão conectadas através de redes de alta velocidade, de baixa latência e totalmente redundantes. As AZs fornecem uma maneira de construir aplicativos altamente disponíveis e tolerantes a falhas.

Zonas Locais: As zonas locais da AWS aproximam a computação, o armazenamento, o banco de dados e outros produtos da AWS selecionados dos usuários finais. Com as zonas locais da AWS, você pode executar facilmente aplicativos altamente exigentes que exigem latências em milissegundos de um dígito para seus usuários finais, como criação de conteúdo de mídia e entretenimento, jogos em tempo real, simulações de reservatórios, automação de projetos eletrônicos e machine learning.

Wavelenght: O AWS Wavelength permite que os desenvolvedores criem aplicações com latências de um dígito para dispositivos móveis e usuários finais. Os desenvolvedores da AWS podem implantar seus aplicativos nas Zonas do Wavelength, implantações de infraestrutura da AWS que incorporam serviços de computação e armazenamento da AWS aos datacenters dos provedores de telecomunicações na borda das redes 5G e acessam facilmente a variedade de serviços da AWS na região. Isso permite que os desenvolvedores forneçam aplicativos que exigem latências inferiores a 10 milissegundos, como streaming de jogos e vídeos ao vivo, inferência de machine learning na borda e realidade aumentada e virtual (AR/VR).

OutPosts: O AWS Outposts leva produtos, infraestrutura e modelos operacionais nativos da AWS a praticamente qualquer datacenter, espaço de colocalização ou instalações on-premises. Você pode usar as mesmas APIs, ferramentas e infraestrutura da AWS no local e na Nuvem AWS para oferecer uma experiência híbrida verdadeiramente consistente. O AWS Outposts foi projetado para ambientes conectados e pode ser usado para oferecer suporte a workloads que precisam permanecer on-premises devido à baixa latência ou às necessidades de processamento de dados locais.

A infraestrutura global da AWS permite que os usuários implantem seus aplicativos e serviços de maneira flexível, resiliente e eficiente em termos de latência, onde quer que seus clientes estejam localizados no mundo. Isso significa que, como usuário da AWS, você pode oferecer uma experiência de usuário mais rápida e melhor para seus clientes, independentemente de sua localização geográfica.

Resumo - Share Model
O Modelo de Responsabilidade Compartilhada da AWS é uma estrutura de governança que delineia a divisão de responsabilidades de segurança entre a Amazon Web Services (AWS) e o usuário (cliente). Essa divisão de responsabilidades permite que a AWS se concentre na segurança da infraestrutura de computação em nuvem, enquanto o usuário se concentra na segurança dos dados e recursos que colocam na nuvem.

Aqui está uma visão geral das responsabilidades compartilhadas:



Segurança "da" nuvem: A AWS é responsável pela proteção da infraestrutura que executa todos os serviços oferecidos na AWS Cloud. Isso inclui hardware, software, redes e instalações que sustentam os serviços AWS Cloud.

Segurança "na" nuvem: O cliente é responsável pela segurança de qualquer coisa que coloque "na" nuvem ou conecte "à" nuvem. Isso pode incluir a configuração correta de controles de segurança e conformidade em serviços da AWS, gerenciamento de dados (incluindo criptografia e backups), classificação de ativos e outras várias tarefas de segurança de TI.

Serviços de Infraestrutura, Contêiner e Abstração: Dependendo do tipo de serviço da AWS que está sendo usado (por exemplo, uma instância EC2 versus um banco de dados RDS), a AWS e o cliente compartilharão diferentes partes da responsabilidade de segurança. Por exemplo, para um serviço de infraestrutura como o EC2, a AWS fornece a segurança física, a do hypervisor e a da rede, enquanto o cliente é responsável pelo sistema operacional e pelas aplicações. Para um serviço de contêiner como o RDS, a AWS também é responsável pela segurança do sistema operacional e do serviço de banco de dados, enquanto o cliente ainda é responsável pelas aplicações e dados.

A compreensão e a aplicação adequada do Modelo de Responsabilidade Compartilhada da AWS são fundamentais para garantir a segurança e a conformidade ao usar a AWS. Isso requer que os clientes estejam cientes de suas responsabilidades de segurança e implementem práticas de segurança robustas ao usar serviços da AWS.


Resumo - EC2
O Amazon Elastic Compute Cloud (EC2) é um componente central da plataforma de computação em nuvem da Amazon. O EC2 permite aos usuários alugar máquinas virtuais usando a infraestrutura da Amazon. Ele foi projetado para tornar a computação em escala na web mais acessível para os desenvolvedores.

Aqui estão alguns pontos-chave sobre o Amazon EC2:



Máquinas Virtuais: EC2 fornece instâncias, que são máquinas virtuais executando os sistemas operacionais que você escolher.

Escalabilidade: Você pode dimensionar a capacidade de computação facilmente, criando e lançando novas instâncias conforme necessário, o que é útil para lidar com picos de demanda e escala.

Controle Completo: Os usuários têm controle total sobre as instâncias do EC2. Eles têm acesso de root, e podem interagir com elas como fariam com qualquer máquina.

Várias Regiões e Zonas de Disponibilidade: As instâncias do EC2 podem ser implantadas em várias regiões geográficas e zonas de disponibilidade. Isso ajuda a reduzir latência, aumentar a tolerância a falhas e cumprir os requisitos de residência de dados.

Modelos de Instância: O EC2 fornece uma variedade de tipos de instâncias otimizadas para diferentes casos de uso, garantindo que você tenha os recursos de que precisa para o aplicativo que está executando.

Preços Flexíveis: O EC2 oferece várias opções de preços, incluindo On-Demand (pague pelo que usar), Reservado (reserve uma instância por um período e obtenha um desconto) e Spot (licitação por capacidade não utilizada a preços mais baixos).

Armazenamento Integrado: As instâncias do EC2 podem ser integradas com outros serviços da AWS para fornecer armazenamento (por exemplo, Amazon EBS), bancos de dados (por exemplo, Amazon RDS), e redes (por exemplo, Amazon VPC).

Segurança: O EC2 trabalha com o Amazon VPC para fornecer segurança e robustez por meio de grupos de segurança e redes isoladas.

Em resumo, o Amazon EC2 é um serviço poderoso e flexível que forma a espinha dorsal da computação na plataforma AWS, permitindo que as empresas executem e dimensionem aplicativos na nuvem de forma eficiente e segura.
