



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:08
draft: false
lang: es
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Incorporar un código de barras en su JPEG con Python"
head_description: "Agregue de manera eficiente firmas de códigos de barras a documentos JPEG con unas pocas líneas en Python. GroupDocs.Signature ofrece soluciones de firma integradas para múltiples formatos de documentos."

############################# Header ############################
title: "Generar códigos de barras para JPEG" 
description: "Con GroupDocs.Signature for Python via .NET, puede colocar códigos de barras en sus documentos comerciales donde sea necesario. Nuestra solución proporciona opciones flexibles para la personalización de firmas de códigos de barras."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Prueba gratuita"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "Acerca de GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "Aprende más"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) es una poderosa herramienta de firma de documentos que admite una amplia gama de tipos de firma, incluidos texto, imágenes, códigos de barras, certificados digitales y sellos. Compatible con más de 60 formatos de archivo, como PDF, MS Office, imágenes, ZIP y más, no solo le permite aplicar firmas, sino que también le permite buscar, verificar, modificar o eliminarlas según sea necesario.

############################# Steps ############################
steps:
    enable: true
    title: "Pasos para generar e insertar un código de barras en JPEG"
    content: |
      [GroupDocs.Signature](/signature/python-net/) le permite generar e incrustar códigos de barras en documentos JPEG de manera rápida y eficiente. Al admitir más de 60 formatos de códigos de barras, las aplicaciones Python via .NET pueden agregar funcionalidad de firma de código de barras integrando nuestra biblioteca.
      
      1. Proporcione el archivo o flujo de JPEG para procesar.
      2. Asigne el texto del código de barras al objeto BarcodeSignOptions.
      3. Ajuste las opciones del código de barras, como posición y tamaño.
      4. Guarde el documento con el código de barras incrustado.
   
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

            # Inicializar el objeto Signature con la ruta del documento
            with sg.Signature('input.jpeg') as signature:

                # Utilizar BarcodeSignOptions para agregar un código de barras al documento
                options = sg.BarcodeSignOptions('Business data')

                # Establecer el tipo de código de barras y configurar sus propiedades
                options.EncodeType = sg.BarcodeTypes.Code128
                options.Left = 50
                options.Top = 150

                # Guardar el documento firmado
                result = signature.Sign('output.jpeg', options)
        ```          

############################# More features ############################
more_features:
  enable: true
  title: "Mejore sus documentos con características avanzadas de firma"
  description: "La biblioteca GroupDocs.Signature for Python via .NET proporciona soluciones integrales para firmar y procesar documentos en formatos comúnmente utilizados. Puede agregar, modificar, verificar o eliminar fácilmente varios tipos de firma según sus necesidades."
  image: "/img/signature/features_barcode.webp" # 500x500 px
  image_description: "Características clave de GroupDocs.Signature"
  features:
    # feature loop
    - title: "Firma de documentos flexible"
      content: "Firme cualquier página en documentos admitidos con texto, imágenes, códigos de barras, códigos QR o sellos. Agregue metadatos ocultos como datos EXIF en imágenes y asegure la protección del contenido con certificados digitales para evitar cambios no autorizados."

    # feature loop
    - title: "Buscar y verificar firmas"
      content: "Nuestra herramienta garantiza la integridad de sus documentos al permitir la verificación de firmas. También puede recuperar una lista completa de todas las firmas en un documento para una gestión sencilla."

    # feature loop
    - title: "Editar firmas fácilmente"
      content: "Modifique las firmas existentes sin complicaciones. Ajuste el texto, reubique elementos o cambie colores para adaptarse a las necesidades de su documento."

    # feature loop
    - title: "Eliminar firmas sin esfuerzo"
      content: "Con funcionalidad completa de CRUD, GroupDocs.Signature for Python via .NET facilita la eliminación de cualquier firma no deseada u obsoleta de sus documentos."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Crear y colocar una firma de código de barras"
      content: |
        Este ejemplo demuestra cómo insertar un código de barras personalizado en un documento JPEG.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # Proporcione el documento a firmar
              with sg.Signature('input.jpeg') as signature:

                  # Establecer el texto del código de barras y las opciones de firma
                  options = sg.BarcodeSignOptions('Accepted')
                  options.EncodeType = sg.BarcodeTypes.Code39FullASCII

                  # Elegir la posición del código de barras en la página
                  options.VerticalAlignment = sg.VerticalAlignment.Top
                  options.HorizontalAlignment = sg.HorizontalAlignment.Left

                  # Establecer el relleno entre el código de barras y el borde de la página
                  options.Margin = sg.Padding()
                  options.Margin.Top = 180
                  options.Margin.Right = 20

                  # Especificar el color de las barras del código de barras
                  options.ForeColor = sg.Color.Red

                  # Elegir el estilo de fuente para el mensaje del código de barras
                  options.Font = sg.SignatureFont()
                  options.Font.Size = 12
                  options.Font.FamilyName = 'Arial'

                  # Establecer la posición del texto del mensaje
                  options.CodeTextAlignment = sg.CodeTextAlignment.Above

                  # Firmar y guardar el documento
                  result = signature.Sign('output.jpeg', options)
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
            link: "/examples/signature/formats/signature_barcode.jpeg"
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
    title: "Explore nuestras características clave"
    exclude: "barcode"
    description: "Ofrecemos una amplia gama de opciones de firma y operaciones para sus necesidades documentales."
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
    title: "Firmar documentos en múltiples formatos"
    exclude: "JPEG"
    description: "La API Python via .NET admite la firma de más de 60 formatos de archivo, lo que le permite agregar varios tipos de firmas a cualquier página o ubicación específica dentro de sus documentos."
    items: 
          
        # format loop 1
        - name: "Agregar código de barras a PDF"
          format: "PDF"
          link: "/signature/python-net/barcode/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 2
        - name: "Agregar código de barras a DOCX"
          format: "DOCX"
          link: "/signature/python-net/barcode/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Agregar código de barras a JPEG"
          format: "JPEG"
          link: "/signature/python-net/barcode/jpeg/"
          description: "Imagen JPEG"
          
        # format loop 4
        - name: "Agregar código de barras a PPTX"
          format: "PPTX"
          link: "/signature/python-net/barcode/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 5
        - name: "Agregar código de barras a XLSX"
          format: "XLSX"
          link: "/signature/python-net/barcode/xlsx/"
          description: "Hoja de Cálculo XML Abierto de Microsoft Excel"


          

---