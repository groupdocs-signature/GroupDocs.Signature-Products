



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:49
draft: false
lang: pt
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Crie selos redondos e quadrados em PDF usando Python"
head_description: "Gere e insira selos personalizados em arquivos PDF com a API GroupDocs.Signature for Python via .NET."

############################# Header ############################
title: "Crie selos para PDF" 
description: "Adicione selos personalizados em qualquer parte de seus documentos com GroupDocs.Signature for Python via .NET, oferecendo grande flexibilidade para posicionamento e configuração para atender suas necessidades de negócios."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Baixar gratuitamente"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "Visão geral do GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "Saiba mais"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) é uma ferramenta abrangente que permite inserir vários tipos de assinatura em documentos, incluindo selos personalizados. Suportando mais de 60 formatos de arquivo - de PDFs e documentos do Word a imagens e arquivos ZIP - você pode enriquecer seus documentos com texto, imagem, código de barras, metadados, certificados digitais e selos. Você também tem controle total para pesquisar, verificar, editar ou excluir quaisquer assinaturas aplicadas.

############################# Steps ############################
steps:
    enable: true
    title: "Como adicionar um selo a PDF usando Python"
    content: |
      [GroupDocs.Signature](/signature/python-net/) fornece ferramentas robustas para criação de selos para aprimorar aplicativos Python via .NET. Use-o para projetar e implementar selos personalizados para suas páginas de documentos.
      
      1. Forneça o documento PDF que deseja selar.
      2. Use StampSignOptions para configurar todas as configurações necessárias.
      3. Adicione várias linhas de selo se necessário.
      4. Aplique o selo e salve o documento atualizado.
   
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

            # Anexe o caminho do documento à instância Signature
            with sg.Signature('input.pdf') as signature:

                # Configure StampSignOptions com os detalhes necessários do selo
                options = sg.StampSignOptions()
                options.Height = 180
                options.Width = 180

                # Adicione uma ou mais linhas ao selo
                outerLine = sg.StampLine()
                outerLine.Text = "* The Best Company *"
                outerLine.TextRepeatType = sg.StampTextRepeatType.FullTextRepeat
                outerLine.Font = sg.SignatureFont()
                outerLine.Font.Size = 12
                outerLine.Font.FamilyName = "Arial"
                outerLine.Height = 22
                outerLine.TextBottomIntent = 6
                outerLine.TextColor = sg.Color.WhiteSmoke
                outerLine.BackgroundColor = sg.Color.DarkSlateBlue
                options.OuterLines.Add(outerLine)

                # Salve o documento com o selo aplicado
                result = signature.Sign("output.pdf", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Use assinaturas para proteger e melhorar a integridade do documento"
  description: "Com a biblioteca GroupDocs.Signature for Python via .NET, você pode adicionar funcionalidades de assinatura aos seus documentos de forma fluida. Crie, modifique, verifique ou exclua facilmente selos personalizados e outros tipos de assinatura, proporcionando flexibilidade e segurança para seus fluxos de trabalho de documentos."
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "Assinaturas de Selo Reforçadas por GroupDocs.Signature"
  features:
    # feature loop
    - title: "Assinatura completa de documentos"
      content: "Eleve seus documentos adicionando assinaturas como texto, imagens, códigos de barras, códigos QR e selos em qualquer posição de qualquer página. Gerencie metadados incorporados e aplique certificados digitais para proteger contra alterações não autorizadas."

    # feature loop
    - title: "Busca e verificação de assinatura eficientes"
      content: "Após a assinatura, utilize ferramentas de busca avançadas para encontrar todas as assinaturas incorporadas. Verifique ou gerencie facilmente os dados das assinaturas para garantir a integridade do documento."

    # feature loop
    - title: "Edite e personalize assinaturas"
      content: "Faça alterações em assinaturas previamente adicionadas. Se desejar alterar o conteúdo, a posição, o tamanho ou a cor, GroupDocs.Signature for Python via .NET oferece controle total para ajustar as assinaturas conforme necessário."

    # feature loop
    - title: "Remova assinaturas facilmente"
      content: "Se precisar remover assinaturas, GroupDocs.Signature for Python via .NET oferece todas as ferramentas necessárias para excluir qualquer tipo, incluindo selos e certificados digitais, ajudando você a manter seus documentos atualizados e em conformidade."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Como adicionar selos personalizados a documentos"
      content: |
        Este exemplo mostra como criar e inserir selos personalizados com detalhes de texto específicos em um documento.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # Forneça o documento que deseja selar
              with sg.Signature('input.pdf') as signature:

                    # Configure as opções de selo com suas configurações desejadas
                    options = sg.StampSignOptions()

                    # Defina o tamanho e o posicionamento do selo na página
                    options.Height = 200
                    options.Width = 200
                    options.VerticalAlignment = sg.VerticalAlignment.Bottom
                    options.HorizontalAlignment = sg.HorizontalAlignment.Right
                    options.AllPages = True

                    # Adicione linhas circulares externas com texto
                    outerLine = sg.StampLine()
                    outerLine.Text = "* The best  choice *"
                    outerLine.TextRepeatType = sg.StampTextRepeatType.FullTextRepeat
                    outerLine.Font = sg.SignatureFont()
                    outerLine.Font.Size = 12
                    outerLine.Font.FamilyName = "Arial"
                    outerLine.Height = 22
                    outerLine.TextBottomIntent = 6
                    outerLine.TextColor = sg.Color.WhiteSmoke
                    outerLine.BackgroundColor = sg.Color.DarkSlateBlue
                    options.OuterLines.Add(outerLine)

                    # Opcionalmente, adicione linhas quadradas internas
                    innerLine = sg.StampLine()
                    innerLine.Text = "Company #1"
                    innerLine.TextColor = sg.Color.MediumVioletRed
                    innerLine.Font = sg.SignatureFont()
                    innerLine.Font.Size = 20
                    innerLine.Font.Bold = True
                    innerLine.Height = 40
                    options.InnerLines.Add(innerLine)

                    # Finalize e salve o documento selado
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
            link: "/examples/signature/formats/signature_stamp.pdf"
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
    title: "Explore recursos principais"
    exclude: "stamp"
    description: "Encontre uma ampla gama de opções para criar, gerenciar e remover assinaturas, dando a você total controle sobre os fluxos de trabalho dos documentos."
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
    title: "Aplique selos a vários formatos de documento"
    exclude: "PDF"
    description: "Com a API GroupDocs.Signature, você pode inserir selos personalizados em mais de 60 tipos de arquivo padrão. Aplique selos facilmente em qualquer lugar dos seus documentos, melhorando a personalização e o rastreamento."
    items: 
          
        # format loop 1
        - name: "Carimbar PDF"
          format: "PDF"
          link: "/signature/python-net/stamp/pdf/"
          description: "Formato de Documento Portátil Adobe"
          
        # format loop 2
        - name: "Carimbar DOCX"
          format: "DOCX"
          link: "/signature/python-net/stamp/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 3
        - name: "Carimbar JPEG"
          format: "JPEG"
          link: "/signature/python-net/stamp/jpeg/"
          description: "Imagem JPEG"
          
        # format loop 4
        - name: "Carimbar PPTX"
          format: "PPTX"
          link: "/signature/python-net/stamp/pptx/"
          description: "Apresentação PowerPoint Open XML"
          
        # format loop 5
        - name: "Carimbar XLSX"
          format: "XLSX"
          link: "/signature/python-net/stamp/xlsx/"
          description: "Planilha Microsoft Excel Open XML"


          

---