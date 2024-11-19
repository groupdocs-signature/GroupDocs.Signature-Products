



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:22
draft: false
lang: es
format: Pptx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Generar códigos QR para archivos PPTX utilizando Python"
head_description: "Utilice la API GroupDocs.Signature para generar e incrustar códigos QR en archivos PPTX. Coloque códigos QR en cualquier página para agregar funcionalidad adicional."

############################# Header ############################
title: "Generar códigos QR para PPTX" 
description: "Cree códigos de barras 2D utilizando datos textuales o numéricos y aplíquelos a varias páginas y formatos, incluidos PDFs, Word, Excel y más con GroupDocs.Signature for Python via .NET."
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
    title: "Explorar las características de GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "Aprende más"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) ofrece una amplia variedad de capacidades, permitiendo a los usuarios generar e incrustar diferentes tipos de firma en los principales formatos de documentos. Ya se trate de PDFs, Word, Excel, PowerPoint o imágenes, potencie sus documentos con firmas de Texto, Imagen, Código de Barras, Código QR, Metadatos, Digitales o Sello.

############################# Steps ############################
steps:
    enable: true
    title: "Pasos para generar e insertar un código QR en PPTX"
    content: |
      [GroupDocs.Signature](/signature/python-net/) le permite crear códigos QR en formatos populares y ubicarlos en páginas PPTX. Con soporte para más de 10 tipos de códigos QR, puede integrar esta funcionalidad sin problemas en aplicaciones Python via .NET. Mejore sus documentos con firmas de códigos QR usando nuestro producto.
      
      1. Obtenga el archivo o flujo PPTX donde se añadirá el código QR.
      2. Proporcione el texto requerido a QrCodeSignOptions.
      3. Personalice configuraciones visuales como color, posición y tamaño.
      4. Guarde el documento con el código QR incrustado.
   
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

            # Inicialice una nueva instancia de Signature con el documento
            with sg.Signature('input.pptx') as signature:

                # Utilice QrCodeSignOptions para incrustar un código QR en el documento
                options = sg.QrCodeSignOptions("Text Content")

                # Especifique el tipo de firma y establezca su posición en la página
                options.EncodeType = sg.QrCodeTypes.QR
                options.Left = 50
                options.Top = 150

                # Guarde el documento con el código QR incrustado
                result = signature.Sign("output.pptx", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Integración completa de firma para documentos"
  description: "Con la API GroupDocs.Signature for Python via .NET, los usuarios pueden generar, modificar, buscar, validar y eliminar diferentes tipos de firma, simplificando los flujos de trabajo documentales con precisión."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "Características clave de GroupDocs.Signature"
  features:
    # feature loop
    - title: "Aplicar múltiples tipos de firma"
      content: "GroupDocs.Signature permite la aplicación de firmas de Texto, Imagen, Código de Barras, Código QR y Sello a cualquier documento. Puede colocar las firmas con precisión en cualquier página y gestionar los metadatos de manera sencilla. Proteja sus documentos de cambios no autorizados con certificados digitales."

    # feature loop
    - title: "Buscar y validar firmas"
      content: "Verifique las firmas de documentos para autenticar y asegurar su precisión usando herramientas avanzadas de validación. Obtenga fácilmente una lista detallada de todas las firmas incrustadas en un documento para una mejor supervisión."

    # feature loop
    - title: "Modificar firmas existentes"
      content: "Puede actualizar las firmas aplicadas previamente ajustando su contenido, posición, color, tamaño y otros atributos para satisfacer sus necesidades específicas."

    # feature loop
    - title: "Eliminar firmas rápidamente"
      content: "Agilice la gestión de documentos eliminando rápidamente las firmas no deseadas. Ya sea un certificado digital u otro tipo de firma, la eliminación se puede realizar de manera eficiente."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Personalizar un código QR generado"
      content: |
        Este ejemplo muestra cómo colocar un código QR personalizado en una página PPTX.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # Obtenga el documento que se va a firmar y páselo a Signature
              with sg.Signature('input.pptx') as signature:

                    # Configure las opciones del código QR con el texto requerido
                    options = sg.QrCodeSignOptions("Archived on July 11, 2019")

                    # Establezca la posición del código QR en la página
                    options.VerticalAlignment = sg.Domain.VerticalAlignment.Top
                    options.HorizontalAlignment = sg.Domain.HorizontalAlignment.Right

                    # Establezca el relleno para la firma
                    options.Margin = sg.Padding()
                    options.Margin.Top = 20
                    options.Margin.Right = 20

                    # Elija el color del código QR
                    options.ForeColor = sg.Color.Red

                    # Defina las opciones de fuente para el mensaje
                    options.Font = sg.SignatureFont()
                    options.Font.Size = 12
                    options.Font.FamilyName = "Comic Sans MS"

                    # Establezca el color de fondo y el pincel para el código QR
                    options.Background = sg.Background()
                    options.Background.Color = Color.LimeGreen
                    options.Background.Transparency = 0.5
                    options.Background.Brush = sg.LinearGradientBrush(sg.Color.LimeGreen, sg.Color.DarkGreen)

                    # Incruste el código QR en el documento
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
            link: "/examples/signature/formats/signature_qrcode.pptx"
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
    title: "Explore nuestras soluciones de firma"
    exclude: "qrcode"
    description: "Ofrecemos una amplia variedad de tipos de firma y operaciones para satisfacer sus necesidades documentales."
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
    title: "Incrustar códigos QR en varios formatos de documento"
    exclude: "PPTX"
    description: "Utilice la API Python via .NET para incrustar códigos QR en cualquier formato de documento estándar de la industria. Almacene y codifique información importante en códigos de barras 2D para un escaneo y recuperación de datos sencillos."
    items: 
          
        # format loop 1
        - name: "Código QR para PDF"
          format: "PDF"
          link: "/signature/python-net/qrcode/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 2
        - name: "Código QR para DOCX"
          format: "DOCX"
          link: "/signature/python-net/qrcode/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Código QR para JPEG"
          format: "JPEG"
          link: "/signature/python-net/qrcode/jpeg/"
          description: "Imagen JPEG"
          
        # format loop 4
        - name: "Código QR para PPTX"
          format: "PPTX"
          link: "/signature/python-net/qrcode/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 5
        - name: "Código QR para XLSX"
          format: "XLSX"
          link: "/signature/python-net/qrcode/xlsx/"
          description: "Hoja de Cálculo XML Abierto de Microsoft Excel"


          

---