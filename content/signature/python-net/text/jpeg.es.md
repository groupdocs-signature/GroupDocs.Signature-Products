



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:15
draft: false
lang: es
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Añadir firmas de texto a JPEG usando Python"
head_description: "Aprovecha la API de Python para incrustar firmas basadas en texto en archivos JPEG, soportando formatos como PDF, Word, Excel, PowerPoint, imágenes y ZIP."

############################# Header ############################
title: "Añadir firmas de texto a JPEG" 
description: "Integra sin esfuerzo firmas de texto personalizadas en tus documentos usando GroupDocs.Signature for Python via .NET. Simplifica tus flujos de trabajo con opciones flexibles de personalización de firmas."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Pruébalo gratis hoy"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "Descubre el potencial de GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "Aprende más"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) ofrece una plataforma integral para incrustar firmas de texto personalizables, lo que facilita los flujos de trabajo de documentos. Personaliza el contenido y la apariencia de las firmas en todos los documentos para aumentar la eficiencia y mejorar la gestión documental.

############################# Steps ############################
steps:
    enable: true
    title: "Cómo crear firmas de texto en JPEG con Python"
    content: |
      [GroupDocs.Signature](/signature/python-net/) permite una fácil integración de firma de texto en archivos JPEG dentro de aplicaciones Python via .NET. Añade rápidamente funcionalidad a tus productos con esta solución.
      
      1. Proporciona el documento JPEG al constructor de Signature.
      2. Crea TextSignOptions con tu texto de firma.
      3. Establece las propiedades visuales de la firma.
      4. Inserta la firma en las páginas deseadas del documento.
   
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

            # Inicializa la Signature con la ruta del documento
            with sg.Signature('input.jpeg') as signature:

                # Configura TextSignOptions con el texto de firma deseado
                options = sg.TextSignOptions("Approved")

                # Elige el color y la fuente para la firma
                options.ForeColor = sg.Color.Red
                options.Font = sg.SignatureFont()
                options.Font.Size = 12
                options.Font.FamilyName = "Comic Sans MS"

                # Aplica la firma de texto al documento
                result = signature.Sign("output.jpeg", options)
        ```                

############################# More features ############################
more_features:
  enable: true
  title: "Gestión completa de firmas de texto"
  description: "GroupDocs.Signature for Python via .NET te ayuda a gestionar flujos de trabajo de documentos al añadir firmas de texto personalizadas a formatos populares. Controla sin esfuerzo la apariencia, la ubicación y el contenido de las firmas para adaptarlas a tus necesidades."
  image: "/img/signature/features_text.webp" # 500x500 px
  image_description: "Descubre las características de GroupDocs.Signature"
  features:
    # feature loop
    - title: "Firmas de documentos flexibles"
      content: "Añade varios tipos de firma: texto, imágenes, códigos de barras, códigos QR y sellos a cualquier página del documento. Usa metadatos para incluir información oculta y proteger tus archivos con certificados digitales."

    # feature loop
    - title: "Verificar y buscar firmas"
      content: "Utiliza herramientas avanzadas para comprobar la integridad de tus documentos firmados. Busca y analiza todas las firmas en un archivo para una validación adicional."

    # feature loop
    - title: "Editar o eliminar firmas"
      content: "Actualiza fácilmente el contenido, la apariencia o la ubicación de las firmas existentes. Elimina firmas obsoletas para mantener tus documentos actualizados."

    # feature loop
    - title: "Firmas de texto especializadas"
      content: "Aplica firmas de texto específicas para el documento, como marcas de agua para archivos de Word o sellos para PDFs, añadiendo un nivel adicional de control y personalización."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Añadir firmas de texto a documentos"
      content: |
        Aprende cómo incrustar firmas de texto en documentos para optimizar tus procesos.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # Selecciona el documento para firmar
              with sg.Signature('input.jpeg') as signature:

                    # Configura las opciones de texto con el contenido deseado
                    options = sg.TextSignOptions("Rescheduled to 03/04/2025")

                    # Define el tamaño y la ubicación de la firma
                    options.Left = 100
                    options.Top = 180
                    options.Width = 230
                    options.Height = 30

                    # Establece el relleno desde los bordes de la página
                    options.Margin = sg.Padding()
                    options.Margin.Top = 20
                    options.Margin.Right = 20

                    # Elige el color del texto y el estilo de fuente
                    options.ForeColor = sg.Color.Red
                    options.Font = sg.SignatureFont()
                    options.Font.Size = 12
                    options.Font.FamilyName = "Comic Sans MS"

                    # Añade un borde alrededor de la firma de texto
                    options.Border = sg.Border()
                    options.Border.Color = sg.Color.Red
                    options.Border.DashStyle = sg.DashStyle.DashLongDashDot
                    options.Border.Transparency = 0.5
                    options.Border.Visible = True
                    options.Border.Weight = 2

                    # Personaliza el fondo si es necesario
                    options.Background = sg.Background()
                    options.Background.Color = sg.Color.Yellow
                    options.Background.Transparency = 0.8

                    # Opcionalmente guarda la firma como una imagen para compatibilidad
                    options.SignatureImplementation = sg.TextSignatureImplementation.Image

                    # Guarda el documento con la firma incrustada
                    result = signature.Sign("output.jpeg", options)
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
            link: "/examples/signature/formats/signature_text.jpeg"
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
    title: "Características avanzadas de firmas"
    exclude: "text"
    description: "Nuestra API soporta la gestión completa del ciclo de vida para siete tipos de firma, permitiéndote crear, gestionar, verificar y personalizar tus firmas de forma efectiva."
    items: 
          
        # operation loop 1
        - name: "Firmas electrónicas"
          operation: "esign"
          link: "/signature/python-net/esign/jpeg/"
          description: "Agrega varios tipos de firmas a formatos de archivo soportados"

        # operation loop 2
        - name: "Agregar texto a documentos"
          operation: "text"
          link: "/signature/python-net/text/jpeg/"
          description: "Mejora el contenido del documento con firmas de texto personalizables"

        # operation loop 3
        - name: "Firmas de imagen"
          operation: "image"
          link: "/signature/python-net/image/jpeg/"
          description: "Coloca cualquier imagen en cualquier posición dentro de un documento"

        # operation loop 4
        - name: "Generar códigos de barras"
          operation: "barcode"
          link: "/signature/python-net/barcode/jpeg/"
          description: "Crear e insertar varios códigos de barras en documentos soportados"

        # operation loop 5
        - name: "Generar códigos QR"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/jpeg/"
          description: "Generar y utilizar códigos QR para la firma de documentos"
          
        # operation loop 6
        - name: "Certificados digitales"
          operation: "digital"
          link: "/signature/python-net/digital/pdf/"
          description: "Asegura negocios y firma documentos con certificados digitales"

        # operation loop 7
        - name: "Firmas de sello"
          operation: "stamp"
          link: "/signature/python-net/stamp/jpeg/"
          description: "Utiliza el Constructor de Sellos para crear sellos personalizados redondos o cuadrados"
          
        # operation loop 8
        - name: "Buscar firmas"
          operation: "search"
          link: "/signature/python-net/search/pdf/"
          description: "Ubica cualquier firma previamente añadida dentro de un documento"
          
        # operation loop 9
        - name: "Verificación de firmas"
          operation: "verify"
          link: "/signature/python-net/verify/pdf/"
          description: "Verifica la autenticidad de las firmas después de que se han aplicado"
          
        # operation loop 10
        - name: "Modificar firmas"
          operation: "modify"
          link: "/signature/python-net/modify/pdf/"
          description: "Edita fácilmente una variedad de firmas dentro de un documento"
          
        # operation loop 11
        - name: "Eliminar firmas"
          operation: "delete"
          link: "/signature/python-net/delete/pdf/"
          description: "Remueve una amplia gama de firmas aplicadas previamente"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Incrustar firmas de texto en múltiples formatos"
    exclude: "JPEG"
    description: "Con la API de Python via .NET, puedes añadir firmas de texto a varios documentos de Office, dándote control total sobre el ciclo de vida del documento y mejorando la seguridad."
    items: 
          
        # format loop 1
        - name: "Firmas de texto PDF"
          format: "PDF"
          link: "/signature/python-net/text/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 2
        - name: "Firmas de texto DOCX"
          format: "DOCX"
          link: "/signature/python-net/text/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Firmas de texto JPEG"
          format: "JPEG"
          link: "/signature/python-net/text/jpeg/"
          description: "Imagen JPEG"
          
        # format loop 4
        - name: "Firmas de texto PPTX"
          format: "PPTX"
          link: "/signature/python-net/text/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 5
        - name: "Firmas de texto XLSX"
          format: "XLSX"
          link: "/signature/python-net/text/xlsx/"
          description: "Hoja de Cálculo XML Abierto de Microsoft Excel"


          

---