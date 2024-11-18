



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:47
draft: false
lang: pt
format: Docx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Selos redondos e quadrados DOCX via C#"
head_description: "Use GroupDocs.Signature for .NET para gerar e incorporar selos personalizados em arquivos DOCX."

############################# Header ############################
title: "Gere selos para arquivos DOCX" 
description: "Integre perfeitamente selos projetados sob medida em qualquer seção de seus documentos usando GroupDocs.Signature for .NET, oferecendo flexibilidade extensiva para a colocação e configuração dos selos conforme suas necessidades comerciais."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Baixe sua versão gratuita"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "Visão Geral do GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "Saiba mais"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) é uma ferramenta versátil que permite a inserção de múltiplos tipos de assinatura em documentos, incluindo selos personalizáveis. Suportando mais de 60 formatos de arquivo, de PDFs e documentos do Word a imagens e arquivos ZIP, você pode enriquecer seus documentos com texto, imagens, códigos de barras, metadados, certificados digitais e selos. Além disso, você tem total controle para pesquisar, validar, modificar ou remover qualquer assinatura aplicada aos seus arquivos.

############################# Steps ############################
steps:
    enable: true
    title: "Como incorporar um selo em DOCX usando C#"
    content: |
      [GroupDocs.Signature](/signature/net/) oferece uma robusta funcionalidade de criação de selos, ideal para aprimorar aplicações .NET. Aproveite essa ferramenta para criar e implementar selos altamente personalizados em suas páginas de documentos.
      
      1. Forneça o documento DOCX a ser selado.
      2. Utilize StampSignOptions para configurar meticulosamente todos os parâmetros necessários.
      3. Adicione múltiplas linhas de selo conforme suas necessidades.
      4. Aplique o selo configurado e salve o documento modificado.
   
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
        // Integre o caminho do documento com a instância Signature
        using (Signature signature = new Signature("input.docx"))
        {
            // Inicialize StampSignOptions com o conteúdo de assinatura necessário
            StampSignOptions options = new StampSignOptions();
            options.Height = 180;
            options.Width = 180;

            // Incorpore uma ou várias linhas de selos
            options.OuterLines.Add(
                new StampLine()
                {
                    Text = "* The Best Company *",
                    TextRepeatType = StampTextRepeatType.FullTextRepeat,
                    Font = new SignatureFont() { Size = 12, FamilyName = "Arial" },
                    Height = 22,
                    TextBottomIntent = 6,
                    TextColor = Color.WhiteSmoke,
                    BackgroundColor = Color.DarkSlateBlue
                }
            );

            // Preserve o documento com o selo aplicado
            SignResult result = signature.Sign("output.docx", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Aproveite as assinaturas para garantir e melhorar a integridade dos documentos"
  description: "Com a biblioteca GroupDocs.Signature for .NET, você pode integrar a funcionalidade de assinatura em seus documentos. Adicione, modifique, verifique ou remova facilmente selos personalizados e outros tipos de assinatura, oferecendo flexibilidade e precisão para a gestão segura de documentos."
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "Assinaturas de Selo Powered by GroupDocs.Signature"
  features:
    # feature loop
    - title: "Assinatura de documentos abrangente"
      content: "Melhore seus documentos colocando assinaturas, incluindo texto, imagens, códigos de barras, códigos QR e selos, em qualquer posição ou página dentro do arquivo. Além disso, gerencie metadados incorporados e aplique certificados digitais para proteger contra alterações não autorizadas."

    # feature loop
    - title: "Busca e validação de assinatura eficientes"
      content: "Após a assinatura, verifique a autenticidade e integridade das assinaturas do documento. Utilize funcionalidades de busca avançada para recuperar e gerenciar todos os dados de assinatura incorporados no documento."

    # feature loop
    - title: "Modificar e personalizar assinaturas"
      content: "Ajuste assinaturas previamente inseridas com precisão. Se você precisar mudar o conteúdo, posição, tamanho ou cor, nossa solução oferece total flexibilidade para modificação de assinaturas."

    # feature loop
    - title: "Remova assinaturas sem esforço"
      content: "Quando assinaturas precisam ser removidas, GroupDocs.Signature for .NET fornece um conjunto completo de ferramentas para deletar qualquer tipo de assinatura, incluindo selos, certificados digitais e mais, garantindo que seus documentos permaneçam atualizados e em conformidade."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Implemente selos personalizados em documentos"
      content: |
        Descubra como elaborar e integrar selos personalizados contendo informações textuais críticas em seus documentos.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Forneça o documento a ser selado
          using (Signature signature = new Signature("input.docx"))
          {
              // Inicialize as opções de selo com as configurações desejadas
              StampSignOptions options = new StampSignOptions()
              {
                    // Defina as dimensões e a posição do selo na página
                    Height = 200,
                    Width = 200,
                    VerticalAlignment = VerticalAlignment.Bottom,
                    HorizontalAlignment = HorizontalAlignment.Right,
                    AllPages = true
              };

              // Incorpore linhas circulares externas com texto
              options.OuterLines.Add(
                    new StampLine()
                    {
                        Text = "* The best  choice *",
                        TextRepeatType = StampTextRepeatType.FullTextRepeat,
                        Font = new SignatureFont() { Size = 12, FamilyName = "Arial" },
                        Height = 22,
                        TextBottomIntent = 6,
                        TextColor = Color.WhiteSmoke,
                        BackgroundColor = Color.DarkSlateBlue
                    }
              );

              // Integre linhas quadradas internas, se necessário
              options.InnerLines.Add(
                    new StampLine()
                    { 
                        Text = "Company #1",
                        TextColor = Color.MediumVioletRed,
                        Font = new SignatureFont() { Size = 20, Bold = true },
                        Height = 40
                    }
              );

              // Finalize e salve o documento selado
              SignResult result = signature.Sign("output.docx", options);
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
            link: "/examples/signature/formats/signature_stamp.docx"
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
    title: "Explore funcionalidades essenciais"
    exclude: "stamp"
    description: "Descubra uma ampla gama de opções para criar, gerenciar e deletar diversos tipos de assinaturas, garantindo controle abrangente sobre seus fluxos de trabalho de documentos."
    items: 
          
        # operation loop 1
        - name: "Assinaturas eletrônicas"
          operation: "esign"
          link: "/signature/net/esign/docx/"
          description: "Adicionar vários tipos de assinaturas a formatos de arquivo suportados"

        # operation loop 2
        - name: "Adicionar texto a documentos"
          operation: "text"
          link: "/signature/net/text/docx/"
          description: "Melhore o conteúdo do documento com assinaturas de texto personalizáveis"

        # operation loop 3
        - name: "Assinaturas de imagem"
          operation: "image"
          link: "/signature/net/image/docx/"
          description: "Colocar qualquer imagem em qualquer posição dentro de um documento"

        # operation loop 4
        - name: "Gerar códigos de barras"
          operation: "barcode"
          link: "/signature/net/barcode/docx/"
          description: "Criar e inserir vários códigos de barras em documentos suportados"

        # operation loop 5
        - name: "Gerar QR codes"
          operation: "qrcode"
          link: "/signature/net/qrcode/docx/"
          description: "Gerar e QR Codes, incluindo códigos QR, para assinatura de documentos"
          
        # operation loop 6
        - name: "Certificados digitais"
          operation: "digital"
          link: "/signature/net/digital/docx/"
          description: "Proteger negócios e assinar documentos com certificados digitais"

        # operation loop 7
        - name: "Assinaturas de carimbo"
          operation: "stamp"
          link: "/signature/net/stamp/docx/"
          description: "Use o Construtor de Carimbos para criar carimbos redondos ou quadrados personalizados"
          
        # operation loop 8
        - name: "Buscar assinaturas"
          operation: "search"
          link: "/signature/net/search/docx/"
          description: "Localizar quaisquer assinaturas previamente adicionadas em um documento"
          
        # operation loop 9
        - name: "Verificação de assinaturas"
          operation: "verify"
          link: "/signature/net/verify/docx/"
          description: "Verificar a autenticidade das assinaturas após a aplicação"
          
        # operation loop 10
        - name: "Modificar assinaturas"
          operation: "modify"
          link: "/signature/net/modify/docx/"
          description: "Editar uma variedade de assinaturas dentro de um documento"
          
        # operation loop 11
        - name: "Excluir assinaturas"
          operation: "delete"
          link: "/signature/net/delete/docx/"
          description: "Remover uma ampla gama de assinaturas previamente aplicadas"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Aplique selos em diversos formatos de documento"
    exclude: "DOCX"
    description: "A API GroupDocs.Signature permite que você incorpore selos em mais de 60 tipos de arquivos padrão da indústria. Aplique facilmente selos personalizados em qualquer local dentro de seus documentos, permitindo maior rastreamento e personalização dos documentos."
    items: 
          
        # format loop 1
        - name: "Carimbar PDF"
          format: "PDF"
          link: "/signature/net/stamp/pdf/"
          description: "Formato de Documento Portátil Adobe"
          
        # format loop 2
        - name: "Carimbar DOCX"
          format: "DOCX"
          link: "/signature/net/stamp/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 3
        - name: "Carimbar JPEG"
          format: "JPEG"
          link: "/signature/net/stamp/jpeg/"
          description: "Imagem JPEG"
          
        # format loop 4
        - name: "Carimbar PPTX"
          format: "PPTX"
          link: "/signature/net/stamp/pptx/"
          description: "Apresentação PowerPoint Open XML"
          
        # format loop 5
        - name: "Carimbar XLSX"
          format: "XLSX"
          link: "/signature/net/stamp/xlsx/"
          description: "Planilha Microsoft Excel Open XML"


          

---