



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:28
draft: false
lang: pt
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Assine arquivos DOCX com aplicativos Java"
head_description: "Use a API Java para processar arquivos DOCX e aplicar vários tipos de assinaturas, incluindo PDF, Word, Excel, Apresentações e Imagens."

############################# Header ############################
title: "Assinaturas eletrônicas para DOCX" 
description: "Adicione uma ampla gama de assinaturas eletrônicas usando GroupDocs.Signature for Java a todos os formatos de negócios populares, incluindo PDF, Word, Excel, Apresentações e Imagens."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download gratuito"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "Sobre a API GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "Saiba mais"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) oferece recursos avançados de e-signature. Use-o para adicionar, pesquisar, verificar, modificar e remover vários tipos de e-assinaturas em documentos e imagens, sem a necessidade de software externo. Assine PDFs, documentos Word, planilhas Excel, apresentações PowerPoint e formatos de imagem populares.

############################# Steps ############################
steps:
    enable: true
    title: "Etapas para assinar DOCX usando Java"
    content: |
      [GroupDocs.Signature](/signature/java/) permite adicionar assinaturas personalizadas a arquivos DOCX. Desenvolvedores de Java podem integrar a funcionalidade de assinatura em seus aplicativos usando nosso software.
      
      1. Forneça o arquivo DOCX a ser assinado para a instância Signature.
      2. Use SignOptions para definir os detalhes da assinatura.
      3. Personalize várias propriedades, como tamanho, cor e conteúdo.
      4. Salve o arquivo assinado no local desejado.
   
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
        // Carregue o documento em uma instância Signature
        Signature signature = new Signature("input.docx");

        // Instancie um objeto QrCodeSignOptions
        QrCodeSignOptions options = new QrCodeSignOptions("QR code text");

        // Configure todas as opções desejadas
        options.setLeft(100);
        options.setTop(100);
        options.setForeColor(Color.RED);

        // Salve o arquivo com o código QR adicionado no disco local
        signature.sign("output.docx", options);
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Assinaturas eletrônicas de documentos"
  description: "Nossa API de e-signing simplifica os processos de negócios. Assine, pesquise, atualize, exclua e verifique várias assinaturas programaticamente."
  image: "/img/signature/features_esign.webp" # 500x500 px
  image_description: "Assinaturas eletrônicas"
  features:
    # feature loop
    - title: "Assine documentos de escritório"
      content: "Posicione assinaturas eletrônicas em qualquer lugar de qualquer página de um documento. Enriqueca o conteúdo do documento com texto, imagens, códigos de barras, metadados ou certificados digitais."

    # feature loop
    - title: "Gerenciamento de assinaturas"
      content: "Após a assinatura, os documentos podem ser processados de forma adicional. Recupere uma lista de todas as assinaturas presentes, modifique-as ou exclua-as conforme necessário."

    # feature loop
    - title: "Controle avançado de conteúdo"
      content: "Proteja documentos de negócios contra alterações não autorizadas com certificados digitais corporativos. Adicione ou extraia entradas de metadados ocultos disponíveis em todos os tipos de documentos."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Como adicionar uma assinatura de imagem a um documento"
      content: |
        Este exemplo demonstra como colocar uma assinatura de imagem em uma página específica de um documento.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Forneça o documento fonte como parâmetro
          Signature signature = new Signature("input.docx");

          // Especifique o caminho da imagem nas opções de assinatura
          ImageSignOptions options = new ImageSignOptions("image.jpg");

          // Defina o tamanho e as páginas alvo para a assinatura
          options.setVerticalAlignment(VerticalAlignment.Bottom);
          options.setHorizontalAlignment(HorizontalAlignment.Right);
          options.setHeight(150);
          options.setWidth(200);
          Padding padding = new Padding(50);
          options.setMargin(padding);
          options.setAllPages(true);

          // Aplique a assinatura ao documento
          signature.sign("output.docx", options);

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
            link: "/examples/signature/formats/signature_esign.docx"
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
    title: "Explore nossos principais recursos"
    exclude: "esign"
    description: "Temos orgulho em oferecer uma ampla gama de assinaturas e operações suportadas."
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
    title: "Assine formatos de arquivo populares com e-assinaturas"
    exclude: "DOCX"
    description: "A API de e-signing para Java permite o processamento de todos os formatos de arquivo e documento modernos de negócios."
    items: 
          
        # format loop 1
        - name: "Assinatura eletrônica em PDF"
          format: "PDF"
          link: "/signature/java/esign/pdf/"
          description: "Formato de Documento Portátil Adobe"
          
        # format loop 2
        - name: "Assinatura eletrônica em DOCX"
          format: "DOCX"
          link: "/signature/java/esign/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 3
        - name: "Assinatura eletrônica em JPEG"
          format: "JPEG"
          link: "/signature/java/esign/jpeg/"
          description: "Imagem JPEG"
          
        # format loop 4
        - name: "Assinatura eletrônica em PPTX"
          format: "PPTX"
          link: "/signature/java/esign/pptx/"
          description: "Apresentação PowerPoint Open XML"
          
        # format loop 5
        - name: "Assinatura eletrônica em XLSX"
          format: "XLSX"
          link: "/signature/java/esign/xlsx/"
          description: "Planilha Microsoft Excel Open XML"


          

---