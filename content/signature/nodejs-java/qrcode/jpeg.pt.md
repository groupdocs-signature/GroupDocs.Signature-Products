



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:22
draft: false
lang: pt
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Gerar códigos QR em documentos JPEG com JavaScript"
head_description: "Utilize a API GroupDocs.Signature para criar e integrar códigos de barras 2D em arquivos JPEG. Insira códigos QR em qualquer página do documento."

############################# Header ############################
title: "Crie códigos QR para JPEG" 
description: "Crie e insira códigos de barras 2D com conteúdo personalizável, incluindo texto e dados numéricos, em vários tipos de documentos, como PDFs, Word, Excel e Imagens com GroupDocs.Signature for Node.js via Java."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Experimente Gratuitamente"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Explore as capacidades do GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "Saiba mais"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) oferece ferramentas avançadas para aprimorar documentos, permitindo a geração e a inclusão de múltiplos tipos de assinatura, incluindo códigos QR, em formatos de arquivo populares. Assine e proteja PDFs, documentos Word, planilhas Excel, apresentações PowerPoint e imagens com assinaturas de Texto, Imagem, Código de Barras, Código QR, Metadados, Digital e Carimbo.

############################# Steps ############################
steps:
    enable: true
    title: "Guia para gerar e incorporar um código QR em qualquer lugar dentro de um JPEG"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) permite a criação de códigos QR em vários formatos amplamente utilizados e sua integração em páginas JPEG. Com suporte a mais de 10 tipos distintos de códigos QR, nossa solução pode ser incorporada perfeitamente em aplicativos Node.js via Java, enriquecendo-os com capacidades de assinatura de códigos QR.
      
      1. Forneça o arquivo JPEG ou stream para a assinatura do código QR.
      2. Insira o texto desejado na instância de QrCodeSignOptions.
      3. Ajuste as configurações visuais, como cor, posicionamento, tamanho, etc.
      4. Salve o documento contendo o código QR.
   
    code:
      platform: "nodejs-java"
      copy_title: "Copiar"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Assinaturas de exemplo"
      install:
        command: "npm i @groupdocs/groupdocs.signature"
        copy_tip: "clique para copiar"
        copy_done: "copiado"
      links:
        #  loop
        - title: "Mais exemplos"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
        #  loop
        - title: "Documentação"
          link: "https://docs.groupdocs.com/signature/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')

        // Crie uma instância de Signature e passe o caminho do documento
        const signature = new signatureLib.Signature('input.jpeg');

        // Utilize QrCodeSignOptions para inserir um código QR no documento
        // Create QR code sign options
        const options = new signatureLib.QrCodeSignOptions('Text Content');

        // Defina o tipo de assinatura e a colocação na página
        options.setEncodeType(signatureLib.QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);
  
        // Armazene o documento com o novo código QR adicionado
        signature.sign('output.jpeg', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Integração abrangente de assinatura e código QR"
  description: "Com a API GroupDocs.Signature for Node.js via Java, você pode gerenciar uma ampla gama de assinaturas. Gere, personaliza, valide, busque e remova assinaturas de maneira simples em diferentes tipos de documentos, oferecendo flexibilidade incomparável para seus fluxos de trabalho."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "Recursos de assinatura e código QR"
  features:
    # feature loop
    - title: "Assinatura de documentos em múltiplos formatos"
      content: "Adicione vários tipos de assinaturas, incluindo Texto, Imagem, Código de Barras, Código QR e assinaturas de Carimbo, a qualquer formato de documento suportado. Coloque-os em qualquer página e gerencie os metadados do documento. Garanta a segurança do documento através de certificados digitais para impedir alterações não autorizadas."

    # feature loop
    - title: "Validação eficiente de assinaturas"
      content: "Valide todas as assinaturas dentro de um documento para garantir que atendam aos padrões exigidos. Recupere e revise facilmente as assinaturas através da funcionalidade de busca integrada."

    # feature loop
    - title: "Edição flexível de assinaturas"
      content: "Atualize ou modifique assinaturas existentes, ajustando aspectos como conteúdo, localização, tamanho e cor, para atender às necessidades do seu documento após a assinatura inicial."

    # feature loop
    - title: "Remoção de assinaturas simplificada"
      content: "Remova quaisquer assinaturas indesejadas ou obsoletas, incluindo certificados digitais, com facilidade. O controle total sobre o gerenciamento de assinaturas garante um documento limpo e bem organizado."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Personalizando um código QR gerado"
      content: |
        Este exemplo detalha o processo de adicionar um código QR personalizado a uma página JPEG.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // Obtenha o documento a ser assinado e passe-o para Signature
          const signature = new signatureLib.Signature('input.jpeg');

          // Configure as opções do código QR com o texto necessário
          const signOptions = new signatureLib.QrCodeSignOptions('Archived on July 11, 2019');

          // Determine a posição do código QR na página
          signOptions.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          signOptions.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);

          // Especifique o espaçamento da assinatura
          const padding = new signatureLib.Padding();
          padding.setRight(20);
          padding.setTop(20);
          signOptions.setMargin(padding);

          // Escolha a cor do código QR
          signOptions.setForeColor(signatureLib.Color.RED);

          // Defina as opções de fonte para a mensagem acompanhante
          const font = new signatureLib.SignatureFont();
          font.setSize(12);
          font.setFamilyName("Comic Sans MS");
          signOptions.setFont(font);

          // Personalize a cor de fundo e o pincel para o código QR
          const background = new signatureLib.Background();
          background.setColor(signatureLib.Color.GREEN);
          background.setTransparency(0.5);
          background.setBrush(new signatureLib.LinearGradientBrush(signatureLib.Color.GREEN, signatureLib.Color.DARK_GRAY, 0));
          signOptions.setBackground(background);

          // Implemente o código QR no documento
          signature.sign('output.jpeg', signOptions);
          ```
        platform: "nodejs-java"
        copy_title: "Copiar"
        install:
          command: "npm i @groupdocs/groupdocs.signature"
          copy_tip: "clique para copiar"
          copy_done: "copiado"
        top_links:
          #  loop
          - title: "Baixar resultado"
            icon: "download"
            link: "/examples/signature/formats/signature_qrcode.jpeg"
        links:
          #  loop
          - title: "Mais exemplos"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
          #  loop
          - title: "Documentação"
            link: "https://docs.groupdocs.com/signature/nodejs-java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Pronto para começar?"
  description: "Experimente os recursos do GroupDocs.Signature gratuitamente ou solicite uma licença"
  items:
    #  loop
    - title: "Baixar NPM"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      color: "red"
        #  loop
    - title: "Licenciamento"
      link: "https://purchase.groupdocs.com/pricing/signature/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Entenda nossas principais capacidades"
    exclude: "qrcode"
    description: "Oferecemos uma ampla seleção de formatos de assinatura e operações adaptadas às suas necessidades."
    items: 
          
        # operation loop 1
        - name: "Assinaturas eletrônicas"
          operation: "esign"
          link: "/signature/nodejs-java/esign/jpeg/"
          description: "Adicionar vários tipos de assinaturas a formatos de arquivo suportados"

        # operation loop 2
        - name: "Adicionar texto a documentos"
          operation: "text"
          link: "/signature/nodejs-java/text/jpeg/"
          description: "Melhore o conteúdo do documento com assinaturas de texto personalizáveis"

        # operation loop 3
        - name: "Assinaturas de imagem"
          operation: "image"
          link: "/signature/nodejs-java/image/jpeg/"
          description: "Colocar qualquer imagem em qualquer posição dentro de um documento"

        # operation loop 4
        - name: "Gerar códigos de barras"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/jpeg/"
          description: "Criar e inserir vários códigos de barras em documentos suportados"

        # operation loop 5
        - name: "Gerar QR codes"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/jpeg/"
          description: "Gerar e QR Codes, incluindo códigos QR, para assinatura de documentos"
          
        # operation loop 6
        - name: "Certificados digitais"
          operation: "digital"
          link: "/signature/nodejs-java/digital/pdf/"
          description: "Proteger negócios e assinar documentos com certificados digitais"

        # operation loop 7
        - name: "Assinaturas de carimbo"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/jpeg/"
          description: "Use o Construtor de Carimbos para criar carimbos redondos ou quadrados personalizados"
          
        # operation loop 8
        - name: "Buscar assinaturas"
          operation: "search"
          link: "/signature/nodejs-java/search/pdf/"
          description: "Localizar quaisquer assinaturas previamente adicionadas em um documento"
          
        # operation loop 9
        - name: "Verificação de assinaturas"
          operation: "verify"
          link: "/signature/nodejs-java/verify/pdf/"
          description: "Verificar a autenticidade das assinaturas após a aplicação"
          
        # operation loop 10
        - name: "Modificar assinaturas"
          operation: "modify"
          link: "/signature/nodejs-java/modify/pdf/"
          description: "Editar uma variedade de assinaturas dentro de um documento"
          
        # operation loop 11
        - name: "Excluir assinaturas"
          operation: "delete"
          link: "/signature/nodejs-java/delete/pdf/"
          description: "Remover uma ampla gama de assinaturas previamente aplicadas"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Integre códigos QR com vários formatos de arquivo"
    exclude: "JPEG"
    description: "Aproveite a API Node.js via Java para gerar códigos QR e incorporá-los em uma variedade de formatos de arquivo amplamente utilizados. Encapsule dados importantes nesses códigos de barras para integração fluida e recuperação futura."
    items: 
          
        # format loop 1
        - name: "QR-Code para PDF"
          format: "PDF"
          link: "/signature/nodejs-java/qrcode/pdf/"
          description: "Formato de Documento Portátil Adobe"
          
        # format loop 2
        - name: "QR-Code para DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/qrcode/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 3
        - name: "QR-Code para JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/qrcode/jpeg/"
          description: "Imagem JPEG"
          
        # format loop 4
        - name: "QR-Code para PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/qrcode/pptx/"
          description: "Apresentação PowerPoint Open XML"
          
        # format loop 5
        - name: "QR-Code para XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/qrcode/xlsx/"
          description: "Planilha Microsoft Excel Open XML"


          

---