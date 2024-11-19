



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:16
draft: false
lang: pt
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Adicionar assinaturas eletrônicas digitais ao arquivo DOCX com Java"
head_description: "Coloque uma assinatura digital em um arquivo DOCX usando Java com apenas algumas linhas de código. Use GroupDocs.Signature for Java para assinar diversos formatos de arquivo."

############################# Header ############################
title: "Assine DOCX com assinaturas digitais" 
description: "Proteja o conteúdo dos seus documentos comerciais selando-os com certificados digitais através dos recursos do GroupDocs.Signature for Java. Oferecemos várias maneiras de marcar e proteger seus documentos."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Baixe gratuitamente"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "Sobre GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "Saiba mais"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) é uma solução abrangente de assinatura que suporta diversos tipos de processamento de documentos. Você pode adicionar texto, imagens, certificados digitais e carimbos a arquivos em mais de 60 formatos, incluindo PDF, MS Office, imagens, arquivos ZIP e outros formatos de negócios populares. Além disso, documentos assinados podem ser pesquisados, verificados, modificados ou excluídos automaticamente de maneira conveniente.

############################# Steps ############################
steps:
    enable: true
    title: "Passos para proteger DOCX com certificados digitais em Java"
    content: |
      [GroupDocs.Signature](/signature/java/) permite que desenvolvedores Java evitem alterações em documentos DOCX usando assinaturas digitais. Capacite suas aplicações empresariais com a capacidade de proteger dados importantes.
      
      1. Passe o documento DOCX para o construtor da classe Signature.
      2. Use um certificado digital e sua senha para proteger o documento.
      3. Opcionalmente, adicione uma representação visual da assinatura digital nas páginas do documento.
      4. Assine o documento para evitar quaisquer alterações futuras.
   
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
        // Use Signature com o documento para assinatura digital
        Signature signature = new Signature("input.docx");

        // Forneça um certificado digital e senha
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");
        options.setPassword("1234567890");

        // Configure uma representação visual se necessário
        options.setPageNumber(1);
        options.setLeft(100);
        options.setTop(100);

        // Proteja o documento com um certificado digital
        SignResult result = signature.sign("output.docx", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Melhore ou proteja o conteúdo do documento com assinaturas"
  description: "A biblioteca GroupDocs.Signature for Java é capaz de assinar todos os formatos de arquivo populares. Adicione, modifique, verifique ou exclua automaticamente vários tipos de assinaturas para otimizar seus processos de negócios."
  image: "/img/signature/features_digital.webp" # 500x500 px
  image_description: "Recursos do GroupDocs.Signature"
  features:
    # feature loop
    - title: "Adicionar assinaturas a documentos"
      content: "Assinaturas de Texto, Imagem, Código de Barras, QR-Code ou Carimbo podem ser adicionadas com precisão a qualquer página de qualquer documento suportado. Metadados ocultos como EXIF podem ser adicionados ou editados em imagens e na maioria dos tipos de arquivo. Proteja o conteúdo do documento contra alterações não autorizadas usando assinaturas digitais."

    # feature loop
    - title: "Pesquisa e verificação de assinaturas"
      content: "Os documentos podem ser processados de várias maneiras após a assinatura. Verifique documentos assinados para garantir que foram processados corretamente. Se precisar de mais controle, recupere uma lista de todas as assinaturas por meio de pesquisa."

    # feature loop
    - title: "Editar assinaturas"
      content: "A maioria dos tipos de assinaturas suporta modificação adicional. Você pode corrigir texto, alterar posição, cor, tamanho e mais."

    # feature loop
    - title: "Remover assinaturas desnecessárias"
      content: "Nossa solução suporta operações completas de CRUD para assinaturas. Muitos tipos de assinaturas, incluindo certificados digitais, podem ser excluídos de um documento quando necessário."
      
  code_samples:
    # code sample loop
    - title: "Proteger documentos com assinaturas digitais"
      content: |
        Aprenda a proteger um documento contra alterações usando assinaturas digitais.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        // Forneça um documento para assinatura
        Signature signature = new Signature("input.docx");

        // Use um certificado digital válido com uma senha
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");
        options.setPassword("1234567890");

        // Especifique dados textuais adicionais
        options.setReason("Security issue");
        options.setContact("John Smith");
        options.setLocation("Office D.W.");

        // Use uma imagem e outras opções para representação visual
        options.setImageFilePath("image.png");

        options.setAllPages(true);
        options.setVerticalAlignment(VerticalAlignment.Bottom);
        options.setHorizontalAlignment(HorizontalAlignment.Right);
        options.setWidth(80);
        options.setHeight(60);

        Padding padding = new Padding();
        padding.setBottom(10);
        padding.setRight(10);
        options.setMargin(padding);

        // Salve o documento protegido em um local diferente
        SignResult result = signature.sign("output.docx", options);
        ```
        {{< /landing/code >}}


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
    title: "Examine nosso conjunto de recursos abrangente"
    exclude: "digital"
    description: "Temos orgulho da funcionalidade extensa e do suporte a assinaturas que nossa plataforma oferece."
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
    description: "A API Java permite que você processe mais de 60 formatos. Crie e adicione várias assinaturas a qualquer página, selando o conteúdo com certificados digitais, além de gerenciar e editar assinaturas existentes dentro do documento."
    items: 
          
        # format loop 1
        - name: "Proteger PDF"
          format: "PDF"
          link: "/signature/java/digital/pdf/"
          description: "Formato de Documento Portátil Adobe"
          
        # format loop 2
        - name: "Proteger DOCX"
          format: "DOCX"
          link: "/signature/java/digital/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 3
        - name: "Proteger PPTX"
          format: "PPTX"
          link: "/signature/java/digital/pptx/"
          description: "Apresentação PowerPoint Open XML"
          
        # format loop 4
        - name: "Proteger XLSX"
          format: "XLSX"
          link: "/signature/java/digital/xlsx/"
          description: "Planilha Microsoft Excel Open XML"


          

---