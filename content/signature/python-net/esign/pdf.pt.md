



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:11
draft: false
lang: pt
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Assinatura eletrônica de documentos PDF com apps Python"
head_description: "Aproveite o poder da API Python para assinar eletronicamente e proteger documentos PDF como PDFs, arquivos Word, planilhas Excel, apresentações e imagens."

############################# Header ############################
title: "Assine documentos PDF eletronicamente" 
description: "Use GroupDocs.Signature for Python via .NET para incorporar uma variedade de assinaturas eletrônicas em seus documentos, garantindo conformidade e integridade dos dados em formatos como PDFs, Word, Excel, apresentações e imagens."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Baixe gratuitamente"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "Visão geral da API GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "Saiba mais"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) oferece um conjunto completo de ferramentas para adicionar assinaturas eletrônicas a documentos. Se você precisa assinar, buscar, verificar, atualizar ou remover assinaturas digitais, o GroupDocs.Signature for Python via .NET facilita tudo em múltiplos formatos — PDFs, documentos Word, planilhas Excel, apresentações PowerPoint e diversos formatos de imagem — sem necessidade de software de terceiros.

############################# Steps ############################
steps:
    enable: true
    title: "Passos para assinar eletronicamente PDF usando Python"
    content: |
      Com [GroupDocs.Signature](/signature/python-net/), desenvolvedores Python via .NET podem integrar funcionalidade de assinatura de forma contínua em documentos PDF. Adicione assinaturas personalizadas às suas aplicações.
      
      1. Carregue o arquivo PDF na instância Signature.
      2. Use SignOptions para configurar as definições da assinatura.
      3. Personalize as propriedades da assinatura, como tamanho, cor e conteúdo.
      4. Salve o documento assinado no local desejado.
   
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

            # Carregue o documento em uma instância Signature
            with sg.Signature('input.pdf') as signature:

                # Crie um novo objeto QrCodeSignOptions
                options = sg.QrCodeSignOptions("QR code text")

                # Configure todas as opções necessárias
                options.Left = 100
                options.Top = 100
                options.ForeColor = sg.Color.Red

                # Salve o documento assinado em seu sistema
                result = signature.Sign("output.pdf", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Recursos avançados de assinatura eletrônica para documentos"
  description: "Nossa API de assinatura eletrônica simplifica os processos de negócios, oferecendo maneiras eficientes de assinar, validar, modificar e gerenciar assinaturas eletrônicas com total suporte à automação."
  image: "/img/signature/features_esign.webp" # 500x500 px
  image_description: "Recursos de Assinatura Eletrônica"
  features:
    # feature loop
    - title: "Assinatura de documentos do escritório"
      content: "Insira assinaturas eletrônicas em qualquer lugar de seus documentos. Personalize seu conteúdo com certificados digitais, códigos de barras, metadados e elementos visuais, enquanto garante a segurança e autenticidade do documento."

    # feature loop
    - title: "Gerenciamento completo de assinaturas"
      content: "Depois que um documento é assinado, você pode visualizar e gerenciar todas as assinaturas. Você pode fazer atualizações ou remover assinaturas conforme necessário, garantindo controle total sobre o documento."

    # feature loop
    - title: "Aumente a segurança do documento"
      content: "Proteja seus documentos com certificados digitais. Incorpore ou recupere metadados para melhorar o rastreamento, auditoria e conformidade, garantindo a autenticidade do seu conteúdo."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Como adicionar uma assinatura de imagem a um documento"
      content: |
        Este exemplo demonstra como aplicar uma assinatura de imagem a uma página específica de um documento.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg
        
          def run():

              # Carregue o documento que você deseja assinar
              with sg.Signature('input.pdf') as signature:

                  # Defina o caminho da imagem nas opções de assinatura
                  options = sg.ImageSignOptions("image.jpg")

                  # Defina o tamanho e a colocação da assinatura nas páginas de destino
                  options.VerticalAlignment = sg.VerticalAlignment.Bottom
                  options.HorizontalAlignment = sg.HorizontalAlignment.Right
                  options.Height = 150
                  options.Width = 200
                  options.Margin = sg.Padding(50)
                  options.AllPages = True

                  # Aplique a assinatura e salve o documento assinado
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
            link: "/examples/signature/formats/signature_esign.pdf"
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
    title: "Explore nosso conjunto completo de recursos"
    exclude: "esign"
    description: "Oferecemos uma ampla gama de opções de assinatura e operações para todas as suas necessidades de assinatura eletrônica."
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
    title: "Assine uma ampla variedade de formatos de arquivo"
    exclude: "PDF"
    description: "Com a API Python via .NET, você pode assinar eletronicamente mais de 60 formatos padrão do setor, oferecendo flexibilidade inigualável na segurança de seus documentos comerciais."
    items: 
          
        # format loop 1
        - name: "Assinatura eletrônica em PDF"
          format: "PDF"
          link: "/signature/python-net/esign/pdf/"
          description: "Formato de Documento Portátil Adobe"
          
        # format loop 2
        - name: "Assinatura eletrônica em DOCX"
          format: "DOCX"
          link: "/signature/python-net/esign/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 3
        - name: "Assinatura eletrônica em JPEG"
          format: "JPEG"
          link: "/signature/python-net/esign/jpeg/"
          description: "Imagem JPEG"
          
        # format loop 4
        - name: "Assinatura eletrônica em PPTX"
          format: "PPTX"
          link: "/signature/python-net/esign/pptx/"
          description: "Apresentação PowerPoint Open XML"
          
        # format loop 5
        - name: "Assinatura eletrônica em XLSX"
          format: "XLSX"
          link: "/signature/python-net/esign/xlsx/"
          description: "Planilha Microsoft Excel Open XML"


          

---