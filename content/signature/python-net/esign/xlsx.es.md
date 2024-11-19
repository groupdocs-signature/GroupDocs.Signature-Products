



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:30
draft: false
lang: es
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Firma electrónicamente documentos XLSX con aplicaciones Python"
head_description: "Aprovecha el poder de la API Python para firmar electrónicamente y asegurar documentos XLSX como PDFs, archivos de Word, hojas de Excel, presentaciones e imágenes."

############################# Header ############################
title: "Firma electrónica de XLSX" 
description: "Utiliza GroupDocs.Signature for Python via .NET para incrustar una variedad de firmas electrónicas en tus documentos, garantizando cumplimiento e integridad de datos en formatos como PDFs, Word, Excel, presentaciones e imágenes."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Descargar gratis"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "Resumen de la API GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "Aprende más"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) proporciona un conjunto completo de herramientas para agregar firmas electrónicas a documentos. Ya sea que necesites firmar, buscar, verificar, actualizar o eliminar firmas digitales, GroupDocs.Signature for Python via .NET lo hace sencillo en múltiples formatos: PDFs, documentos de Word, hojas de Excel, presentaciones de PowerPoint y varios formatos de imagen, sin necesidad de software de terceros.

############################# Steps ############################
steps:
    enable: true
    title: "Pasos para firmar electrónicamente XLSX usando Python"
    content: |
      Con [GroupDocs.Signature](/signature/python-net/), los desarrolladores de Python via .NET pueden integrar sin problemas la funcionalidad de firma en documentos XLSX. Agrega firmas personalizadas a tus aplicaciones.
      
      1. Carga el archivo XLSX en la instancia de Signature.
      2. Utiliza SignOptions para configurar los ajustes de la firma.
      3. Personaliza las propiedades de la firma como tamaño, color y contenido.
      4. Guarda el documento firmado en la ubicación deseada.
   
    code:
      platform: "python-net"
      copy_title: "Copiar"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Firmas de muestra"
      install:
        command: "pip install groupdocs-signature-net"
        copy_tip: "haz clic para copiar"
        copy_done: "copiado"
      links:
        #  loop
        - title: "Más ejemplos"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Python-via-.NET/"
        #  loop
        - title: "Documentación"
          link: "https://docs.groupdocs.com/signature/python-net/"
          
      content: |
        ```python {style=abap}
        import groupdocs.signature as sg

        def run():

            # Carga el documento en una instancia de Signature
            with sg.Signature('input.xlsx') as signature:

                # Crea un nuevo objeto QrCodeSignOptions
                options = sg.QrCodeSignOptions("QR code text")

                # Configura todas las opciones requeridas
                options.Left = 100
                options.Top = 100
                options.ForeColor = sg.Color.Red

                # Guarda el documento firmado en tu sistema
                result = signature.Sign("output.xlsx", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Características avanzadas de firma electrónica para documentos"
  description: "Nuestra API de firma electrónica optimiza los procesos comerciales al ofrecer maneras eficientes de firmar, validar, modificar y gestionar firmas electrónicas con soporte completo para la automatización."
  image: "/img/signature/features_esign.webp" # 500x500 px
  image_description: "Características de firma electrónica"
  features:
    # feature loop
    - title: "Firma documentos de oficina"
      content: "Coloca firmas electrónicas en cualquier parte de tus documentos. Personaliza tu contenido con certificados digitales, códigos de barras, metadatos y elementos visuales, todo mientras aseguras la seguridad y autenticidad del documento."

    # feature loop
    - title: "Gestión completa de firmas"
      content: "Una vez que un documento está firmado, puedes ver y gestionar todas las firmas. Puedes realizar actualizaciones o eliminar firmas según sea necesario, asegurando el control completo sobre el documento."

    # feature loop
    - title: "Aumenta la seguridad de los documentos"
      content: "Protege tus documentos con certificados digitales. Incrusta o recupera metadatos para mejorar el seguimiento, auditoría y cumplimiento, asegurando la autenticidad de tu contenido."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cómo añadir una firma de imagen a un documento"
      content: |
        Este ejemplo demuestra cómo aplicar una firma de imagen a una página específica de un documento.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg
        
          def run():

              # Carga el documento que deseas firmar
              with sg.Signature('input.xlsx') as signature:

                  # Establece la ruta de la imagen en las opciones de la firma
                  options = sg.ImageSignOptions("image.jpg")

                  # Define el tamaño y la colocación de la firma en las páginas objetivo
                  options.VerticalAlignment = sg.VerticalAlignment.Bottom
                  options.HorizontalAlignment = sg.HorizontalAlignment.Right
                  options.Height = 150
                  options.Width = 200
                  options.Margin = sg.Padding(50)
                  options.AllPages = True

                  # Aplica la firma y guarda el documento firmado
                  result = signature.Sign("output.xlsx", options)
          ```
        platform: "python-net"
        copy_title: "Copiar"
        install:
          command: "pip install groupdocs-signature-net"
          copy_tip: "haz clic para copiar"
          copy_done: "copiado"
        top_links:
          #  loop
          - title: "Descargar resultado"
            icon: "download"
            link: "/examples/signature/formats/signature_esign.xlsx"
        links:
          #  loop
          - title: "Más ejemplos"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Python-via-.NET/"
          #  loop
          - title: "Documentación"
            link: "https://docs.groupdocs.com/signature/python-net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "¿Listo para empezar?"
  description: "Prueba las funciones de GroupDocs.Signature de forma gratuita o solicita una licencia"
  items:
    #  loop
    - title: "Descarga de PyPi"
      link: "https://releases.groupdocs.com/signature/python-net/"
      color: "red"
        #  loop
    - title: "Licenciamiento"
      link: "https://purchase.groupdocs.com/pricing/signature/python-net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Explora nuestro conjunto completo de funciones"
    exclude: "esign"
    description: "Ofrecemos una amplia gama de opciones y operaciones de firma para todas tus necesidades de firma electrónica."
    items: 
          
        # operation loop 1
        - name: "Firmas electrónicas"
          operation: "esign"
          link: "/signature/python-net/esign/xlsx/"
          description: "Agrega varios tipos de firmas a formatos de archivo soportados"

        # operation loop 2
        - name: "Agregar texto a documentos"
          operation: "text"
          link: "/signature/python-net/text/xlsx/"
          description: "Mejora el contenido del documento con firmas de texto personalizables"

        # operation loop 3
        - name: "Firmas de imagen"
          operation: "image"
          link: "/signature/python-net/image/xlsx/"
          description: "Coloca cualquier imagen en cualquier posición dentro de un documento"

        # operation loop 4
        - name: "Generar códigos de barras"
          operation: "barcode"
          link: "/signature/python-net/barcode/xlsx/"
          description: "Crear e insertar varios códigos de barras en documentos soportados"

        # operation loop 5
        - name: "Generar códigos QR"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/xlsx/"
          description: "Generar y utilizar códigos QR para la firma de documentos"
          
        # operation loop 6
        - name: "Certificados digitales"
          operation: "digital"
          link: "/signature/python-net/digital/xlsx/"
          description: "Asegura negocios y firma documentos con certificados digitales"

        # operation loop 7
        - name: "Firmas de sello"
          operation: "stamp"
          link: "/signature/python-net/stamp/xlsx/"
          description: "Utiliza el Constructor de Sellos para crear sellos personalizados redondos o cuadrados"
          
        # operation loop 8
        - name: "Buscar firmas"
          operation: "search"
          link: "/signature/python-net/search/xlsx/"
          description: "Ubica cualquier firma previamente añadida dentro de un documento"
          
        # operation loop 9
        - name: "Verificación de firmas"
          operation: "verify"
          link: "/signature/python-net/verify/xlsx/"
          description: "Verifica la autenticidad de las firmas después de que se han aplicado"
          
        # operation loop 10
        - name: "Modificar firmas"
          operation: "modify"
          link: "/signature/python-net/modify/xlsx/"
          description: "Edita fácilmente una variedad de firmas dentro de un documento"
          
        # operation loop 11
        - name: "Eliminar firmas"
          operation: "delete"
          link: "/signature/python-net/delete/xlsx/"
          description: "Remueve una amplia gama de firmas aplicadas previamente"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Firma una amplia gama de formatos de archivo"
    exclude: "XLSX"
    description: "Con la API Python via .NET, puedes firmar electrónicamente más de 60 formatos estándar de la industria, ofreciendo una flexibilidad sin igual en la seguridad de tus documentos comerciales."
    items: 
          
        # format loop 1
        - name: "Firma electrónica PDF"
          format: "PDF"
          link: "/signature/python-net/esign/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 2
        - name: "Firma electrónica DOCX"
          format: "DOCX"
          link: "/signature/python-net/esign/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Firma electrónica JPEG"
          format: "JPEG"
          link: "/signature/python-net/esign/jpeg/"
          description: "Imagen JPEG"
          
        # format loop 4
        - name: "Firma electrónica PPTX"
          format: "PPTX"
          link: "/signature/python-net/esign/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 5
        - name: "Firma electrónica XLSX"
          format: "XLSX"
          link: "/signature/python-net/esign/xlsx/"
          description: "Hoja de Cálculo XML Abierto de Microsoft Excel"


          

---