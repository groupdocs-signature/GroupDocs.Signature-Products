



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:46
draft: false
lang: pt
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Adicione carimbos ao JPEG usando Java"
head_description: "Aproveite o GroupDocs.Signature e Java para criar carimbos personalizados e colocá-los em qualquer página dentro de documentos JPEG."

############################# Header ############################
title: "Adicione carimbos personalizados ao JPEG" 
description: "Desenhe e aplique carimbos redondos ou quadrados em qualquer seção dos seus documentos usando GroupDocs.Signature for Java. Nossa solução oferece amplas opções de personalização para atender a todas as suas necessidades empresariais."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Baixar gratuitamente"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "Sobre GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "Saiba mais"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) é uma ferramenta robusta que permite adicionar várias assinaturas de carimbo a documentos. Suporta mais de 60 formatos de arquivo diferentes, incluindo PDFs, Word, Excel, imagens e arquivos ZIP. Você pode aplicar assinaturas de texto, imagem, código de barras, metadados, certificado digital e carimbos. Além de adicionar assinaturas, você pode procurar, verificar, modificar e removê-las.

############################# Steps ############################
steps:
    enable: true
    title: "Passos para adicionar carimbos ao JPEG via Java"
    content: |
      [GroupDocs.Signature](/signature/java/) fornece um construtor de carimbo que pode ser extremamente benéfico para aplicações Java. Utilize-o para criar carimbos bem personalizados para as páginas do seu documento.
      
      1. Forneça o documento JPEG a ser carimbado.
      2. Use StampSignOptions para configurar todos os parâmetros necessários.
      3. Adicione quantas linhas forem necessárias.
      4. Aplique o carimbo e salve o documento.
   
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
        // Use o caminho do documento com o objeto Signature
        Signature signature = new Signature("input.jpeg");

        // Instancie StampSignOptions com o texto da assinatura desejado
        StampSignOptions options = new StampSignOptions();
        options.Height = 180;
        options.Width = 180;

        // Adicione uma ou mais linhas de carimbo
        StampLine outerLine = new StampLine();
        outerLine.setText("* The Best Company *");
        outerLine.setTextRepeatType(StampTextRepeatType.FullTextRepeat);
        outerLine.getFont().setSize(12);
        outerLine.setHeight(22);
        outerLine.setTextBottomIntent(6);
        outerLine.setTextColor(Color.WHITE);
        outerLine.setBackgroundColor(Color.BLUE);
        options.getOuterLines().add(outerLine);

        // Salve o documento carimbado
        SignResult result = signature.sign("output.jpeg", options);
        ```        

############################# More features ############################
more_features:
  enable: true
  title: "Proteja o conteúdo do seu documento com assinaturas"
  description: "A biblioteca GroupDocs.Signature for Java é projetada para assinar e gerenciar assinaturas em formatos de arquivo populares. Adicione, modifique, verifique ou remova carimbos e outros tipos de assinaturas sem esforço."
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "Assinaturas de Carimbo com GroupDocs.Signature"
  features:
    # feature loop
    - title: "Assine seus documentos"
      content: "Aplique assinaturas personalizáveis em qualquer parte do seu documento. Escolha entre vários tipos de assinatura, incluindo texto, imagens, códigos de barras, códigos QR e carimbos. Além disso, metadados ocultos podem ser adicionados ou modificados para aumentar a segurança do documento."

    # feature loop
    - title: "Pesquise e valide assinaturas"
      content: "Uma vez que um documento é assinado, utilize nossas ferramentas de verificação para garantir que o conteúdo da assinatura seja válido. Pesquise e recupere uma lista de todas as assinaturas para processamento adicional."

    # feature loop
    - title: "Atualize assinaturas conforme necessário"
      content: "Modifique facilmente uma ampla gama de assinaturas aplicadas a um documento. Atualize propriedades como tamanho, cor, posição, conteúdo e mais."

    # feature loop
    - title: "Remova assinaturas"
      content: "Precisa remover assinaturas de um documento? Nossa API oferece suporte total à exclusão de assinaturas, facilitando a gestão eficaz dos seus documentos."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Adicione carimbos personalizados a documentos usando assinaturas especiais"
      content: |
        Aprenda como gerar e adicionar carimbos personalizados com informações textuais importantes aos seus documentos.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Forneça o documento a ser carimbado
          Signature signature = new Signature("input.jpeg");

          // Instancie o objeto de opções de carimbo
          StampSignOptions options = new StampSignOptions();

          // Defina o tamanho e a posição na página
          options.setHeight(200);
          options.setWidth(200);
          options.setVerticalAlignment(VerticalAlignment.Bottom);
          options.setHorizontalAlignment(HorizontalAlignment.Right);
          options.setAllPages(true);

          // Adicione uma ou mais linhas redondas externas com texto
          StampLine outerLine1 = new StampLine();
          outerLine1.setText("* The best  choice *");
          outerLine1.setTextRepeatType(StampTextRepeatType.FullTextRepeat);
          SignatureFont signatureFont1 = new SignatureFont();
          signatureFont1.setSize(12);
          signatureFont1.setFamilyName("Arial");
          outerLine1.setFont(signatureFont1);
          outerLine1.setHeight(30);
          outerLine1.setTextBottomIntent(6);
          outerLine1.setTextColor(Color.WHITE);
          outerLine1.setBackgroundColor(Color.BLUE);
          options.getOuterLines().add(outerLine1);

          // Adicione uma ou mais linhas quadradas internas
          StampLine innerLine1 = new StampLine();
          innerLine1.setText("Company #1");
          innerLine1.setTextColor(Color.RED);
          SignatureFont signFont1 = new SignatureFont();
          signFont1.setSize(20);
          signFont1.setBold(true);
          innerLine1.setFont(signFont1);
          innerLine1.setHeight(40);
          options.getInnerLines().add(innerLine1);

          // Salve o documento carimbado
          SignResult result = signature.sign("output.jpeg", options);
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
            link: "/examples/signature/formats/signature_stamp.jpeg"
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
    title: "Explore nossos recursos principais"
    exclude: "stamp"
    description: "Utilize uma ampla gama de opções para adicionar, gerenciar e excluir assinaturas."
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
    title: "Adicione carimbos em vários formatos de arquivo"
    exclude: "JPEG"
    description: "A API GroupDocs.Signature suporta carimbar documentos em mais de 60 formatos. Coloque carimbos em qualquer página ou área para melhorar a gestão e personalização do documento."
    items: 
          
        # format loop 1
        - name: "Carimbar PDF"
          format: "PDF"
          link: "/signature/java/stamp/pdf/"
          description: "Formato de Documento Portátil Adobe"
          
        # format loop 2
        - name: "Carimbar DOCX"
          format: "DOCX"
          link: "/signature/java/stamp/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 3
        - name: "Carimbar JPEG"
          format: "JPEG"
          link: "/signature/java/stamp/jpeg/"
          description: "Imagem JPEG"
          
        # format loop 4
        - name: "Carimbar PPTX"
          format: "PPTX"
          link: "/signature/java/stamp/pptx/"
          description: "Apresentação PowerPoint Open XML"
          
        # format loop 5
        - name: "Carimbar XLSX"
          format: "XLSX"
          link: "/signature/java/stamp/xlsx/"
          description: "Planilha Microsoft Excel Open XML"


          

---