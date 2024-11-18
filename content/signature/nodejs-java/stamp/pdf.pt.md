



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:48
draft: false
lang: pt
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Gerar e adicionar carimbos ao PDF via JavaScript"
head_description: "Aproveite o poder do GroupDocs.Signature e JavaScript para gerar e posicionar carimbos personalizados em qualquer página dos seus documentos PDF."

############################# Header ############################
title: "Insira carimbos personalizados em arquivos PDF" 
description: "Utilize o GroupDocs.Signature for Node.js via Java para gerar carimbos adaptados e inseri-los em qualquer local dos seus documentos. Nossa plataforma oferece amplas opções para personalizar carimbos de acordo com suas necessidades empresariais específicas."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Teste gratuito"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "O que é GroupDocs.Signature for Node.js via Java?"
    link: "/signature/nodejs-java/"
    link_title: "Saiba mais"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) oferece uma solução robusta e versátil para assinatura de documentos. Permite que os usuários adicionem carimbos e outros tipos de assinatura em mais de 60 formatos diferentes, como PDFs, Word, Excel, arquivos de imagens e arquivos ZIP. A plataforma permite inserir texto, imagem, código de barras, QR code, metadados, certificado digital e assinaturas em carimbos. Além da assinatura, você pode buscar, verificar, modificar ou excluir quaisquer assinaturas presentes em seus documentos.

############################# Steps ############################
steps:
    enable: true
    title: "Guia para incorporar carimbos em PDF usando JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) oferece uma poderosa ferramenta para criar e incorporar carimbos, que podem melhorar significativamente as aplicações Node.js via Java. Use este recurso para criar e aplicar carimbos personalizados nas páginas do seu documento.
      
      1. Insira o documento PDF que requer carimbagem.
      2. Implante StampSignOptions para definir todos os parâmetros essenciais.
      3. Insira quantas linhas de carimbo forem necessárias.
      4. Aplique o carimbo e salve o documento finalizado.
   
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

        // Associe o caminho do documento à instância Signature
        const signature = new signatureLib.Signature('input.pdf');

        // Crie StampSignOptions com o conteúdo da assinatura necessário
        const options = new signatureLib.StampSignOptions();
        options.Height = 180;
        options.Width = 180;

        // Incorpore uma ou mais linhas de carimbo
        const outerLine = new signatureLib.StampLine();
        outerLine.setText("* The Best Company *");
        outerLine.setTextRepeatType(signatureLib.StampTextRepeatType.FullTextRepeat);
        outerLine.getFont().setSize(12);
        outerLine.setHeight(22);
        outerLine.setTextBottomIntent(6);
        outerLine.setTextColor(signatureLib.Color.WHITE);
        outerLine.setBackgroundColor(signatureLib.Color.BLUE);
        options.getOuterLines().add(outerLine);

        // Salve o documento com o carimbo aplicado
        const result = signature.sign('output.pdf', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Fortaleça a segurança dos documentos com assinaturas"
  description: "Com o GroupDocs.Signature for Node.js via Java, você pode adicionar, editar, validar ou remover carimbos e outros tipos de assinatura em todos os formatos de documentos populares. A API simplifica o processo de gerenciamento de assinaturas para melhorar a integridade e a personalização dos documentos."
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "Recursos do GroupDocs.Signature"
  features:
    # feature loop
    - title: "Assinatura personalizada de documentos"
      content: "Aplique assinaturas como texto, imagens, códigos de barras, QR codes e carimbos a qualquer parte do seu documento. Esta ferramenta também permite a inclusão de metadados ocultos e certificados digitais para proteger ainda mais seu conteúdo contra modificações não autorizadas."

    # feature loop
    - title: "Busca e verificação de assinaturas"
      content: "Após a assinatura de um documento, use nosso sistema de verificação para garantir a integridade das assinaturas. Além disso, nossa plataforma permite que você busque e recupere informações detalhadas sobre todas as assinaturas aplicadas a um documento."

    # feature loop
    - title: "Modifique assinaturas conforme necessário"
      content: "Ajuste e atualize assinaturas aplicadas anteriormente. Quer você altere o conteúdo, cor, tamanho ou posição da assinatura, o GroupDocs.Signature for Node.js via Java oferece opções completas de personalização."

    # feature loop
    - title: "Remova assinaturas indesejadas"
      content: "Remova facilmente quaisquer assinaturas desnecessárias de seus documentos. Nossa API suporta a exclusão de uma ampla gama de tipos de assinatura, incluindo carimbos e certificados digitais, oferecendo total flexibilidade para gerenciar seus documentos."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Integre carimbos personalizados em documentos"
      content: |
        Aprenda como criar e aplicar carimbos personalizados contendo texto essencial aos seus documentos.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // Forneça o documento para carimbagem
          const signature = new signatureLib.Signature('input.pdf');

          // Configurar as opções de carimbo com as configurações desejadas
          const options = new signatureLib.StampSignOptions();

          // Especifique as dimensões e a posição do carimbo na página
          options.setHeight(200);
          options.setWidth(200);
          options.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          options.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);
          options.setAllPages(true);

          // Inclua linhas externas circulares com texto personalizado
          const outerLine1 = new signatureLib.StampLine();
          outerLine1.setText('* The best  choice *');
          outerLine1.setTextRepeatType(signatureLib.StampTextRepeatType.FullTextRepeat);
          const signatureFont1 = new signatureLib.SignatureFont();
          signatureFont1.setSize(12);
          signatureFont1.setFamilyName('Arial');
          outerLine1.setFont(signatureFont1);
          outerLine1.setHeight(30);
          outerLine1.setTextBottomIntent(6);
          outerLine1.setTextColor(signatureLib.Color.WHITE);
          outerLine1.setBackgroundColor(signatureLib.Color.BLUE);
          options.getOuterLines().add(outerLine1);

          // Adicione linhas internas quadradas conforme necessário
          const innerLine1 = new signatureLib.StampLine();
          innerLine1.setText('Company #1');
          innerLine1.setTextColor(signatureLib.Color.RED);
          const signFont1 = new signatureLib.SignatureFont();
          signFont1.setSize(20);
          signFont1.setBold(true);
          innerLine1.setFont(signFont1);
          innerLine1.setHeight(40);
          options.getInnerLines().add(innerLine1);
          
          // Salve o documento carimbado
          const result = signature.sign('output.pdf', options);
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
            link: "/examples/signature/formats/signature_stamp.pdf"
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
    title: "Explore os recursos principais"
    exclude: "stamp"
    description: "Nossa solução oferece uma variedade de ferramentas para criar, gerenciar e remover diferentes tipos de assinaturas, proporcionando aos usuários total controle sobre seus fluxos de trabalho de documentos."
    items: 
          
        # operation loop 1
        - name: "Assinaturas eletrônicas"
          operation: "esign"
          link: "/signature/nodejs-java/esign/pdf/"
          description: "Adicionar vários tipos de assinaturas a formatos de arquivo suportados"

        # operation loop 2
        - name: "Adicionar texto a documentos"
          operation: "text"
          link: "/signature/nodejs-java/text/pdf/"
          description: "Melhore o conteúdo do documento com assinaturas de texto personalizáveis"

        # operation loop 3
        - name: "Assinaturas de imagem"
          operation: "image"
          link: "/signature/nodejs-java/image/pdf/"
          description: "Colocar qualquer imagem em qualquer posição dentro de um documento"

        # operation loop 4
        - name: "Gerar códigos de barras"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/pdf/"
          description: "Criar e inserir vários códigos de barras em documentos suportados"

        # operation loop 5
        - name: "Gerar QR codes"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/pdf/"
          description: "Gerar e QR Codes, incluindo códigos QR, para assinatura de documentos"
          
        # operation loop 6
        - name: "Certificados digitais"
          operation: "digital"
          link: "/signature/nodejs-java/digital/pdf/"
          description: "Proteger negócios e assinar documentos com certificados digitais"

        # operation loop 7
        - name: "Assinaturas de carimbo"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/pdf/"
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
    title: "Aplique assinaturas em carimbos em vários tipos de arquivo"
    exclude: "PDF"
    description: "A API GroupDocs.Signature suporta assinaturas em carimbos em mais de 60 formatos de arquivo, permitindo que os usuários coloquem carimbos personalizados em qualquer página ou área, melhorando a acessibilidade e a segurança dos documentos."
    items: 
          
        # format loop 1
        - name: "Carimbar PDF"
          format: "PDF"
          link: "/signature/nodejs-java/stamp/pdf/"
          description: "Formato de Documento Portátil Adobe"
          
        # format loop 2
        - name: "Carimbar DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/stamp/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 3
        - name: "Carimbar JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/stamp/jpeg/"
          description: "Imagem JPEG"
          
        # format loop 4
        - name: "Carimbar PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/stamp/pptx/"
          description: "Apresentação PowerPoint Open XML"
          
        # format loop 5
        - name: "Carimbar XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/stamp/xlsx/"
          description: "Planilha Microsoft Excel Open XML"


          

---