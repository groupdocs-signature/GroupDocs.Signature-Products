



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:15
draft: false
lang: pt
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Adicione assinaturas de texto a PDF usando Python"
head_description: "Utilize a API Python para incorporar assinaturas baseadas em texto em arquivos PDF, suportando formatos como PDF, Word, Excel, PowerPoint, imagens e ZIP."

############################# Header ############################
title: "Adicione assinaturas de texto a PDF" 
description: "Integre assinaturas de texto personalizadas em seus documentos com GroupDocs.Signature for Python via .NET. Simplifique seus fluxos de trabalho com opções flexíveis de personalização de assinaturas."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Experimente gratuitamente hoje"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "Explore o poder do GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "Saiba mais"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) oferece uma plataforma abrangente para incorporar assinaturas de texto personalizáveis, tornando os fluxos de trabalho de documentos mais ágeis. Personalize o conteúdo e a aparência das assinaturas em documentos para aumentar a eficiência e melhorar a gestão de documentos.

############################# Steps ############################
steps:
    enable: true
    title: "Como criar assinaturas de texto em PDF com Python"
    content: |
      [GroupDocs.Signature](/signature/python-net/) possibilita a integração de assinaturas de texto em arquivos PDF dentro de aplicativos Python via .NET. Adicione rapidamente funcionalidades aos seus produtos com esta solução.
      
      1. Forneça o documento PDF ao construtor Signature.
      2. Crie TextSignOptions com o texto da sua assinatura.
      3. Defina as propriedades visuais da assinatura.
      4. Insira a assinatura nas páginas desejadas do documento.
   
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

            # Inicialize a Signature com o caminho do documento
            with sg.Signature('input.pdf') as signature:

                # Configure TextSignOptions com o texto da assinatura desejado
                options = sg.TextSignOptions("Approved")

                # Escolha a cor e a fonte para a assinatura
                options.ForeColor = sg.Color.Red
                options.Font = sg.SignatureFont()
                options.Font.Size = 12
                options.Font.FamilyName = "Comic Sans MS"

                # Aplique a assinatura de texto ao documento
                result = signature.Sign("output.pdf", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Gerenciamento completo de assinaturas de texto"
  description: "GroupDocs.Signature for Python via .NET ajuda você a gerenciar fluxos de trabalho de documentos adicionando assinaturas de texto personalizadas a formatos populares. Controle facilmente a aparência, o posicionamento e o conteúdo das assinaturas de acordo com suas necessidades."
  image: "/img/signature/features_text.webp" # 500x500 px
  image_description: "Descubra os Recursos do GroupDocs.Signature"
  features:
    # feature loop
    - title: "Assinaturas documentais flexíveis"
      content: "Adicione vários tipos de assinatura—texto, imagens, códigos de barras, QR codes e carimbos—em qualquer página do documento. Utilize metadados para incluir informações ocultas e proteja seus arquivos com certificados digitais."

    # feature loop
    - title: "Verifique e busque assinaturas"
      content: "Use ferramentas avançadas para verificar a integridade de seus documentos assinados. Pesquise e analise todas as assinaturas em um arquivo para validação adicional."

    # feature loop
    - title: "Edite ou remova assinaturas"
      content: "Atualize facilmente o conteúdo, a aparência ou a posição de assinaturas existentes. Remova assinaturas desatualizadas para manter seus documentos atualizados."

    # feature loop
    - title: "Assinaturas de texto especializadas"
      content: "Aplique assinaturas de texto específicas do documento, como marcas d'água para arquivos do Word ou carimbos para PDFs, adicionando um nível extra de controle e personalização."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Adicione assinaturas de texto a documentos"
      content: |
        Aprenda como incorporar assinaturas de texto em documentos para otimizar seus processos.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # Selecione o documento a ser assinado
              with sg.Signature('input.pdf') as signature:

                    # Configure as opções de texto com o conteúdo desejado
                    options = sg.TextSignOptions("Rescheduled to 03/04/2025")

                    # Defina o tamanho e a posição da assinatura
                    options.Left = 100
                    options.Top = 180
                    options.Width = 230
                    options.Height = 30

                    # Defina a margem das bordas da página
                    options.Margin = sg.Padding()
                    options.Margin.Top = 20
                    options.Margin.Right = 20

                    # Escolha a cor do texto e o estilo da fonte
                    options.ForeColor = sg.Color.Red
                    options.Font = sg.SignatureFont()
                    options.Font.Size = 12
                    options.Font.FamilyName = "Comic Sans MS"

                    # Adicione uma borda em torno da assinatura de texto
                    options.Border = sg.Border()
                    options.Border.Color = sg.Color.Red
                    options.Border.DashStyle = sg.DashStyle.DashLongDashDot
                    options.Border.Transparency = 0.5
                    options.Border.Visible = True
                    options.Border.Weight = 2

                    # Personalize o fundo, se necessário
                    options.Background = sg.Background()
                    options.Background.Color = sg.Color.Yellow
                    options.Background.Transparency = 0.8

                    # Opcionalmente, salve a assinatura como uma imagem para compatibilidade
                    options.SignatureImplementation = sg.TextSignatureImplementation.Image

                    # Salve o documento com a assinatura incorporada
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
            link: "/examples/signature/formats/signature_text.pdf"
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
    title: "Recursos avançados de assinatura"
    exclude: "text"
    description: "Nossa API suporta gerenciamento completo do ciclo de vida para sete tipos de assinatura, permitindo que você crie, gerencie, verifique e personalize suas assinaturas com eficiência."
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
    title: "Incorpore assinaturas de texto em vários formatos"
    exclude: "PDF"
    description: "Com a API Python via .NET, você pode adicionar assinaturas de texto a vários documentos do Office, dando a você controle total sobre o ciclo de vida do documento e melhorando a segurança."
    items: 
          
        # format loop 1
        - name: "Assinaturas de texto em PDF"
          format: "PDF"
          link: "/signature/python-net/text/pdf/"
          description: "Formato de Documento Portátil Adobe"
          
        # format loop 2
        - name: "Assinaturas de texto em DOCX"
          format: "DOCX"
          link: "/signature/python-net/text/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 3
        - name: "Assinaturas de texto em JPEG"
          format: "JPEG"
          link: "/signature/python-net/text/jpeg/"
          description: "Imagem JPEG"
          
        # format loop 4
        - name: "Assinaturas de texto em PPTX"
          format: "PPTX"
          link: "/signature/python-net/text/pptx/"
          description: "Apresentação PowerPoint Open XML"
          
        # format loop 5
        - name: "Assinaturas de texto em XLSX"
          format: "XLSX"
          link: "/signature/python-net/text/xlsx/"
          description: "Planilha Microsoft Excel Open XML"


          

---