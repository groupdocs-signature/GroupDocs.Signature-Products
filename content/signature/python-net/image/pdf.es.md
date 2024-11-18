



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:52
draft: false
lang: es
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Inserta firmas de imagen en archivos PDF con Python"
head_description: "Incorpora firmas de imagen en documentos PDF para Python utilizando solo unas pocas líneas de código. Utiliza la API de GroupDocs.Signature for Python via .NET para añadir firmas basadas en imágenes de forma sencilla."

############################# Header ############################
title: "Añade firmas de imagen a PDF" 
description: "Utiliza GroupDocs.Signature for Python via .NET para integrar firmas de imagen en diversos formatos de documentos de oficina, incluyendo PDF, Word, Excel y archivos de imagen. Incluir una imagen de la firma de tu gerente mejora el profesionalismo, aumentando tanto el impacto visual como la autenticidad del documento."
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
    title: "Explora GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "Aprende más"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) ofrece opciones versátiles para incrustar firmas de imagen en cualquier lugar dentro de tus documentos empresariales. Optimiza los flujos de trabajo añadiendo imágenes a PDFs, documentos de Word, hojas de Excel, presentaciones de PowerPoint y formatos de imagen populares utilizando nuestra poderosa biblioteca.

############################# Steps ############################
steps:
    enable: true
    title: "Cómo insertar una firma de imagen en un archivo PDF utilizando Python"
    content: |
      Utiliza [GroupDocs.Signature](/signature/python-net/) para dotar a las aplicaciones Python via .NET de la capacidad de añadir con precisión firmas de imagen en cualquier lugar de los documentos PDF. Mejora tu producto integrando nuestra solución.
      
      1. Crea una instancia de Signature con el documento PDF.
      2. Configura ImageSignOptions con la imagen deseada para la firma.
      3. Posiciona la imagen en la ubicación elegida dentro del documento.
      4. Guarda el documento firmado en la ubicación especificada.
   
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

            # Inicializa Signature con la ruta del documento
            with sg.Signature('input.pdf') as signature:

                # Configura ImageSignOptions con la imagen elegida para la firma
                options = sg.ImageSignOptions("company_logo.jpg")

                # Posiciona la imagen en la esquina superior izquierda de cada página
                options.AllPages = True
                options.Left = 100
                options.Top = 200
                
                # Guarda el documento firmado
                result = signature.Sign("output.pdf", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Características integrales de firma de documentos"
  description: "Nuestra API admite una amplia gama de funcionalidades de firma. Puedes agregar, actualizar, eliminar, buscar y validar diferentes tipos de firmas, incluidas las firmas basadas en imágenes."
  image: "/img/signature/features_image.webp" # 500x500 px
  image_description: "Integración de Firma de Imagen"
  features:
    # feature loop
    - title: "Inserta imágenes en documentos de oficina"
      content: "Incorpora firmas electrónicas e imágenes en cualquier punto elegido dentro de un documento. Mejora tus documentos con imágenes, códigos de barras, texto, metadatos o certificados digitales para mejorar la funcionalidad y la seguridad."

    # feature loop
    - title: "Búsqueda y validación de firmas"
      content: "Garantiza la integridad del documento verificando la autenticidad de las firmas. Recupera una lista detallada de todas las firmas dentro de un documento y evalúa sus propiedades individuales."

    # feature loop
    - title: "Edita firmas existentes"
      content: "Actualiza fácilmente el contenido, la apariencia, el tamaño o la posición de las firmas dentro de tus documentos para adaptarlas a tus necesidades cambiantes."

    # feature loop
    - title: "Elimina firmas innecesarias"
      content: "Nuestra API proporciona un control total, permitiéndote eliminar firmas de la mayoría de los formatos de archivo compatibles siempre que sea necesario."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Mejora documentos con firmas de imagen"
      content: |
        Aprende cómo insertar firmas de imagen en tus documentos empresariales para enriquecer el contenido.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # Elige el documento que se va a firmar
              with sg.Signature('input.pdf') as signature:

                    # Configura las opciones de imagen con la ruta del archivo de imagen
                    options = sg.ImageSignOptions("manager_signature.jpg")

                    # Especifica el tamaño de la firma de imagen
                    options.Width = 100
                    options.Height = 100

                    # Posiciona la imagen en la esquina inferior derecha de la página
                    options.VerticalAlignment = sg.VerticalAlignment.Bottom
                    options.HorizontalAlignment = sg.HorizontalAlignment.Right

                    # Aplica margen desde los bordes de la página según sea necesario
                    options.Margin = sg.Padding()
                    options.Margin.Bottom = 120
                    options.Margin.Right = 120

                    # Opcionalmente, añade un borde alrededor de la imagen
                    options.Border = sg.Border()
                    options.Border.Visible = True
                    options.Border.Color = sg.Color.OrangeRed
                    options.Border.DashStyle = sg.DashStyle.DashDotDot
                    options.Border.Weight = 5

                    # Rota la imagen para asegurar una alineación adecuada
                    options.RotationAngle = 45

                    # Guarda el documento actualizado
                    result = signature.Sign("output.pdf", options)
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
            link: "/examples/signature/formats/signature_image.pdf"
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
    title: "Explora nuestras características"
    exclude: "image"
    description: "Descubre los diferentes tipos de firma y operaciones que ofrece nuestra plataforma."
    items: 
          
        # operation loop 1
        - name: "Firmas electrónicas"
          operation: "esign"
          link: "/signature/python-net/esign/pdf/"
          description: "Agrega varios tipos de firmas a formatos de archivo soportados"

        # operation loop 2
        - name: "Agregar texto a documentos"
          operation: "text"
          link: "/signature/python-net/text/pdf/"
          description: "Mejora el contenido del documento con firmas de texto personalizables"

        # operation loop 3
        - name: "Firmas de imagen"
          operation: "image"
          link: "/signature/python-net/image/pdf/"
          description: "Coloca cualquier imagen en cualquier posición dentro de un documento"

        # operation loop 4
        - name: "Generar códigos de barras"
          operation: "barcode"
          link: "/signature/python-net/barcode/pdf/"
          description: "Crear e insertar varios códigos de barras en documentos soportados"

        # operation loop 5
        - name: "Generar códigos QR"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/pdf/"
          description: "Generar y utilizar códigos QR para la firma de documentos"
          
        # operation loop 6
        - name: "Certificados digitales"
          operation: "digital"
          link: "/signature/python-net/digital/pdf/"
          description: "Asegura negocios y firma documentos con certificados digitales"

        # operation loop 7
        - name: "Firmas de sello"
          operation: "stamp"
          link: "/signature/python-net/stamp/pdf/"
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
    title: "Incorpora imágenes en múltiples formatos de archivo"
    exclude: "PDF"
    description: "Utiliza la API de Python via .NET para insertar imágenes en varios formatos de documento. Redimensiona, posiciona, selecciona páginas específicas y aplica firmas basadas en imágenes, dándote control total sobre el diseño de tu documento."
    items: 
          
        # format loop 1
        - name: "Firmar PDF con imagen"
          format: "PDF"
          link: "/signature/python-net/image/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 2
        - name: "Firmar DOCX con imagen"
          format: "DOCX"
          link: "/signature/python-net/image/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Firmar JPEG con imagen"
          format: "JPEG"
          link: "/signature/python-net/image/jpeg/"
          description: "Imagen JPEG"
          
        # format loop 4
        - name: "Firmar PPTX con imagen"
          format: "PPTX"
          link: "/signature/python-net/image/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 5
        - name: "Firmar XLSX con imagen"
          format: "XLSX"
          link: "/signature/python-net/image/xlsx/"
          description: "Hoja de Cálculo XML Abierto de Microsoft Excel"


          

---