



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:05
draft: false
lang: pt
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Adicione códigos de barras a arquivos DOCX com Java"
head_description: "Crie e insira assinaturas de código de barras em documentos DOCX em Java. GroupDocs.Signature permite uma integração versátil de assinaturas para múltiplos formatos."

############################# Header ############################
title: "Gere códigos de barras para DOCX" 
description: "Adicione códigos de barras de formatos populares em qualquer parte dos seus documentos comerciais com GroupDocs.Signature for Java. Nossa solução oferece amplas opções para personalizar assinaturas de código de barras."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Baixar Grátis"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "Sobre GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "Saiba mais"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) é uma solução avançada de assinatura que suporta uma ampla gama de tipos de assinatura. Você pode assinar documentos com texto, imagens, códigos de barras, certificados digitais, carimbos e muito mais em mais de 60 formatos de arquivo, incluindo PDF, MS Office, imagens, arquivos ZIP e outros formatos comerciais populares. Além disso, as assinaturas em documentos assinados podem ser pesquisadas, verificadas, modificadas ou excluídas a qualquer momento.

############################# Steps ############################
steps:
    enable: true
    title: "Passos para gerar e adicionar um código de barras ao arquivo DOCX"
    content: |
      [GroupDocs.Signature](/signature/java/) pode gerar códigos de barras em vários formatos populares e colocá-los nas páginas de DOCX. Com suporte a mais de 60 tipos de códigos de barras, aplicações Java podem ser facilmente aprimoradas com capacidades de assinatura de códigos de barras incorporando nossa biblioteca.
      
      1. Forneça o arquivo ou fluxo DOCX a ser processado.
      2. Passe o texto do código de barras para a instância BarcodeSignOptions.
      3. Personalize as opções do código de barras, como posição, tamanho, etc.
      4. Salve o arquivo com o código de barras recém-adicionado.
   
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
        // Crie uma nova instância Signature com o caminho do documento
        Signature signature = new Signature("input.docx");

        // Use BarcodeSignOptions para adicionar um código de barras ao documento
        BarcodeSignOptions options = new BarcodeSignOptions("Business data");

        // Configure o tipo de código de barras e outras propriedades
        options.setEncodeType(BarcodeTypes.Code128);
        options.setLeft(100);
        options.setTop(100);

        // Salve o arquivo assinado
        signature.sign("output.docx", options);

        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Melhore ou proteja o conteúdo do documento com assinaturas"
  description: "A biblioteca GroupDocs.Signature for Java é projetada para assinar e processar formatos de arquivo populares. Adicione, modifique, verifique ou exclua rapidamente vários tipos de assinaturas."
  image: "/img/signature/features_barcode.webp" # 500x500 px
  image_description: "Recursos do GroupDocs.Signature"
  features:
    # feature loop
    - title: "Assinatura de documentos"
      content: "Assine qualquer página de documentos suportados com texto, imagens, códigos de barras, códigos QR ou carimbos. Adicione metadados ocultos como EXIF em imagens ou proteja o conteúdo do documento contra alterações não autorizadas usando certificados digitais."

    # feature loop
    - title: "Pesquisa e verificação de assinaturas"
      content: "Há muito mais que você pode fazer com um documento assinado. Oferecemos verificação de assinaturas para garantir que tudo esteja em ordem. Além disso, você pode recuperar uma lista de todas as assinaturas do documento por meio de uma pesquisa."

    # feature loop
    - title: "Modificar assinaturas"
      content: "A maioria das assinaturas adicionadas anteriormente pode ser modificada. Corrija facilmente texto, ajuste a posição ou mude a cor."

    # feature loop
    - title: "Excluir assinaturas"
      content: "Nossa solução suporta operações completas de CRUD para assinaturas. Muitos tipos de assinaturas podem ser excluídos de um documento quando necessário."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Como criar uma assinatura de código de barras"
      content: |
        Este exemplo demonstra como colocar um código de barras personalizado nas páginas do documento DOCX.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Forneça o documento a ser assinado
          Signature signature = new Signature("input.docx");

          // Crie opções de assinatura com o texto desejado
          BarcodeSignOptions signOptions = new BarcodeSignOptions("Accepted");
          signOptions.setEncodeType(BarcodeTypes.Code39FullASCII);

          // Defina a posição relativa do código de barras na página
          signOptions.setVerticalAlignment(VerticalAlignment.Bottom);
          signOptions.setHorizontalAlignment(HorizontalAlignment.Left);

          // Defina a margem do código de barras a partir da borda da página
          Padding padding = new Padding();
          padding.setLeft(20);
          padding.setTop(180);
          signOptions.setMargin(padding);

          // Defina a cor das barras
          signOptions.setForeColor(Color.RED);

          // Defina o estilo da fonte da mensagem
          SignatureFont font = new SignatureFont();
          font.setSize(12);
          font.setFamilyName("Arial");
          signOptions.setFont(font);

          // Especifique a posição da mensagem
          signOptions.setCodeTextAlignment(CodeTextAlignment.Above);

          // Assine e salve o documento
          SignResult signResult = signature.sign("output.docx", signOptions);

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
            link: "/examples/signature/formats/signature_barcode.docx"
        links:
          #  loop
          - title: "Mais exemplos"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
          #  loop
          - title: "Documentação"
            link: "https://docs.groupdocs.com/signature/java/"
            

            


############################## Actions ############################

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
    title: "Descubra nossas principais capacidades"
    exclude: "barcode"
    description: "Temos o orgulho de apresentar uma ampla variedade de assinaturas e funções suportadas."
    items: 
          
        # operation loop 1
        - name: "Assinaturas eletrônicas"
          operation: "esign"
          link: "/signature/java/esign/docx/"
          description: "Adicionar vários tipos de assinaturas a formatos de arquivo suportados"

        # operation loop 2
        - name: "Adicionar texto a documentos"
          operation: "text"
          link: "/signature/java/text/docx/"
          description: "Melhore o conteúdo do documento com assinaturas de texto personalizáveis"

        # operation loop 3
        - name: "Assinaturas de imagem"
          operation: "image"
          link: "/signature/java/image/docx/"
          description: "Colocar qualquer imagem em qualquer posição dentro de um documento"

        # operation loop 4
        - name: "Gerar códigos de barras"
          operation: "barcode"
          link: "/signature/java/barcode/docx/"
          description: "Criar e inserir vários códigos de barras em documentos suportados"

        # operation loop 5
        - name: "Gerar QR codes"
          operation: "qrcode"
          link: "/signature/java/qrcode/docx/"
          description: "Gerar e QR Codes, incluindo códigos QR, para assinatura de documentos"
          
        # operation loop 6
        - name: "Certificados digitais"
          operation: "digital"
          link: "/signature/java/digital/docx/"
          description: "Proteger negócios e assinar documentos com certificados digitais"

        # operation loop 7
        - name: "Assinaturas de carimbo"
          operation: "stamp"
          link: "/signature/java/stamp/docx/"
          description: "Use o Construtor de Carimbos para criar carimbos redondos ou quadrados personalizados"
          
        # operation loop 8
        - name: "Buscar assinaturas"
          operation: "search"
          link: "/signature/java/search/docx/"
          description: "Localizar quaisquer assinaturas previamente adicionadas em um documento"
          
        # operation loop 9
        - name: "Verificação de assinaturas"
          operation: "verify"
          link: "/signature/java/verify/docx/"
          description: "Verificar a autenticidade das assinaturas após a aplicação"
          
        # operation loop 10
        - name: "Modificar assinaturas"
          operation: "modify"
          link: "/signature/java/modify/docx/"
          description: "Editar uma variedade de assinaturas dentro de um documento"
          
        # operation loop 11
        - name: "Excluir assinaturas"
          operation: "delete"
          link: "/signature/java/delete/docx/"
          description: "Remover uma ampla gama de assinaturas previamente aplicadas"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Assine documentos em outros formatos"
    exclude: "DOCX"
    description: "Mais de 60 formatos podem ser assinados usando nossa API Java. Aplique várias assinaturas a qualquer página ou posição dentro do documento."
    items: 
          
        # format loop 1
        - name: "Adicionar código de barras ao PDF"
          format: "PDF"
          link: "/signature/java/barcode/pdf/"
          description: "Formato de Documento Portátil Adobe"
          
        # format loop 2
        - name: "Adicionar código de barras ao DOCX"
          format: "DOCX"
          link: "/signature/java/barcode/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 3
        - name: "Adicionar código de barras ao JPEG"
          format: "JPEG"
          link: "/signature/java/barcode/jpeg/"
          description: "Imagem JPEG"
          
        # format loop 4
        - name: "Adicionar código de barras ao PPTX"
          format: "PPTX"
          link: "/signature/java/barcode/pptx/"
          description: "Apresentação PowerPoint Open XML"
          
        # format loop 5
        - name: "Adicionar código de barras ao XLSX"
          format: "XLSX"
          link: "/signature/java/barcode/xlsx/"
          description: "Planilha Microsoft Excel Open XML"


          

---