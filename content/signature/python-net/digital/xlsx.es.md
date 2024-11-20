



---
############################# Static ############################
layout: "format"
date:  2024-11-20T08:57:23
draft: false
lang: es
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Crea firmas digitales para XLSX usando Python"
head_description: "Firma digitalmente documentos XLSX usando Python en solo unas pocas líneas de código. Utiliza GroupDocs.Signature for Python via .NET para firmar una amplia gama de formatos de archivo."

############################# Header ############################
title: "Firma digitalmente XLSX" 
description: "Asegura la seguridad y autenticidad de tus documentos aplicando certificados digitales a través de GroupDocs.Signature for Python via .NET. Nuestra solución te permite firmar y proteger tus documentos con herramientas potentes."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Obténlo gratis"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "¿Qué es GroupDocs.Signature for Python via .NET?"
    link: "/signature/python-net/"
    link_title: "Aprende más"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) es una herramienta integral de firma que admite una amplia gama de tareas de procesamiento de documentos. Te permite añadir texto, imágenes, certificados digitales y sellos a más de 60 formatos de archivo, incluidos PDFs, archivos de MS Office, imágenes y ZIPs. Con GroupDocs.Signature for Python via .NET, también puedes buscar, verificar, actualizar o eliminar firmas cuando lo necesites.

############################# Steps ############################
steps:
    enable: true
    title: "Cómo proteger XLSX con certificados digitales en Python"
    content: |
      [GroupDocs.Signature](/signature/python-net/) ayuda a los desarrolladores de Python via .NET a proteger archivos XLSX añadiendo firmas digitales. Fortalece tus aplicaciones empresariales con sólidas funciones de protección de documentos.
      
      1. Carga el archivo XLSX en la clase Signature.
      2. Aplica un certificado digital y su contraseña para asegurar el archivo.
      3. Opcionalmente, añade una representación visual de la firma digital en las páginas del documento.
      4. Firma el documento para evitar cambios no autorizados.
   
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

            # Utiliza Signature para firmar digitalmente el documento
            with sg.Signature('input.xlsx') as signature:

                # Ingresa el certificado digital y su contraseña
                options = sg.DigitalSignOptions("certificate.pfx")
                options.Password = "1234567890"

                # Opcionalmente, configura cómo se verá la firma
                options.PageNumber = 1
                options.Left = 50
                options.Top = 50

                # Finaliza el documento con el certificado digital
                result = signature.Sign("output.xlsx", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Mejora y asegura documentos con firmas digitales"
  description: "La biblioteca GroupDocs.Signature for Python via .NET está diseñada para firmar todos los principales formatos de archivo. Simplifica tu flujo de trabajo añadiendo, verificando, actualizando o eliminando diferentes tipos de firmas."
  image: "/img/signature/features_digital.webp" # 500x500 px
  image_description: "Características clave de GroupDocs.Signature"
  features:
    # feature loop
    - title: "Añadir firmas a tus documentos"
      content: "Inserta firmas de texto, imagen, código de barras, código QR o sello con precisión en cualquier parte de los documentos compatibles. También puedes gestionar metadatos ocultos, como EXIF en imágenes, para asegurar la integridad del documento con firmas digitales."

    # feature loop
    - title: "Verificar y buscar firmas"
      content: "Después de firmar, puedes verificar documentos fácilmente para garantizar un procesamiento correcto. Recupera y gestiona todas las firmas dentro de tus archivos con potentes capacidades de búsqueda."

    # feature loop
    - title: "Editar firmas existentes"
      content: "La mayoría de las firmas pueden ser completamente personalizadas. Puedes editar texto, mover elementos, cambiar colores, ajustar tamaños y más para adaptarlas a tus necesidades."

    # feature loop
    - title: "Eliminar firmas innecesarias"
      content: "Nuestra solución admite una gestión completa de firmas, permitiéndote eliminar firmas, incluidos certificados digitales, de cualquier documento cuando sea necesario."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Protege documentos con firmas digitales"
      content: |
        Aprende a asegurar tus documentos aplicando firmas digitales para prevenir modificaciones no autorizadas.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # Carga el documento que será firmado
              with sg.Signature('input.xlsx') as signature:

                  # Utiliza un certificado digital válido con su contraseña correspondiente
                  options = sg.DigitalSignOptions("certificate.pfx")
                  options.Password = "1234567890"

                  # Añade cualquier información de texto adicional si es necesario
                  options.Reason = "Security issue"
                  options.Contact = "John Smith"
                  options.Location = "Office D.W."

                  # Incluye una imagen u otras opciones para representación visual de la firma
                  options.ImageFilePath = "image.png"
                  options.AllPages = True
                  options.VerticalAlignment = sg.VerticalAlignment.Center
                  options.HorizontalAlignment = sg.HorizontalAlignment.Left
                  options.Width = 60
                  options.Height = 80

                  options.Margin = sg.Padding()
                  options.Margin.Bottom = 10
                  options.Margin.Right = 10

                  # Guarda el documento firmado en una ubicación segura
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
            link: "/examples/signature/formats/signature_digital.xlsx"
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
    title: "Explora nuestras características clave"
    exclude: "digital"
    description: "Ofrecemos una amplia gama de opciones de firma y potentes operaciones sobre documentos."
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
    title: "Firma documentos en múltiples formatos"
    exclude: "XLSX"
    description: "Con la API Python via .NET, puedes procesar más de 60 formatos diferentes, añadiendo firmas, aplicando certificados digitales para seguridad y gestionando firmas en varias páginas."
    items: 
          
        # format loop 1
        - name: "Proteger PDF"
          format: "PDF"
          link: "/signature/python-net/digital/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 2
        - name: "Proteger DOCX"
          format: "DOCX"
          link: "/signature/python-net/digital/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Proteger PPTX"
          format: "PPTX"
          link: "/signature/python-net/digital/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 4
        - name: "Proteger XLSX"
          format: "XLSX"
          link: "/signature/python-net/digital/xlsx/"
          description: "Hoja de Cálculo XML Abierto de Microsoft Excel"


          

---