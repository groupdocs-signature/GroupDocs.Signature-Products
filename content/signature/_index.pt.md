---
############################# Static ############################
layout: "family"
date:  2024-09-26T13:44:48
draft: false

product: "Signature"
product_tag: "signature"

lang: pt

############################# Head ############################
head_title: "Aplicativos de assinatura digital C# .NET, Java, Node.js"
head_description: "Integre assinaturas eletrônicas em aplicativos .NET, Java ou Node.js com GroupDocs.Signature. Assine formatos de documentos comerciais populares."

############################# Header ############################
title: "Solução de assinatura eletrônica de documentos"
description:  |
  Assine documentos e imagens digitais em qualquer plataforma usando nossas APIs flexíveis e soluções baseadas em aplicativos para programadores e usuários finais.

  Pesquise e modifique assinaturas adicionadas anteriormente usando métodos avançados.

  Proteja documentos contra alterações com certificados digitais e controle metadados ocultos.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "Escolha sua plataforma"
  title: "Independência de plataforma"
  description: "A biblioteca GroupDocs.Signature oferece suporte aos seguintes sistemas operacionais e estruturas:"
  details_link_title: "Saber mais"

  items:
    # items loop
    - title: ".NET"
      description: GroupDocs.Signature .NET 
      color: "blue"
      tag: "net"
      link: "/signature/net/"
      features_link: "https://docs.groupdocs.com/signature/net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    .NET Framework 4.6.2 or higher <br> .NET Core 3.0 or higher <br> .NET 6.0 or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS <br> Microsoft Azure
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio <br> JetBrains Rider <br> Microsoft Visual Code
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats
      

    # items loop
    - title: "Java"
      description: GroupDocs.Signature Java
      color: "red"
      tag: "java"
      link: "/signature/java/"
      features_link: "https://docs.groupdocs.com/signature/java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Java 8 or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    IntelliJ IDEA <br> Eclipse <br> NetBeans
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats

    # items loop
    - title: "Node.js"
      description: GroupDocs.Signature Node.js
      color: "green"
      tag: "nodejs-java"
      link: "/signature/nodejs-java/"
      features_link: "https://docs.groupdocs.com/signature/nodejs-java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Node.js 16+ and J2SE 8.0 (1.8)+
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Atom <br> Visual Studio Code <br> Qualquer outro editor de texto
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats

    # items loop
    - title: "Python"
      description: GroupDocs.Signature Python
      color: "yellow"
      tag: "python-net"
      link: "/signature/python-net/"
      features_link: "https://docs.groupdocs.com/signature/python-net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Python 3.9+ and .Net 6+
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    IDLE <br> PyCharm <br> Visual Studio Code
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats

############################# Features ###############################
features:
  enable: true
  title: "Principais recursos do GroupDocs.Signature"
  description: "Nossa solução foi projetada para adicionar vários tipos de assinaturas a formatos populares de documentos e arquivos. Enriqueça seus processos de negócios facilmente."

  items:
    # items loop
    - icon: "additional"
      title: "Enriqueça seus dados com assinaturas"
      content: "Anexe texto, imagens, marcas d'água, etc. aos seus documentos comerciais."

    # items loop
    - icon: "protect"
      title: "Proteja o conteúdo dos documentos"
      content: "Proíba alterações de documentos selando-os com um certificado digital."

    # items loop
    - icon: "search"
      title: "Adicione dados e códigos de barras ocultos"
      content: "Use metadados para armazenar informações invisíveis ou coloque códigos de barras personalizados nas páginas."

    # items loop
    - icon: "manipulate"
      title: "Manipular assinaturas"
      content: "Pesquise, atualize ou exclua todas as assinaturas que foram adicionadas anteriormente."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Proteja seus arquivos usando assinaturas"
  description: "Exemplos de código GroupDocs.Signature"
  items:
    # code sample loop
    - title: "Gere e adicione código QR"
      content: |
       GroupDocs.Signature nos permite gerar e adicionar códigos QR a documentos com formatos suportados. Forneça o caminho para um documento que deve ser assinado e configure o texto desejado e as opções visuais do código QR. Você pode colocar a imagem do código QR gerada em qualquer área de qualquer página do documento.
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // Especifique o documento para assinatura
            using (Signature signature = new Signature("source.docx"))
            {
                // Crie opções de sinal de código QR
                QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith")
                {
                    // Definir opções de código QR
                    EncodeType = QrCodeTypes.QR,
                    Left = 50,
                    Top = 150,
                };

                // Assine e salve o arquivo processado
                SignResult result = signature.Sign("result.docx", options);
            }
            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // Especifique o documento para assinatura
            Signature signature = new Signature("source.docx");

            // Crie opções de sinal de código QR
            QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith");

            // Definir opções de código QR
            options.setEncodeType(QrCodeTypes.QR);
            options.setLeft(50);
            options.setTop(100);

            // Assine e salve o arquivo processado
            signature.sign("result.docx", options);
            ```
        - language: "TypeScript"
          color: "green"
          content: |
            ```javascript {style=abap}  
            const signatureLib = require('@groupdocs/groupdocs.signature')

            // Especifique o documento para assinatura
            const signature = new signatureLib.Signature('source.docx');

            // Crie opções de sinal de código QR
            const options = new signatureLib.QrCodeSignOptions('JohnSmith');

            // Definir opções de código QR
            options.setEncodeType(signatureLib.QrCodeTypes.QR);
            options.setLeft(50);
            options.setTop(100);

            // Assine e salve o arquivo processado
            signature.sign('result.docx', options);
            ```
        - language: "Python"
          color: "yellow"
          content: |
            ```python {style=abap}  
            import groupdocs.signature as sg

            def run():

                # Especifique o documento para assinatura
                with sg.Signature('source.docx') as signature:

                    # Crie opções de sinal de código QR
                    options = sg.QrCodeSignOptions('JohnSmith')

                    # Definir opções de código QR
                    options.setEncodeType(sg.QrCodeTypes.QR)
                    options.setLeft(50)
                    options.setTop(100)

                    # Assine e salve o arquivo processado
                    signature.sign('result.docx', options)
            ```

############################# Supported Formats ###############################
formats:
  enable: true
  title: "Mais de 60 formatos de arquivo são suportados"
  description: "GroupDocs.Signature suporta quase todos os formatos de arquivo populares"

############################# Metrics ###############################
metrics:
  enable: true
  title: "Dados estatísticos da nossa biblioteca"
  description: "Inspecione as principais métricas do produto, revelando insights sobre nossas conquistas, impacto e crescimento"

  items:
    # items loop
    - number: "50+"
      title: "Formatos suportados"
      content: "Assinando mais de 60 dos formatos de arquivo comerciais mais populares."

    # items loop
    - number: "500k"
      title: "Downloads do NuGet"
      content: "GroupDocs.Signature for .NET é uma biblioteca popular com mais de 550.000 downloads no NuGet."

    # items loop
    - number: "15k"
      title: "Downloads do Maven"
      content: "Os desenvolvedores Java baixaram GroupDocs.Signature no Maven mais de 15 mil vezes."

    # items loop
    - number: "140+"
      title: "Clientes satisfeitos"
      content: "Desenvolvedores individuais e grandes empresas em todo o mundo utilizam nossos produtos para criar soluções inovadoras."


############################# Customers ###############################
customers:
  enable: true
  title: "Nossos clientes satisfeitos"
  description: "As bibliotecas GroupDocs são empregadas por marcas renomadas e distintas em todo o mundo"

  items:
    # items loop
    - title: "BenQ Corporation"
      logo: "benq"
      
    # items loop
    - title: "Nasdaq Stock Market"
      logo: "nasdaq"
      
    # items loop
    - title: "AT&T Inc."
      logo: "att"
      
    # items loop
    - title: "Customer logo AstraZeneca"
      logo: "astrazeneca"
      
    # items loop
    - title: "Central Bank of Argentina"
      logo: "argentinacentralbank"
      
    # items loop
    - title: "Roche Holding AG"
      logo: "roche"
      
    # items loop
    - title: "Capita"
      logo: "capita"
      
    # items loop
    - title: "Axa S.A."
      logo: "axa"
      
    # items loop
    - title: "Instructure Inc."
      logo: "instructure"
      
    # items loop
    - title: "Wipro"
      logo: "wipro"


############################# Actions ###############################
actions:
  enable: true
  title: "Pronto para começar?"
  description: "Experimente os recursos do GroupDocs.Signature gratuitamente em sua plataforma"

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/signature/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/signature/java/"

    # items loop
    - title: "Node.js"
      color: "green"
      link: "/signature/nodejs-java/"      

############################# FAQ ###############################
faq:
  enable: true
  title: "Perguntas frequentes"
  description: "Explore nossas perguntas frequentes"

  items:
    # items loop
    - question: "GroupDocs.Signature precisa de alguma biblioteca externa para assinatura de documentos?"
      answer: "Não, GroupDocs.Signature funciona de forma independente. Não há dependências de terceiros como Adobe Acrobat, Microsoft Office, etc."

    # items loop
    - question: "É possível testar os recursos do GroupDocs.Signature antes de comprar?"
      answer: "Absolutamente! GroupDocs.Signature oferece um teste gratuito. Instale-o e explore seus recursos. Observe que as versões de teste adicionam 'crachás de teste' aos seus documentos e processam apenas as três primeiras páginas. Para uma experiência completa, obtenha uma licença temporária gratuita de 30 dias para acessar todas as funcionalidades. Veja detalhes em [licença temporária](https://purchase.groupdocs.com/temporary-license/)."

    # items loop
    - question: "Que tipos de licença são fornecidos?"
      answer: "Procurando uma licença do GroupDocs.Signature? Oferecemos diversas opções adaptadas às suas necessidades. Escolha com base no tamanho da equipe, nos locais de implantação (escritório único ou locais de trabalho remotos) e se a distribuição para o cliente final exige o compartilhamento do SDK/API com os clientes. Alternativamente, opte por uma licença de uso mensal com planos medidos – pague apenas pelo que usar. Descubra a melhor opção para você em [pricing](https://purchase.groupdocs.com/pricing/signature/net/)."

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "GroupDocs.Signature APIs de baixo código"
  description: "Assine arquivos usando seu aplicativo por meio de nossa API REST baseada em nuvem."
  
  items:
    # items loop
    - title: "GroupDocs.Signature Cloud for cURL"
      content: "Use a API RESTful cURL para colocar assinaturas em PDF, Word, Excel, PowerPoint, JPEG e muitos outros formatos de arquivo."
      icon: "groupdocs_signature-for-curl"
      link: "https://products.groupdocs.cloud/signature/curl"

    # items loop
    - title: "GroupDocs.Signature Cloud for .NET"
      content: "Enriqueça seus aplicativos .NET com assinatura de documentos via Cloud SDK. Proteja documentos comerciais do seu jeito."
      icon: "groupdocs_signature-for-net"
      link: "https://products.groupdocs.cloud/signature/net"

    # items loop
    - title: "GroupDocs.Signature Cloud for Java"
      content: "GroupDocs.Signature SDK concede acesso a várias possibilidades para seus aplicativos Java assinarem qualquer arquivo."
      icon: "groupdocs_signature-for-java"
      link: "https://products.groupdocs.cloud/signature/java"

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Signature aplicativos da web"
  description: "GroupDocs.Signature apresenta um aplicativo web gratuito onde você pode assinar documentos. Mais de 60 formatos de arquivo populares podem ser assinados GRATUITAMENTE através do seu navegador favorito."

  items:
    # items loop
    - title: "GroupDocs.Signature Total"
      content: "Ferramenta online para colocar assinaturas em documentos de qualquer dispositivo."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/signature/total"

    # items loop
    - title: "GroupDocs.Signature DOCX"
      content: "Assine o MS Word DOCX online."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/signature/docx"

    # items loop
    - title: "GroupDocs.Signature PDF"
      content: "Proteja documentos PDF online."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/signature/pdf"


      


---