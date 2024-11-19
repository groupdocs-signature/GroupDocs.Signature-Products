



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:09
draft: false
lang: pt
format: Docx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Adicionar assinaturas de imagem a arquivos DOCX com C#"
head_description: "Adicione uma assinatura de imagem em arquivo DOCX para .NET usando algumas linhas de código. Use a API GroupDocs.Signature for .NET para adicionar imagens."

############################# Header ############################
title: "Adicione assinatura de imagem a arquivos DOCX" 
description: "Utilize GroupDocs.Signature for .NET para integrar imagens de forma eficiente em diversos formatos de documentos de escritório, incluindo PDFs, Word, Excel e arquivos de imagem. Incorporar uma imagem da assinatura do seu chefe pode criar uma impressão profissional marcante, elevando o apelo visual e a autenticidade dos seus documentos."
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
    title: "Descubra GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "Saiba mais"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) oferece capacidades abrangentes para embutir assinaturas de imagem em qualquer local de qualquer página dos seus documentos de negócios. Aprimore seus fluxos operacionais integrando imagens em PDFs, documentos Word, planilhas Excel, apresentações PowerPoint e uma variedade de formatos populares de imagem através da nossa biblioteca robusta.

############################# Steps ############################
steps:
    enable: true
    title: "Como adicionar uma imagem em qualquer lugar de um DOCX usando C#"
    content: |
      Aproveite [GroupDocs.Signature](/signature/net/) para capacitar aplicações .NET com a habilidade de embutir assinaturas com precisão em qualquer página de documentos DOCX. Melhore as capacidades do seu produto de forma integrada com nossa solução.
      
      1. Instancie a classe Signature com o documento DOCX.
      2. Utilize ImageSignOptions para especificar a imagem da assinatura.
      3. Posicione a imagem com precisão em qualquer local desejado da página.
      4. Salve o documento recém-assinado em um local especificado.
   
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
        // Inicialize Signature com o caminho para o documento
        using (Signature signature = new Signature("input.docx"))
        {
            // Configure ImageSignOptions usando uma imagem para a assinatura
            ImageSignOptions options = new ImageSignOptions("company_logo.jpg")
            {
                // Posicione a imagem no canto superior esquerdo de todas as páginas
                AllPages = true,
                Left = 100,
                Top = 200
            };

            // Salve o documento assinado
            SignResult result = signature.Sign("output.docx", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Soluções abrangentes para assinatura de documentos"
  description: "Temos o prazer de apresentar uma ampla gama de funcionalidades de assinatura suportadas pela nossa API. Adicione, modifique, exclua, busque e verifique diferentes tipos de assinaturas, incluindo assinaturas baseadas em imagem, de forma simples."
  image: "/img/signature/features_image.webp" # 500x500 px
  image_description: "Assinatura de Imagem"
  features:
    # feature loop
    - title: "Embutir imagens em documentos de escritório"
      content: "Insira assinaturas eletrônicas e imagens sem interrupções em qualquer posição designada em qualquer página de um documento. Melhore o conteúdo do seu documento com textos, imagens, códigos de barras, metadados ou certificados digitais para aumentar a funcionalidade e a segurança."

    # feature loop
    - title: "Busca e verificação de assinaturas"
      content: "Gerencie documentos assinados verificando a autenticidade e integridade das assinaturas. Recupere uma lista abrangente de todas as assinaturas dentro de um documento e examine seus atributos específicos."

    # feature loop
    - title: "Modificar assinaturas"
      content: "Eventualmente, as assinaturas nos documentos podem precisar de atualizações. Ajuste o conteúdo, a aparência, o tamanho ou a posição das assinaturas existentes para atender às exigências em evolução."

    # feature loop
    - title: "Remover assinaturas redundantes"
      content: "Nossa API facilita operações completas de CRUD para a maioria dos tipos de assinaturas. Você pode remover eficientemente assinaturas de quase todos os formatos de documento suportados quando necessário."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Proteja o conteúdo do documento com assinaturas de imagem"
      content: |
        Descubra como enriquecer documentos comerciais embutindo imagens, fornecendo informações complementares.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Selecione o documento a ser assinado
          using (Signature signature = new Signature("input.docx"))
          {
              // Crie opções de imagem com o caminho da imagem especificado
              ImageSignOptions options = new ImageSignOptions("manager_signature.jpg")
              {
                    // Defina as dimensões da assinatura da imagem
                    Width = 100,
                    Height = 100,

                    // Posicione a imagem no canto inferior direito
                    VerticalAlignment = VerticalAlignment.Bottom,
                    HorizontalAlignment = HorizontalAlignment.Right,

                    // Aplique o preenchimento necessário a partir das bordas da página
                    Margin = new Padding() { Bottom = 120, Right = 120 },

                    // Opcionalmente, adicione uma borda personalizada à imagem
                    Border = new Border()
                    {
                        Visible = true,
                        Color = Color.Red,
                        DashStyle = DashStyle.DashDotDot,
                        Weight = 5
                    },

                    // Gire a assinatura para alinhamento ideal
                    RotationAngle = 45
              };

              // Salve o documento atualizado no local desejado
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
            link: "/examples/signature/formats/signature_image.docx"
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
    title: "Entenda nossas ofertas de recursos"
    exclude: "image"
    description: "Explore um conjunto diversificado de tipos de assinaturas e operações robustas fornecidas pela nossa plataforma."
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
    title: "Integre imagens em diversos formatos de arquivo"
    exclude: "DOCX"
    description: "Aproveite a API .NET para adicionar formatos de imagem suportados a uma extensa gama de documentos. Redimensione, posicione, selecione páginas específicas e aplique assinaturas baseadas em imagem aos seus documentos com facilidade."
    items: 
          
        # format loop 1
        - name: "Assinar PDF com imagem"
          format: "PDF"
          link: "/signature/net/image/pdf/"
          description: "Formato de Documento Portátil Adobe"
          
        # format loop 2
        - name: "Assinar DOCX com imagem"
          format: "DOCX"
          link: "/signature/net/image/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 3
        - name: "Assinar JPEG com imagem"
          format: "JPEG"
          link: "/signature/net/image/jpeg/"
          description: "Imagem JPEG"
          
        # format loop 4
        - name: "Assinar PPTX com imagem"
          format: "PPTX"
          link: "/signature/net/image/pptx/"
          description: "Apresentação PowerPoint Open XML"
          
        # format loop 5
        - name: "Assinar XLSX com imagem"
          format: "XLSX"
          link: "/signature/net/image/xlsx/"
          description: "Planilha Microsoft Excel Open XML"


          

---