



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:10
draft: false
lang: pt
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Adicionando assinaturas de imagem ao arquivo JPEG com JavaScript"
head_description: "Coloque uma assinatura de imagem no arquivo JPEG para Node.js usando algumas linhas de código. Utilize a API GroupDocs.Signature for Node.js via Java para adicionar imagens."

############################# Header ############################
title: "Assine arquivos JPEG utilizando assinaturas de imagem" 
description: "Aproveite as capacidades do GroupDocs.Signature for Node.js via Java para integrar imagens de maneira eficaz em uma variedade de formatos de documentos, como PDFs, Word, Excel e vários arquivos de imagem. Adicionar uma imagem de assinatura executiva pode aumentar significativamente a profissionalidade e a credibilidade dos seus documentos, criando uma apresentação refinada e polida."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Baixe gratuitamente"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Apresentando o GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "Saiba mais"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) capacita os usuários a incorporar assinaturas de imagem em qualquer local dentro de seus documentos. Esta ferramenta permite que empresas agilizem seus fluxos de trabalho ao adicionar imagens a PDFs, Word, Excel, PowerPoint e formatos de imagem populares, melhorando a eficiência do gerenciamento de documentos.

############################# Steps ############################
steps:
    enable: true
    title: "Guia para adicionar imagens em JPEG usando JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) capacita aplicações Node.js via Java a integrar assinaturas de imagem em documentos JPEG de forma fluida. Amplie as capacidades da sua aplicação com nossa biblioteca abrangente.
      
      1. Instancie Signature com o documento JPEG
      2. Utilize ImageSignOptions para especificar a imagem da assinatura
      3. Posicione a imagem precisamente em qualquer página
      4. Salve o documento assinado no local desejado
   
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

        // Inicialize Signature com o caminho para o documento
        const signature = new signatureLib.Signature('input.jpeg');

        // Configure ImageSignOptions para incluir a assinatura de imagem desejada
        const options = new signatureLib.ImageSignOptions('company_logo.jpg');

        // Coloque a imagem no canto superior esquerdo em todas as páginas
        options.setAllPages(true);
        options.setLeft(100);
        options.setTop(200);
        
        // Salve o documento com a assinatura de imagem aplicada
        const result = signature.sign('output.jpeg', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Capacidades avançadas de assinatura de documentos"
  description: "Nossa API oferece um conjunto de recursos que simplificam a assinatura eletrônica. Você pode adicionar, modificar, remover, procurar e verificar múltiplos tipos de assinaturas, incluindo assinaturas de imagem, com eficiência."
  image: "/img/signature/features_image.webp" # 500x500 px
  image_description: "Assinaturas de imagem"
  features:
    # feature loop
    - title: "Incorpore imagens em documentos de escritório"
      content: "Insira assinaturas de imagem em qualquer lugar do seu documento, seja em PDFs, arquivos Word ou Excel. Melhore seus documentos ao adicionar imagens, códigos de barras, metadados ou certificados digitais para funcionalidade adicional."

    # feature loop
    - title: "Pesquise e valide assinaturas"
      content: "Garanta a autenticidade de seus documentos assinados ao verificar as assinaturas. Utilize a funcionalidade de busca para recuperar e revisar todas as assinaturas incorporadas dentro do seu documento."

    # feature loop
    - title: "Modificar assinaturas existentes"
      content: "Nossa API permite que os usuários atualizem e ajustem assinaturas conforme necessário. Modifique o tamanho, a posição ou outros atributos de qualquer assinatura previamente adicionada para maior flexibilidade no manuseio de documentos."

    # feature loop
    - title: "Remover assinaturas desnecessárias"
      content: "Gerencie seus documentos de forma eficiente removendo assinaturas que não são mais necessárias. Nossa API suporta operações CRUD completas para quase todos os tipos de assinatura."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Melhore documentos com assinaturas de imagem"
      content: |
        Aprenda a incorporar imagens em documentos empresariais para adicionar informações suplementares.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // Selecione o documento a ser assinado
          const signature = new signatureLib.Signature('input.jpeg');

          // Configure as opções da imagem com o caminho da imagem
          const options = new signatureLib.ImageSignOptions('manager_signature.jpg');

          // Ajuste o tamanho da assinatura de imagem
          options.setWidth(100);
          options.setHeight(100);

          // Coloque a imagem no canto inferior direito
          options.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          options.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);

          // Aplique preenchimento nas bordas da página, se necessário
          const padding = new signatureLib.Padding();
          padding.setRight(120);
          padding.setBottom(120);
          options.setMargin(padding);

          // Opcionalmente, adicione uma borda personalizada à imagem
          const border = new signatureLib.Border();
          border.setColor(signatureLib.Color.RED);
          border.setDashStyle(signatureLib.DashStyle.DashDotDot);
          border.setWeight(5);
          border.setVisible(true);
          options.setBorder(border);

          // Gire a assinatura de imagem para melhor aparência
          options.setRotationAngle(45);

          // Salve o documento atualizado no local desejado
          const result = signature.sign('output.jpeg', options);
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
            link: "/examples/signature/formats/signature_image.jpeg"
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
    title: "Descubra as funções que oferecemos"
    exclude: "image"
    description: "Temos o prazer de apresentar uma ampla seleção de métodos e operações de assinatura."
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
    title: "Adicione imagens a vários tipos de arquivo"
    exclude: "JPEG"
    description: "A API Node.js via Java permite que você incorpore imagens em uma ampla gama de formatos de documentos. Personalize o tamanho, a colocação e o posicionamento na página para aprimorar seu processo de assinatura de documentos."
    items: 
          
        # format loop 1
        - name: "Assinar PDF com imagem"
          format: "PDF"
          link: "/signature/nodejs-java/image/pdf/"
          description: "Formato de Documento Portátil Adobe"
          
        # format loop 2
        - name: "Assinar DOCX com imagem"
          format: "DOCX"
          link: "/signature/nodejs-java/image/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 3
        - name: "Assinar JPEG com imagem"
          format: "JPEG"
          link: "/signature/nodejs-java/image/jpeg/"
          description: "Imagem JPEG"
          
        # format loop 4
        - name: "Assinar PPTX com imagem"
          format: "PPTX"
          link: "/signature/nodejs-java/image/pptx/"
          description: "Apresentação PowerPoint Open XML"
          
        # format loop 5
        - name: "Assinar XLSX com imagem"
          format: "XLSX"
          link: "/signature/nodejs-java/image/xlsx/"
          description: "Planilha Microsoft Excel Open XML"


          

---