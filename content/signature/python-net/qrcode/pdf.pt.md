



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:22
draft: false
lang: pt
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Gere códigos QR para arquivos PDF usando Python"
head_description: "Use a API GroupDocs.Signature para gerar e incorporar códigos QR em arquivos PDF. Coloque códigos QR em qualquer página para adicionar funcionalidade extra."

############################# Header ############################
title: "Gere códigos QR para PDF" 
description: "Crie códigos de barras 2D a partir de dados textuais ou numéricos e aplique-os em várias páginas e formatos, incluindo PDFs, Word, Excel e mais, com GroupDocs.Signature for Python via .NET."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Teste grátis"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "Explore os recursos do GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "Saiba mais"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) oferece uma ampla gama de capacidades, permitindo aos usuários gerar e incorporar diferentes tipos de assinatura em formatos de documentos principais. Seja em PDFs, Word, Excel, PowerPoint ou imagens, melhore seus documentos com assinaturas de Texto, Imagem, Código de Barras, Código QR, Metadados, Digital ou Selo.

############################# Steps ############################
steps:
    enable: true
    title: "Passos para gerar e inserir um código QR em PDF"
    content: |
      [GroupDocs.Signature](/signature/python-net/) permite que você crie códigos QR em formatos populares e os coloque em páginas PDF. Com suporte a mais de 10 tipos de código QR, você pode integrar essa funcionalidade em aplicações Python via .NET. Melhore seus documentos com assinaturas de código QR usando nosso produto.
      
      1. Obtenha o arquivo ou stream PDF onde o código QR será adicionado.
      2. Forneça o texto necessário para QrCodeSignOptions.
      3. Personalize configurações visuais como cor, posição e tamanho.
      4. Salve o documento com o código QR incorporado.
   
    code:
      platform: "python-net"
      copy_title: "Copiar"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Assinaturas de exemplo"
      install:
        command: "pip install groupdocs-signature-net"
        copy_tip: "clique para copiar"
        copy_done: "copiado"
      links:
        #  loop
        - title: "Mais exemplos"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Python-via-.NET/"
        #  loop
        - title: "Documentação"
          link: "https://docs.groupdocs.com/signature/python-net/"
          
      content: |
        ```python {style=abap}
        import groupdocs.signature as sg

        def run():

            # Inicialize uma nova instância de Signature com o documento
            with sg.Signature('input.pdf') as signature:

                # Use QrCodeSignOptions para incorporar um código QR no documento
                options = sg.QrCodeSignOptions("Text Content")

                # Especifique o tipo de assinatura e defina sua posição na página
                options.EncodeType = sg.QrCodeTypes.QR
                options.Left = 50
                options.Top = 150

                # Salve o documento com o código QR incorporado
                result = signature.Sign("output.pdf", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Integração completa de assinatura para documentos"
  description: "Com a API GroupDocs.Signature for Python via .NET, os usuários podem gerar, modificar, pesquisar, validar e remover diferentes tipos de assinatura, simplificando fluxos de trabalho de documentos com precisão."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "Recursos Principais do GroupDocs.Signature"
  features:
    # feature loop
    - title: "Aplique múltiplos tipos de assinatura"
      content: "GroupDocs.Signature permite a aplicação de assinaturas de Texto, Imagem, Código de Barras, Código QR e Selo a qualquer documento. Você pode posicionar assinaturas com precisão em qualquer página e gerenciar metadados facilmente. Proteja seus documentos contra alterações não autorizadas com certificados digitais."

    # feature loop
    - title: "Pesquise e valide assinaturas"
      content: "Verifique as assinaturas de documentos quanto à autenticidade e precisão usando ferramentas de validação avançadas. Obtenha facilmente uma lista detalhada de todas as assinaturas incorporadas em um documento para melhor supervisão."

    # feature loop
    - title: "Modifique assinaturas existentes"
      content: "Você pode atualizar assinaturas previamente aplicadas ajustando conteúdo, posição, cor, tamanho e outros atributos para atender às suas necessidades específicas."

    # feature loop
    - title: "Remova assinaturas rapidamente"
      content: "Otimize o gerenciamento de documentos removendo rapidamente assinaturas indesejadas. Seja um certificado digital ou outro tipo de assinatura, a remoção pode ser realizada de forma eficiente."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Personalize um Código QR Gerado"
      content: |
        Este exemplo mostra como colocar um código QR personalizado em uma página PDF.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # Obtenha o documento a ser assinado e passe-o para Signature
              with sg.Signature('input.pdf') as signature:

                    # Configure as opções do código QR com o texto necessário
                    options = sg.QrCodeSignOptions("Archived on July 11, 2019")

                    # Defina a posição do código QR na página
                    options.VerticalAlignment = sg.Domain.VerticalAlignment.Top
                    options.HorizontalAlignment = sg.Domain.HorizontalAlignment.Right

                    # Defina a margem para a assinatura
                    options.Margin = sg.Padding()
                    options.Margin.Top = 20
                    options.Margin.Right = 20

                    # Escolha a cor do código QR
                    options.ForeColor = sg.Color.Red

                    # Defina as opções de fonte para a mensagem
                    options.Font = sg.SignatureFont()
                    options.Font.Size = 12
                    options.Font.FamilyName = "Comic Sans MS"

                    # Defina a cor de fundo e o pincel para o código QR
                    options.Background = sg.Background()
                    options.Background.Color = Color.LimeGreen
                    options.Background.Transparency = 0.5
                    options.Background.Brush = sg.LinearGradientBrush(sg.Color.LimeGreen, sg.Color.DarkGreen)

                    # Incorpore o código QR no documento
                    result = signature.Sign("output.pdf", options)
          ```
        platform: "python-net"
        copy_title: "Copiar"
        install:
          command: "pip install groupdocs-signature-net"
          copy_tip: "clique para copiar"
          copy_done: "copiado"
        top_links:
          #  loop
          - title: "Baixar resultado"
            icon: "download"
            link: "/examples/signature/formats/signature_qrcode.pdf"
        links:
          #  loop
          - title: "Mais exemplos"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Python-via-.NET/"
          #  loop
          - title: "Documentação"
            link: "https://docs.groupdocs.com/signature/python-net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Pronto para começar?"
  description: "Experimente os recursos do GroupDocs.Signature gratuitamente ou solicite uma licença"
  items:
    #  loop
    - title: "Baixar PyPi"
      link: "https://releases.groupdocs.com/signature/python-net/"
      color: "red"
        #  loop
    - title: "Licenciamento"
      link: "https://purchase.groupdocs.com/pricing/signature/python-net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Explore nossas soluções de assinatura"
    exclude: "qrcode"
    description: "Oferecemos uma ampla variedade de tipos de assinatura e operações para atender às suas necessidades documentais."
    items: 
          
        # operation loop 1
        - name: "Assinaturas eletrônicas"
          operation: "esign"
          link: "/signature/python-net/esign/pdf/"
          description: "Adicionar vários tipos de assinaturas a formatos de arquivo suportados"

        # operation loop 2
        - name: "Adicionar texto a documentos"
          operation: "text"
          link: "/signature/python-net/text/pdf/"
          description: "Melhore o conteúdo do documento com assinaturas de texto personalizáveis"

        # operation loop 3
        - name: "Assinaturas de imagem"
          operation: "image"
          link: "/signature/python-net/image/pdf/"
          description: "Colocar qualquer imagem em qualquer posição dentro de um documento"

        # operation loop 4
        - name: "Gerar códigos de barras"
          operation: "barcode"
          link: "/signature/python-net/barcode/pdf/"
          description: "Criar e inserir vários códigos de barras em documentos suportados"

        # operation loop 5
        - name: "Gerar QR codes"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/pdf/"
          description: "Gerar e QR Codes, incluindo códigos QR, para assinatura de documentos"
          
        # operation loop 6
        - name: "Certificados digitais"
          operation: "digital"
          link: "/signature/python-net/digital/pdf/"
          description: "Proteger negócios e assinar documentos com certificados digitais"

        # operation loop 7
        - name: "Assinaturas de carimbo"
          operation: "stamp"
          link: "/signature/python-net/stamp/pdf/"
          description: "Use o Construtor de Carimbos para criar carimbos redondos ou quadrados personalizados"
          
        # operation loop 8
        - name: "Buscar assinaturas"
          operation: "search"
          link: "/signature/python-net/search/pdf/"
          description: "Localizar quaisquer assinaturas previamente adicionadas em um documento"
          
        # operation loop 9
        - name: "Verificação de assinaturas"
          operation: "verify"
          link: "/signature/python-net/verify/pdf/"
          description: "Verificar a autenticidade das assinaturas após a aplicação"
          
        # operation loop 10
        - name: "Modificar assinaturas"
          operation: "modify"
          link: "/signature/python-net/modify/pdf/"
          description: "Editar uma variedade de assinaturas dentro de um documento"
          
        # operation loop 11
        - name: "Excluir assinaturas"
          operation: "delete"
          link: "/signature/python-net/delete/pdf/"
          description: "Remover uma ampla gama de assinaturas previamente aplicadas"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Incorpore códigos QR em vários formatos de documentos"
    exclude: "PDF"
    description: "Use a API Python via .NET para incorporar códigos QR em qualquer formato de documento padrão da indústria. Armazene e codifique informações importantes em códigos de barras 2D para fácil escaneamento e recuperação de dados."
    items: 
          
        # format loop 1
        - name: "QR-Code para PDF"
          format: "PDF"
          link: "/signature/python-net/qrcode/pdf/"
          description: "Formato de Documento Portátil Adobe"
          
        # format loop 2
        - name: "QR-Code para DOCX"
          format: "DOCX"
          link: "/signature/python-net/qrcode/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 3
        - name: "QR-Code para JPEG"
          format: "JPEG"
          link: "/signature/python-net/qrcode/jpeg/"
          description: "Imagem JPEG"
          
        # format loop 4
        - name: "QR-Code para PPTX"
          format: "PPTX"
          link: "/signature/python-net/qrcode/pptx/"
          description: "Apresentação PowerPoint Open XML"
          
        # format loop 5
        - name: "QR-Code para XLSX"
          format: "XLSX"
          link: "/signature/python-net/qrcode/xlsx/"
          description: "Planilha Microsoft Excel Open XML"


          

---