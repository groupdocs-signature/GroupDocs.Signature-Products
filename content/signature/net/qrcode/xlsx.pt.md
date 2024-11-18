



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:02
draft: false
lang: pt
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Gere código QR para arquivos XLSX usando C#"
head_description: "Aproveite a API GroupDocs.Signature para gerar código QR para arquivos XLSX. Integre códigos QR em qualquer página para funcionalidade aprimorada."

############################# Header ############################
title: "Gere códigos QR para XLSX" 
description: "Gere códigos de barras 2D utilizando dados textuais ou numéricos e aplique-os em várias páginas e formatos, incluindo PDFs, Word, Excel e mais, através do GroupDocs.Signature for .NET."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Inicie seu teste gratuito"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "Descubra as capacidades do GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "Saiba mais"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) oferece uma ampla gama de recursos, permitindo que os usuários gerem e integrem vários tipos de assinatura em formatos de documento líderes. Seja em PDFs, documentos Word, planilhas Excel, apresentações PowerPoint ou arquivos de imagem, você pode aprimorar seus documentos com assinaturas de Texto, Imagem, Código de Barras, Código QR, Metadados, Digital e Carimbo.

############################# Steps ############################
steps:
    enable: true
    title: "Como gerar e inserir um código QR em qualquer lugar dentro de um XLSX"
    content: |
      [GroupDocs.Signature](/signature/net/) facilita a geração de códigos QR em vários formatos populares e sua colocação em páginas de XLSX. Com suporte a mais de 10 tipos de códigos QR, nossa biblioteca pode ser integrada facilmente em aplicações .NET. Aprimore seus documentos com assinaturas de código QR utilizando nosso produto.
      
      1. Adquira o arquivo ou fluxo XLSX a ser assinado com um código QR.
      2. Forneça o texto necessário para QrCodeSignOptions.
      3. Personalize parâmetros visuais como cor, posição, tamanho etc.
      4. Persistir o documento com o código QR embutido.
   
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
        // Inicialize uma nova instância de Signature com o documento
        using (Signature signature = new Signature("input.xlsx"))
        {
            // Utilize QrCodeSignOptions para integrar um código QR no documento
            QrCodeSignOptions options = new QrCodeSignOptions("Text Content")
                {
                    // Especifique o tipo de assinatura e denote sua posição na página
                    EncodeType = QrCodeTypes.QR,
                    Left = 50,
                    Top = 150
                };

            // Persistir o documento com o código QR integrado
            SignResult result = signature.Sign("output.xlsx", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Integração abrangente de assinaturas para documentos"
  description: "Com a API GroupDocs.Signature for .NET, os usuários podem gerar, modificar, pesquisar, validar e remover uma variedade de tipos de assinatura, otimizando os fluxos de trabalho documentais com precisão incomparável."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "Recursos Principais do GroupDocs.Signature"
  features:
    # feature loop
    - title: "Assinatura de documentos com múltiplos tipos de assinatura"
      content: "GroupDocs.Signature permite a aplicação de assinaturas de Texto, Imagem, Código de Barras, Código QR e Carimbo em qualquer formato de documento. As assinaturas podem ser posicionadas com precisão em qualquer página, e os metadados podem ser gerenciados de forma eficiente através de assinaturas de metadados. Proteja a integridade de seus documentos incorporando certificados digitais que evitam alterações não autorizadas."

    # feature loop
    - title: "Pesquisa e validação de assinaturas"
      content: "Verifique a autenticidade e a precisão das assinaturas documentais através de um processo de validação avançado. Recupere facilmente uma lista detalhada de todas as assinaturas integradas em um documento para supervisão abrangente."

    # feature loop
    - title: "Modificação de assinatura personalizável"
      content: "Atualize e refine assinaturas previamente aplicadas ajustando conteúdo, posicionamento, cor, tamanho e outros atributos para atender às suas necessidades específicas."

    # feature loop
    - title: "Remoção eficiente de assinaturas"
      content: "Otimize sua gestão documental removendo programaticamente assinaturas indesejadas. Seja lidando com certificados digitais ou outros tipos de assinatura, a remoção pode ser realizada de maneira rápida e eficaz."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Como gerar um código QR com várias opções?"
      content: |
        Este exemplo demonstra como posicionar um código QR personalizado em uma página XLSX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Recupere o documento a ser assinado e passe-o para Signature
          using (Signature signature = new Signature("input.xlsx"))
          {
              // Configure opções de código QR com o texto necessário
              QrCodeSignOptions options = new QrCodeSignOptions("Archived on July 11, 2019")
              {
                    // Determine a posição relativa do código QR na página
                    VerticalAlignment = Domain.VerticalAlignment.Top,
                    HorizontalAlignment = Domain.HorizontalAlignment.Right,

                    // Defina o preenchimento da assinatura
                    Margin = new Padding() { Top = 20, Right = 20 },

                    // Especifique a cor do código QR
                    ForeColor = Color.Red,

                    // Defina as opções de fonte para a mensagem
                    Font = new SignatureFont { Size = 12, FamilyName = "Comic Sans MS" },

                    // Personalize a cor de fundo e o pincel do código QR
                    Background = new Background()
                    {
                        Color = Color.LimeGreen,
                        Transparency = 0.5,
                        Brush = new Domain.Extensions.LinearGradientBrush(Color.LimeGreen, Color.DarkGreen)
                    }
              };

              // Incorpore o código QR no documento
              SignResult result = signature.Sign("output.xlsx", options);
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
            link: "/examples/signature/formats/signature_qrcode.xlsx"
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
    title: "Saiba mais sobre nossas soluções de assinatura"
    exclude: "qrcode"
    description: "Apresentamos com orgulho uma ampla gama de tipos de assinatura e recursos operacionais."
    items: 
          
        # operation loop 1
        - name: "Assinaturas eletrônicas"
          operation: "esign"
          link: "/signature/net/esign/xlsx/"
          description: "Adicionar vários tipos de assinaturas a formatos de arquivo suportados"

        # operation loop 2
        - name: "Adicionar texto a documentos"
          operation: "text"
          link: "/signature/net/text/xlsx/"
          description: "Melhore o conteúdo do documento com assinaturas de texto personalizáveis"

        # operation loop 3
        - name: "Assinaturas de imagem"
          operation: "image"
          link: "/signature/net/image/xlsx/"
          description: "Colocar qualquer imagem em qualquer posição dentro de um documento"

        # operation loop 4
        - name: "Gerar códigos de barras"
          operation: "barcode"
          link: "/signature/net/barcode/xlsx/"
          description: "Criar e inserir vários códigos de barras em documentos suportados"

        # operation loop 5
        - name: "Gerar QR codes"
          operation: "qrcode"
          link: "/signature/net/qrcode/xlsx/"
          description: "Gerar e QR Codes, incluindo códigos QR, para assinatura de documentos"
          
        # operation loop 6
        - name: "Certificados digitais"
          operation: "digital"
          link: "/signature/net/digital/xlsx/"
          description: "Proteger negócios e assinar documentos com certificados digitais"

        # operation loop 7
        - name: "Assinaturas de carimbo"
          operation: "stamp"
          link: "/signature/net/stamp/xlsx/"
          description: "Use o Construtor de Carimbos para criar carimbos redondos ou quadrados personalizados"
          
        # operation loop 8
        - name: "Buscar assinaturas"
          operation: "search"
          link: "/signature/net/search/xlsx/"
          description: "Localizar quaisquer assinaturas previamente adicionadas em um documento"
          
        # operation loop 9
        - name: "Verificação de assinaturas"
          operation: "verify"
          link: "/signature/net/verify/xlsx/"
          description: "Verificar a autenticidade das assinaturas após a aplicação"
          
        # operation loop 10
        - name: "Modificar assinaturas"
          operation: "modify"
          link: "/signature/net/modify/xlsx/"
          description: "Editar uma variedade de assinaturas dentro de um documento"
          
        # operation loop 11
        - name: "Excluir assinaturas"
          operation: "delete"
          link: "/signature/net/delete/xlsx/"
          description: "Remover uma ampla gama de assinaturas previamente aplicadas"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Gere códigos QR para outros formatos de documento"
    exclude: "XLSX"
    description: "Aprimore todos os formatos de arquivo padrão da indústria com a capacidade de integrar códigos QR através da API .NET. Armazene e codifique informações críticas em códigos de barras 2D para escaneamento e recuperação de dados sem interrupções."
    items: 
          
        # format loop 1
        - name: "QR-Code para PDF"
          format: "PDF"
          link: "/signature/net/qrcode/pdf/"
          description: "Formato de Documento Portátil Adobe"
          
        # format loop 2
        - name: "QR-Code para DOCX"
          format: "DOCX"
          link: "/signature/net/qrcode/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 3
        - name: "QR-Code para JPEG"
          format: "JPEG"
          link: "/signature/net/qrcode/jpeg/"
          description: "Imagem JPEG"
          
        # format loop 4
        - name: "QR-Code para PPTX"
          format: "PPTX"
          link: "/signature/net/qrcode/pptx/"
          description: "Apresentação PowerPoint Open XML"
          
        # format loop 5
        - name: "QR-Code para XLSX"
          format: "XLSX"
          link: "/signature/net/qrcode/xlsx/"
          description: "Planilha Microsoft Excel Open XML"


          

---