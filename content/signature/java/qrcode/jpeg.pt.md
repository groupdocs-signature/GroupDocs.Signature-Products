



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:20
draft: false
lang: pt
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Crie código QR para JPEG com Java"
head_description: "A API GroupDocs.Signature permite a geração de códigos QR para arquivos JPEG. Crie códigos QR a partir do seu conteúdo e insira-os em qualquer página."

############################# Header ############################
title: "Crie códigos QR para JPEG" 
description: "Crie códigos de barras 2D com dados de texto e numéricos e coloque-os em qualquer página de diversos documentos usando GroupDocs.Signature for Java."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Teste gratuito"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "Saiba mais sobre GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "Saiba mais"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) oferece uma ampla gama de recursos para gerar e inserir vários tipos de assinaturas em todos os principais formatos de documentos. Suporta PDFs, documentos do Word, planilhas do Excel, apresentações do PowerPoint e imagens. Aprimore seus documentos com assinaturas de Texto, Imagem, Código de Barras, QR Code, Metadados, Digital e Carimbo.

############################# Steps ############################
steps:
    enable: true
    title: "Passos para gerar e colocar um código QR em qualquer localização em um JPEG"
    content: |
      [GroupDocs.Signature](/signature/java/) pode gerar códigos QR em muitos formatos populares e inseri-los nas páginas de JPEG. Mais de 10 tipos de códigos QR são suportados e podem ser rapidamente integrados em aplicações Java. Use nosso produto para assinar documentos com códigos QR gerados.
      
      1. Obtenha o arquivo ou stream JPEG a ser assinado com um código QR.
      2. Forneça o texto para QrCodeSignOptions.
      3. Personalize opções visuais, como cor, posição, tamanho, etc.
      4. Salve o arquivo com o código QR.
   
    code:
      platform: "java"
      copy_title: "Copiar"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Assinaturas de exemplo"
      install:
        command_title: "Maven XML"
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-signature</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "clique para copiar"
        copy_done: "copiado"
      links:
        #  loop
        - title: "Mais exemplos"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
        #  loop
        - title: "Documentação"
          link: "https://docs.groupdocs.com/signature/java/"
          
      content: |
        ```java {style=abap}
        // Passe o documento para uma nova instância de Signature
        Signature signature = new Signature("input.jpeg");

        // Use QrCodeSignOptions para adicionar um código QR ao documento
        QrCodeSignOptions options = new QrCodeSignOptions("Text Content");

        // Especifique o tipo de assinatura e a posição na página
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(50);
        options.setTop(150);

        // Salve o arquivo com o código QR adicionado
        signature.sign("output.jpeg", options);

        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Adicione assinaturas aos seus documentos"
  description: "A API GroupDocs.Signature for Java suporta a assinatura de todos os formatos de arquivo populares. Gere, modifique, pesquise, verifique e exclua diferentes tipos de assinaturas."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "Recursos Principais do GroupDocs.Signature"
  features:
    # feature loop
    - title: "Assinar documentos"
      content: "GroupDocs.Signature suporta assinatura com Textos, Imagens, Códigos de Barras, QR Codes e assinaturas de Carimbo. Coloque-as em qualquer página de qualquer formato de documento compatível. Gerencie metadados do documento com assinaturas de metadados e proteja o conteúdo de alterações não autorizadas usando certificados digitais."

    # feature loop
    - title: "Pesquisa e verificação"
      content: "Certifique-se de que todas as assinaturas em um documento são válidas com o procedimento de verificação. Recupere uma lista completa de assinaturas em um documento usando o recurso de pesquisa integrado."

    # feature loop
    - title: "Modificar assinaturas"
      content: "Modifique facilmente as propriedades da assinatura após a assinatura. Ajuste conteúdo, posição, cor, tamanho e outros atributos conforme necessário."

    # feature loop
    - title: "Remover assinaturas"
      content: "Exclua assinaturas indesejadas com facilidade. Vários tipos de assinaturas, incluindo certificados digitais, podem ser removidos programaticamente dos documentos."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Como personalizar um código QR gerado"
      content: |
        Use este exemplo para aprender a inserir um novo código QR em uma página JPEG.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Obtenha o documento que precisa ser assinado e passe-o para Signature
          Signature signature = new Signature("input.jpeg");

          // Use opções de código QR para fornecer texto com as informações necessárias
          QrCodeSignOptions signOptions = new QrCodeSignOptions("Archived on July 11, 2019");

          // Defina a posição relativa do código QR na página
          signOptions.setVerticalAlignment(VerticalAlignment.Top);
          signOptions.setHorizontalAlignment(HorizontalAlignment.Right);

          // Defina a margem da assinatura
          Padding padding = new Padding();
          padding.setRight(20);
          padding.setTop(20);
          signOptions.setMargin(padding);

          // Especifique a cor do código QR
          signOptions.setForeColor(Color.RED);

          // Defina as opções de fonte para a mensagem
          SignatureFont font = new SignatureFont();
          font.setSize(12);
          font.setFamilyName("Comic Sans MS");
          signOptions.setFont(font);

          // Personalize a cor e o estilo de fundo do código QR
          Background background = new Background();
          background.setColor(Color.GREEN);
          background.setTransparency(0.5);
          background.setBrush(new LinearGradientBrush(Color.GREEN, Color.DARK_GRAY, 0));
          signOptions.setBackground(background);

          // Adicione o código QR ao documento
          SignResult signResult = signature.sign("output.jpeg", signOptions);
          ```
        platform: "java"
        copy_title: "Copiar"
        install:
          command_title: "Maven XML"
          command: |
            <dependencies>
              <dependency>
                <groupId>com.groupdocs</groupId>
                <artifactId>groupdocs-signature</artifactId>
                <version>{0}</version>
              </dependency>
            </dependencies>
            <repositories>
              <repository>
                <id>repository.groupdocs.com</id>
                <name>GroupDocs Repository</name>
                <url>https://repository.groupdocs.com/repo/</url>
              </repository>
            </repositories>
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
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
          #  loop
          - title: "Documentação"
            link: "https://docs.groupdocs.com/signature/java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Pronto para começar?"
  description: "Experimente os recursos do GroupDocs.Signature gratuitamente ou solicite uma licença"
  items:
    #  loop
    - title: "Baixar Maven"
      link: "https://releases.groupdocs.com/signature/java/"
      color: "red"
        #  loop
    - title: "Licenciamento"
      link: "https://purchase.groupdocs.com/pricing/signature/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Confira nossas principais ofertas"
    exclude: "qrcode"
    description: "Oferecemos uma seleção diversificada de recursos de assinatura e operações avançadas."
    items: 
          
        # operation loop 1
        - name: "Assinaturas eletrônicas"
          operation: "esign"
          link: "/signature/java/esign/jpeg/"
          description: "Adicionar vários tipos de assinaturas a formatos de arquivo suportados"

        # operation loop 2
        - name: "Adicionar texto a documentos"
          operation: "text"
          link: "/signature/java/text/jpeg/"
          description: "Melhore o conteúdo do documento com assinaturas de texto personalizáveis"

        # operation loop 3
        - name: "Assinaturas de imagem"
          operation: "image"
          link: "/signature/java/image/jpeg/"
          description: "Colocar qualquer imagem em qualquer posição dentro de um documento"

        # operation loop 4
        - name: "Gerar códigos de barras"
          operation: "barcode"
          link: "/signature/java/barcode/jpeg/"
          description: "Criar e inserir vários códigos de barras em documentos suportados"

        # operation loop 5
        - name: "Gerar QR codes"
          operation: "qrcode"
          link: "/signature/java/qrcode/jpeg/"
          description: "Gerar e QR Codes, incluindo códigos QR, para assinatura de documentos"
          
        # operation loop 6
        - name: "Certificados digitais"
          operation: "digital"
          link: "/signature/java/digital/pdf/"
          description: "Proteger negócios e assinar documentos com certificados digitais"

        # operation loop 7
        - name: "Assinaturas de carimbo"
          operation: "stamp"
          link: "/signature/java/stamp/jpeg/"
          description: "Use o Construtor de Carimbos para criar carimbos redondos ou quadrados personalizados"
          
        # operation loop 8
        - name: "Buscar assinaturas"
          operation: "search"
          link: "/signature/java/search/pdf/"
          description: "Localizar quaisquer assinaturas previamente adicionadas em um documento"
          
        # operation loop 9
        - name: "Verificação de assinaturas"
          operation: "verify"
          link: "/signature/java/verify/pdf/"
          description: "Verificar a autenticidade das assinaturas após a aplicação"
          
        # operation loop 10
        - name: "Modificar assinaturas"
          operation: "modify"
          link: "/signature/java/modify/pdf/"
          description: "Editar uma variedade de assinaturas dentro de um documento"
          
        # operation loop 11
        - name: "Excluir assinaturas"
          operation: "delete"
          link: "/signature/java/delete/pdf/"
          description: "Remover uma ampla gama de assinaturas previamente aplicadas"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Gere códigos QR para formatos de arquivo adicionais"
    exclude: "JPEG"
    description: "Aprimore todos os formatos de arquivo populares com códigos QR gerados usando a API Java. Adicione dados de código de barras 2D para fácil leitura e processamento."
    items: 
          
        # format loop 1
        - name: "QR-Code para PDF"
          format: "PDF"
          link: "/signature/java/qrcode/pdf/"
          description: "Formato de Documento Portátil Adobe"
          
        # format loop 2
        - name: "QR-Code para DOCX"
          format: "DOCX"
          link: "/signature/java/qrcode/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 3
        - name: "QR-Code para JPEG"
          format: "JPEG"
          link: "/signature/java/qrcode/jpeg/"
          description: "Imagem JPEG"
          
        # format loop 4
        - name: "QR-Code para PPTX"
          format: "PPTX"
          link: "/signature/java/qrcode/pptx/"
          description: "Apresentação PowerPoint Open XML"
          
        # format loop 5
        - name: "QR-Code para XLSX"
          format: "XLSX"
          link: "/signature/java/qrcode/xlsx/"
          description: "Planilha Microsoft Excel Open XML"


          

---