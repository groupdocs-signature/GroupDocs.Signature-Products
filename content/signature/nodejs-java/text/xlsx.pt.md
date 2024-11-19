



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:14
draft: false
lang: pt
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Adicione assinaturas de texto a XLSX via JavaScript"
head_description: "Utilize a API JavaScript para integrar assinaturas de texto em documentos XLSX de forma simplificada. Nossa API suporta uma ampla gama de formatos, incluindo PDF, Word, Excel, Apresentações, Imagens e arquivos ZIP."

############################# Header ############################
title: "Adicione assinaturas de texto a XLSX" 
description: "Incorpore assinaturas de texto personalizadas nos seus arquivos de negócios com GroupDocs.Signature for Node.js via Java. Assuma o controle dos seus fluxos de trabalho documentais aprimorando-os com opções de assinatura seguras e personalizáveis."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Comece o teste gratuito"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Apresentando GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "Saiba mais"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) é uma solução inovadora projetada para facilitar a adição de assinaturas de texto a documentos. Personalize e coloque assinaturas em qualquer página, melhorando a eficiência no manuseio de documentos. Agilize os fluxos de trabalho da sua organização integrando marcas textuais personalizadas que aprimoram tanto a funcionalidade quanto o profissionalismo.

############################# Steps ############################
steps:
    enable: true
    title: "Guia para criar assinaturas de texto para XLSX usando JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) permite a adição de assinaturas de texto a documentos XLSX dentro de aplicações Node.js via Java. Melhore rapidamente as capacidades do seu produto com nossas soluções robustas.
      
      1. Forneça o documento XLSX como argumento para a classe Signature.
      2. Instancie TextSignOptions com o texto necessário.
      3. Defina as propriedades visuais da assinatura de texto.
      4. Adicione a assinatura de texto às páginas desejadas do documento.
   
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

        // Inicialize a classe Signature com o caminho do documento
        const signature = new signatureLib.Signature('input.xlsx');

        // Crie TextSignOptions com o texto da assinatura desejada
        const options = new signatureLib.TextSignOptions('Approved');

        // Configure a cor do texto e as propriedades da fonte
        options.setForeColor(new signatureLib.Color(255, 0, 0));
        const signatureFont = new signatureLib.SignatureFont();
        signatureFont.setSize(12);
        signatureFont.setFamilyName('Comic Sans MS');
        options.setFont(signatureFont);
        
        // Adicione a assinatura de texto ao documento
        const result = signature.sign('output.xlsx', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Controle aprimorado de assinaturas de texto"
  description: "Com GroupDocs.Signature for Node.js via Java, você pode melhorar significativamente a gestão de assinaturas baseadas em texto em formatos de documento chave. A ferramenta permite configurar o estilo, a colocação e o conteúdo das assinaturas, permitindo que as empresas personalizem seus processos documentais."
  image: "/img/signature/features_text.webp" # 500x500 px
  image_description: "Recursos principais do GroupDocs.Signature"
  features:
    # feature loop
    - title: "Assinaturas dinâmicas em documentos"
      content: "Insira vários tipos de assinaturas—como texto, imagens, códigos de barras, QR codes ou carimbos—em qualquer página de documentos compatíveis. Incorpore metadados para carregar informações ocultas ou aplique certificados digitais para medidas de segurança avançadas."

    # feature loop
    - title: "Busca e validação de assinaturas"
      content: "Verifique a autenticidade das assinaturas incorporadas em seus documentos. Realize buscas eficientes para localizar todas as instâncias de assinatura, garantindo um rastreamento e gerenciamento completos dos documentos."

    # feature loop
    - title: "Editar ou remover assinaturas"
      content: "Modifique ou exclua assinaturas previamente adicionadas conforme necessário. Você pode ajustar a aparência, a posição ou o conteúdo de qualquer assinatura para atender às exigências em evolução, garantindo flexibilidade no manuseio de documentos."

    # feature loop
    - title: "Personalização nativa de assinaturas"
      content: "Para determinados tipos de arquivos, adapte a colocação das assinaturas com recursos de documento integrados, como adicionar marcas d'água em arquivos Word ou carimbos personalizados em PDFs, aprimorando a singularidade dos seus documentos."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Implemente assinaturas de texto em documentos"
      content: |
        Saiba como incorporar assinaturas de texto em documentos de negócios para otimizar processos.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // Escolha o documento a ser assinado
          const signature = new signatureLib.Signature('input.xlsx');

          // Defina as opções de texto com o conteúdo especificado
          const options = new signatureLib.TextSignOptions('Rescheduled to 03/04/2025');

          // Defina o tamanho e a posição da assinatura na página
          options.setLeft(100);
          options.setTop(180);
          options.setWidth(230);
          options.setHeight(30);

          // Aplique preenchimento para a assinatura a partir das bordas da página
          const padding = new signatureLib.Padding();
          padding.setBottom(20);
          padding.setRight(20);
          options.setMargin(padding);

          // Personalize a cor do texto e o estilo da fonte
          options.setForeColor(signatureLib.Color.RED);
          const signatureFont = new signatureLib.SignatureFont();
          signatureFont.setSize(12);
          signatureFont.setFamilyName('Comic Sans MS');
          options.setFont(signatureFont);

          // Adicione uma borda à assinatura de texto, se desejado
          const border = new signatureLib.Border();
          border.setColor(signatureLib.Color.RED);
          border.setDashStyle(signatureLib.DashStyle.Dash);
          border.setTransparency(0.5);
          border.setVisible(true);
          border.setWeight(2);
          options.setBorder(border);

          // Configure o fundo da assinatura
          const background = new signatureLib.Background();
          background.setColor(signatureLib.Color.YELLOW);
          background.setTransparency(0.8);
          options.setBackground(background);

          // Opcionalmente, salve o texto como uma imagem para compatibilidade
          options.setSignatureImplementation(signatureLib.TextSignatureImplementation.Image);
          
          // Salve o documento com a assinatura de texto adicionada
          const result = signature.sign('output.xlsx', options);
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
            link: "/examples/signature/formats/signature_text.xlsx"
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
    title: "Recursos abrangentes de gerenciamento de assinaturas"
    exclude: "text"
    description: "Nossa plataforma oferece operações completas de CRUD e recursos avançados para o gerenciamento de sete tipos distintos de assinatura, permitindo que você gerencie suas assinaturas documentais com precisão."
    items: 
          
        # operation loop 1
        - name: "Assinaturas eletrônicas"
          operation: "esign"
          link: "/signature/nodejs-java/esign/xlsx/"
          description: "Adicionar vários tipos de assinaturas a formatos de arquivo suportados"

        # operation loop 2
        - name: "Adicionar texto a documentos"
          operation: "text"
          link: "/signature/nodejs-java/text/xlsx/"
          description: "Melhore o conteúdo do documento com assinaturas de texto personalizáveis"

        # operation loop 3
        - name: "Assinaturas de imagem"
          operation: "image"
          link: "/signature/nodejs-java/image/xlsx/"
          description: "Colocar qualquer imagem em qualquer posição dentro de um documento"

        # operation loop 4
        - name: "Gerar códigos de barras"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/xlsx/"
          description: "Criar e inserir vários códigos de barras em documentos suportados"

        # operation loop 5
        - name: "Gerar QR codes"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/xlsx/"
          description: "Gerar e QR Codes, incluindo códigos QR, para assinatura de documentos"
          
        # operation loop 6
        - name: "Certificados digitais"
          operation: "digital"
          link: "/signature/nodejs-java/digital/xlsx/"
          description: "Proteger negócios e assinar documentos com certificados digitais"

        # operation loop 7
        - name: "Assinaturas de carimbo"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/xlsx/"
          description: "Use o Construtor de Carimbos para criar carimbos redondos ou quadrados personalizados"
          
        # operation loop 8
        - name: "Buscar assinaturas"
          operation: "search"
          link: "/signature/nodejs-java/search/xlsx/"
          description: "Localizar quaisquer assinaturas previamente adicionadas em um documento"
          
        # operation loop 9
        - name: "Verificação de assinaturas"
          operation: "verify"
          link: "/signature/nodejs-java/verify/xlsx/"
          description: "Verificar a autenticidade das assinaturas após a aplicação"
          
        # operation loop 10
        - name: "Modificar assinaturas"
          operation: "modify"
          link: "/signature/nodejs-java/modify/xlsx/"
          description: "Editar uma variedade de assinaturas dentro de um documento"
          
        # operation loop 11
        - name: "Excluir assinaturas"
          operation: "delete"
          link: "/signature/nodejs-java/delete/xlsx/"
          description: "Remover uma ampla gama de assinaturas previamente aplicadas"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Aplique assinaturas de texto em vários formatos"
    exclude: "XLSX"
    description: "Aproveite as capacidades da API Node.js via Java para integrar assinaturas baseadas em texto em uma ampla variedade de formatos do Office. Controle o fluxo de informações em cada estágio do ciclo de vida do seu documento ao adicionar marcas de texto altamente personalizáveis."
    items: 
          
        # format loop 1
        - name: "Assinaturas de texto em PDF"
          format: "PDF"
          link: "/signature/nodejs-java/text/pdf/"
          description: "Formato de Documento Portátil Adobe"
          
        # format loop 2
        - name: "Assinaturas de texto em DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/text/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 3
        - name: "Assinaturas de texto em JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/text/jpeg/"
          description: "Imagem JPEG"
          
        # format loop 4
        - name: "Assinaturas de texto em PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/text/pptx/"
          description: "Apresentação PowerPoint Open XML"
          
        # format loop 5
        - name: "Assinaturas de texto em XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/text/xlsx/"
          description: "Planilha Microsoft Excel Open XML"


          

---