



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:25
draft: false
lang: pt
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Gerar código de barras para JPEG usando a API C#"
head_description: "Gere uma assinatura de código de barras e proteja documentos JPEG usando C# com apenas algumas linhas de código. Utilize GroupDocs.Signature para assinar uma ampla variedade de formatos de arquivo."

############################# Header ############################
title: "Gerar código de barras para documentos JPEG" 
description: "Utilize GroupDocs.Signature for .NET para colocar códigos de barras em qualquer lugar dentro dos seus documentos comerciais. Nossa API oferece amplas opções de personalização para assinaturas de código de barras."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Baixar gratuitamente"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "Visão geral do GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "Saiba mais"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) é uma solução avançada para assinatura de documentos que suporta uma vasta gama de tipos de assinatura, incluindo texto, imagens, códigos de barras, certificados digitais e carimbos. Compatível com mais de 60 formatos de arquivo — como PDF, MS Office, imagens, arquivos ZIP e muito mais — esta ferramenta permite não apenas aplicar assinaturas, mas também pesquisar, verificar, modificar ou removê-las conforme necessário.

############################# Steps ############################
steps:
    enable: true
    title: "Passos para gerar e embutir um código de barras em arquivo JPEG"
    content: |
      [GroupDocs.Signature](/signature/net/) facilita a geração de códigos de barras em numerosos formatos populares e sua colocação em páginas de JPEG. Suportando mais de 60 tipos de códigos de barras, aplicações .NET podem ser facilmente ampliadas com funcionalidades de assinatura de código de barras integrando nossa biblioteca.
      
      1. Forneça o arquivo JPEG ou fluxo para processamento.
      2. Passe o texto do código de barras para a instância de BarcodeSignOptions.
      3. Personalize as opções do código de barras, como posição, tamanho, etc.
      4. Salve o arquivo com o código de barras recém-adicionado.
   
    code:
      platform: "net"
      copy_title: "Copiar"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Assinaturas de exemplo"
      install:
        command: "dotnet add package GroupDocs.Signature"
        copy_tip: "clique para copiar"
        copy_done: "copiado"
      links:
        #  loop
        - title: "Mais exemplos"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET/"
        #  loop
        - title: "Documentação"
          link: "https://docs.groupdocs.com/signature/net/"
          
      content: |
        ```csharp {style=abap}
        // Instanciar um novo objeto Signature com o caminho do documento
        using (Signature signature = new Signature("input.jpeg"))
        {
            // Utilizar BarcodeSignOptions para adicionar um código de barras ao documento
            BarcodeSignOptions options = new BarcodeSignOptions("Business data")
            {
                // Configurar o tipo de código de barras e propriedades adicionais
                EncodeType = BarcodeTypes.Code128,
                Left = 50,
                Top = 150
            };

            // Salvar o arquivo assinado
            SignResult result = signature.Sign("output.jpeg", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Melhore e proteja seus documentos com capacidades avançadas de assinatura"
  description: "A biblioteca GroupDocs.Signature for .NET é projetada para facilitar a assinatura e o processamento abrangentes de documentos em formatos amplamente utilizados. Você pode rapidamente adicionar, ajustar, verificar ou remover diferentes tipos de assinaturas."
  image: "/img/signature/features_barcode.webp" # 500x500 px
  image_description: "Recursos Chave do GroupDocs.Signature"
  features:
    # feature loop
    - title: "Assinatura de documentos versátil"
      content: "Assine eficientemente qualquer página dentro de documentos suportados usando texto, imagens, códigos de barras, códigos QR ou carimbos. Além disso, insira metadados ocultos, como dados EXIF em imagens, ou proteja o conteúdo do seu documento contra alterações não autorizadas usando certificados digitais."

    # feature loop
    - title: "Pesquisa e verificação de assinatura abrangentes"
      content: "Nossa ferramenta oferece funcionalidades robustas para trabalhar com documentos assinados. Assegure a integridade de seus documentos verificando assinaturas e recupere facilmente uma lista abrangente de todas as assinaturas dentro de um documento através da nossa funcionalidade de busca."

    # feature loop
    - title: "Edição de assinaturas com facilidade"
      content: "Quase todas as assinaturas aplicadas anteriormente podem ser modificadas. Atualize convenientemente o texto, ajuste a posição ou altere as cores conforme suas necessidades."

    # feature loop
    - title: "Efeito de exclusão de assinatura eficiente"
      content: "Nossa abordagem suporta totalmente operações CRUD para assinaturas, permitindo a remoção rápida de quaisquer assinaturas indesejadas ou desatualizadas de seus documentos."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Como gerar uma assinatura de código de barras"
      content: |
        Este exemplo mostra como embutir um código de barras personalizado nas páginas do documento JPEG.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          using (Signature signature = new Signature("input.jpeg"))
          {
              // Elabore opções de assinatura com o texto desejado
              BarcodeSignOptions options = new BarcodeSignOptions("Accepted")
              {
                  EncodeType = BarcodeTypes.Code39FullASCII,

                  // Determine a posição relativa do código de barras na página
                  VerticalAlignment = Domain.VerticalAlignment.Top,
                  HorizontalAlignment = Domain.HorizontalAlignment.Left,

                  // Defina a margem do código de barras em relação à borda da página
                  Margin = new Padding() { Top = 180, Right = 20 },

                  // Especifique a cor das barras
                  ForeColor = Color.Red,

                  // Selecione o estilo da fonte da mensagem
                  Font = new SignatureFont { Size = 12, FamilyName = "Arial" },

                  // Indique a posição da mensagem
                  CodeTextAlignment = CodeTextAlignment.Above
              };

              // Assine e salve o documento
              SignResult result = signature.Sign("output.jpeg", options);
          }
          ```
        platform: "net"
        copy_title: "Copiar"
        install:
          command: "dotnet add package GroupDocs.Signature"
          copy_tip: "clique para copiar"
          copy_done: "copiado"
        top_links:
          #  loop
          - title: "Baixar resultado"
            icon: "download"
            link: "/examples/signature/formats/signature_barcode.jpeg"
        links:
          #  loop
          - title: "Mais exemplos"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET/"
          #  loop
          - title: "Documentação"
            link: "https://docs.groupdocs.com/signature/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Pronto para começar?"
  description: "Experimente os recursos do GroupDocs.Signature gratuitamente ou solicite uma licença"
  items:
    #  loop
    - title: "Baixar Nuget"
      link: "https://releases.groupdocs.com/signature/net/"
      color: "red"
        #  loop
    - title: "Licenciamento"
      link: "https://purchase.groupdocs.com/pricing/signature/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Descubra nossos principais recursos"
    exclude: "barcode"
    description: "Oferecemos uma impressionante seleção de opções de assinatura e operações."
    items: 
          
        # operation loop 1
        - name: "Assinaturas eletrônicas"
          operation: "esign"
          link: "/signature/net/esign/jpeg/"
          description: "Adicionar vários tipos de assinaturas a formatos de arquivo suportados"

        # operation loop 2
        - name: "Adicionar texto a documentos"
          operation: "text"
          link: "/signature/net/text/jpeg/"
          description: "Melhore o conteúdo do documento com assinaturas de texto personalizáveis"

        # operation loop 3
        - name: "Assinaturas de imagem"
          operation: "image"
          link: "/signature/net/image/jpeg/"
          description: "Colocar qualquer imagem em qualquer posição dentro de um documento"

        # operation loop 4
        - name: "Gerar códigos de barras"
          operation: "barcode"
          link: "/signature/net/barcode/jpeg/"
          description: "Criar e inserir vários códigos de barras em documentos suportados"

        # operation loop 5
        - name: "Gerar QR codes"
          operation: "qrcode"
          link: "/signature/net/qrcode/jpeg/"
          description: "Gerar e QR Codes, incluindo códigos QR, para assinatura de documentos"
          
        # operation loop 6
        - name: "Certificados digitais"
          operation: "digital"
          link: "/signature/net/digital/pdf/"
          description: "Proteger negócios e assinar documentos com certificados digitais"

        # operation loop 7
        - name: "Assinaturas de carimbo"
          operation: "stamp"
          link: "/signature/net/stamp/jpeg/"
          description: "Use o Construtor de Carimbos para criar carimbos redondos ou quadrados personalizados"
          
        # operation loop 8
        - name: "Buscar assinaturas"
          operation: "search"
          link: "/signature/net/search/pdf/"
          description: "Localizar quaisquer assinaturas previamente adicionadas em um documento"
          
        # operation loop 9
        - name: "Verificação de assinaturas"
          operation: "verify"
          link: "/signature/net/verify/pdf/"
          description: "Verificar a autenticidade das assinaturas após a aplicação"
          
        # operation loop 10
        - name: "Modificar assinaturas"
          operation: "modify"
          link: "/signature/net/modify/pdf/"
          description: "Editar uma variedade de assinaturas dentro de um documento"
          
        # operation loop 11
        - name: "Excluir assinaturas"
          operation: "delete"
          link: "/signature/net/delete/pdf/"
          description: "Remover uma ampla gama de assinaturas previamente aplicadas"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Assine documentos em uma variedade de formatos"
    exclude: "JPEG"
    description: "Nossa API .NET suporta a assinatura de mais de 60 formatos diferentes. Coloque facilmente vários tipos de assinaturas em qualquer página ou na posição desejada dentro de seus documentos."
    items: 
          
        # format loop 1
        - name: "Adicionar código de barras ao PDF"
          format: "PDF"
          link: "/signature/net/barcode/pdf/"
          description: "Formato de Documento Portátil Adobe"
          
        # format loop 2
        - name: "Adicionar código de barras ao DOCX"
          format: "DOCX"
          link: "/signature/net/barcode/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 3
        - name: "Adicionar código de barras ao JPEG"
          format: "JPEG"
          link: "/signature/net/barcode/jpeg/"
          description: "Imagem JPEG"
          
        # format loop 4
        - name: "Adicionar código de barras ao PPTX"
          format: "PPTX"
          link: "/signature/net/barcode/pptx/"
          description: "Apresentação PowerPoint Open XML"
          
        # format loop 5
        - name: "Adicionar código de barras ao XLSX"
          format: "XLSX"
          link: "/signature/net/barcode/xlsx/"
          description: "Planilha Microsoft Excel Open XML"


          

---