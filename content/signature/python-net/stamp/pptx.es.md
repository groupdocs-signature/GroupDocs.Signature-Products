



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:07
draft: false
lang: es
format: Pptx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Crea sellos redondos y cuadrados en PPTX usando Python"
head_description: "Genera e inserta sellos personalizados en archivos PPTX con la API GroupDocs.Signature for Python via .NET."

############################# Header ############################
title: "Crea sellos para PPTX" 
description: "Agrega sellos diseñados a medida en cualquier parte de tus documentos con GroupDocs.Signature for Python via .NET, ofreciendo gran flexibilidad para la ubicación y configuración que se adapta a tus necesidades empresariales."
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
    title: "Descripción general de GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "Aprende más"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) es una herramienta integral que te permite insertar varios tipos de firma en documentos, incluidos sellos personalizados. Con soporte para más de 60 formatos de archivo, desde PDFs y documentos de Word hasta imágenes y archivos ZIP, puedes mejorar tus documentos con texto, imágenes, códigos de barras, metadatos, certificados digitales y sellos. También tienes completo control para buscar, verificar, editar o eliminar cualquier firma aplicada.

############################# Steps ############################
steps:
    enable: true
    title: "Cómo agregar un sello a PPTX usando Python"
    content: |
      [GroupDocs.Signature](/signature/python-net/) proporciona robustas herramientas de creación de sellos para mejorar aplicaciones Python via .NET. Úsalo para diseñar e implementar sellos personalizados para las páginas de tus documentos.
      
      1. Proporciona el documento PPTX que deseas sellar.
      2. Usa StampSignOptions para configurar todas las configuraciones necesarias.
      3. Agrega múltiples líneas de sello si es necesario.
      4. Aplica el sello y guarda el documento actualizado.
   
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

            # Adjunta la ruta del documento a la instancia de Signature
            with sg.Signature('input.pptx') as signature:

                # Configura StampSignOptions con los detalles necesarios del sello
                options = sg.StampSignOptions()
                options.Height = 180
                options.Width = 180

                # Agrega una o más líneas al sello
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

                # Guarda el documento con el sello aplicado
                result = signature.Sign("output.pptx", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Utiliza firmas para asegurar y mejorar la integridad del documento"
  description: "Con la biblioteca GroupDocs.Signature for Python via .NET, puedes agregar funcionalidad de firma a tus documentos sin problemas. Crea, modifica, verifica o elimina sellos personalizados y otros tipos de firma, proporcionando flexibilidad y seguridad para tus flujos de trabajo documentales."
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "Firmas de sello impulsadas por GroupDocs.Signature"
  features:
    # feature loop
    - title: "Firma completa del documento"
      content: "Eleva tus documentos agregando firmas como texto, imágenes, códigos de barras, códigos QR y sellos en cualquier posición de cualquier página. Gestiona metadatos incrustados y aplica certificados digitales para proteger contra cambios no autorizados."

    # feature loop
    - title: "Búsqueda y verificación de firmas eficientes"
      content: "Después de firmar, usa herramientas de búsqueda avanzadas para encontrar todas las firmas incrustadas. Verifica o gestiona fácilmente los datos de firma para asegurar la integridad del documento."

    # feature loop
    - title: "Editar y personalizar firmas"
      content: "Realiza cambios en las firmas previamente agregadas. Ya sea que desees cambiar el contenido, la posición, el tamaño o el color, GroupDocs.Signature for Python via .NET te brinda el control total para ajustar las firmas según sea necesario."

    # feature loop
    - title: "Eliminar firmas fácilmente"
      content: "Si necesitas eliminar firmas, GroupDocs.Signature for Python via .NET ofrece todas las herramientas necesarias para eliminar cualquier tipo, incluidos sellos y certificados digitales, ayudándote a mantener tus documentos actualizados y en cumplimiento."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cómo agregar sellos personalizados a documentos"
      content: |
        Este ejemplo muestra cómo crear e insertar sellos personalizados con detalles de texto específicos en un documento.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # Proporciona el documento que deseas sellar
              with sg.Signature('input.pptx') as signature:

                    # Configura las opciones del sello con tus ajustes deseados
                    options = sg.StampSignOptions()

                    # Define el tamaño y la colocación del sello en la página
                    options.Height = 200
                    options.Width = 200
                    options.VerticalAlignment = sg.VerticalAlignment.Bottom
                    options.HorizontalAlignment = sg.HorizontalAlignment.Right
                    options.AllPages = True

                    # Agrega líneas circulares externas con texto
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

                    # Opcionalmente, agrega líneas cuadradas internas
                    innerLine = sg.StampLine()
                    innerLine.Text = "Company #1"
                    innerLine.TextColor = sg.Color.MediumVioletRed
                    innerLine.Font = sg.SignatureFont()
                    innerLine.Font.Size = 20
                    innerLine.Font.Bold = True
                    innerLine.Height = 40
                    options.InnerLines.Add(innerLine)

                    # Finaliza y guarda el documento sellado
                    result = signature.Sign("output.pptx", options)
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
            link: "/examples/signature/formats/signature_stamp.pptx"
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
    title: "Explora características clave"
    exclude: "stamp"
    description: "Encuentra una amplia gama de opciones para crear, gestionar y eliminar firmas, brindándote control total sobre los flujos de trabajo documentales."
    items: 
          
        # operation loop 1
        - name: "Firmas electrónicas"
          operation: "esign"
          link: "/signature/python-net/esign/pptx/"
          description: "Agrega varios tipos de firmas a formatos de archivo soportados"

        # operation loop 2
        - name: "Agregar texto a documentos"
          operation: "text"
          link: "/signature/python-net/text/pptx/"
          description: "Mejora el contenido del documento con firmas de texto personalizables"

        # operation loop 3
        - name: "Firmas de imagen"
          operation: "image"
          link: "/signature/python-net/image/pptx/"
          description: "Coloca cualquier imagen en cualquier posición dentro de un documento"

        # operation loop 4
        - name: "Generar códigos de barras"
          operation: "barcode"
          link: "/signature/python-net/barcode/pptx/"
          description: "Crear e insertar varios códigos de barras en documentos soportados"

        # operation loop 5
        - name: "Generar códigos QR"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/pptx/"
          description: "Generar y utilizar códigos QR para la firma de documentos"
          
        # operation loop 6
        - name: "Certificados digitales"
          operation: "digital"
          link: "/signature/python-net/digital/pptx/"
          description: "Asegura negocios y firma documentos con certificados digitales"

        # operation loop 7
        - name: "Firmas de sello"
          operation: "stamp"
          link: "/signature/python-net/stamp/pptx/"
          description: "Utiliza el Constructor de Sellos para crear sellos personalizados redondos o cuadrados"
          
        # operation loop 8
        - name: "Buscar firmas"
          operation: "search"
          link: "/signature/python-net/search/pptx/"
          description: "Ubica cualquier firma previamente añadida dentro de un documento"
          
        # operation loop 9
        - name: "Verificación de firmas"
          operation: "verify"
          link: "/signature/python-net/verify/pptx/"
          description: "Verifica la autenticidad de las firmas después de que se han aplicado"
          
        # operation loop 10
        - name: "Modificar firmas"
          operation: "modify"
          link: "/signature/python-net/modify/pptx/"
          description: "Edita fácilmente una variedad de firmas dentro de un documento"
          
        # operation loop 11
        - name: "Eliminar firmas"
          operation: "delete"
          link: "/signature/python-net/delete/pptx/"
          description: "Remueve una amplia gama de firmas aplicadas previamente"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Aplica sellos a varios formatos de documentos"
    exclude: "PPTX"
    description: "Con la API GroupDocs.Signature, puedes insertar sellos personalizados en más de 60 tipos de archivos estándar. Aplica sellos en cualquier lugar de tus documentos, mejorando la personalización y el seguimiento."
    items: 
          
        # format loop 1
        - name: "Sellar PDF"
          format: "PDF"
          link: "/signature/python-net/stamp/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 2
        - name: "Sellar DOCX"
          format: "DOCX"
          link: "/signature/python-net/stamp/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Sellar JPEG"
          format: "JPEG"
          link: "/signature/python-net/stamp/jpeg/"
          description: "Imagen JPEG"
          
        # format loop 4
        - name: "Sellar PPTX"
          format: "PPTX"
          link: "/signature/python-net/stamp/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 5
        - name: "Sellar XLSX"
          format: "XLSX"
          link: "/signature/python-net/stamp/xlsx/"
          description: "Hoja de Cálculo XML Abierto de Microsoft Excel"


          

---