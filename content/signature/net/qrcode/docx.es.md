



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:01
draft: false
lang: es
format: Docx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Generar código QR para archivos DOCX usando C#"
head_description: "Aproveche la API de GroupDocs.Signature para generar códigos QR para archivos DOCX. Incorpore sin problemas códigos QR en cualquier página para mejorar la funcionalidad."

############################# Header ############################
title: "Generar códigos QR para DOCX" 
description: "Genere códigos de barras 2D utilizando datos de texto o numéricos y aplíquelos en múltiples páginas y formatos, incluidos PDF, Word, Excel y más, a través de GroupDocs.Signature for .NET."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Comienza tu prueba gratis"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "Descubre las capacidades de GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "Aprende más"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) ofrece una amplia gama de características, permitiendo a los usuarios generar e incrustar diversos tipos de firmas en los principales formatos de documentos. Ya sean PDFs, documentos de Word, hojas de Excel, presentaciones de PowerPoint o archivos de imagen, puedes realzar tus documentos con firmas de Texto, Imagen, Código de Barras, Código QR, Metadatos, Digitales y de Sello.

############################# Steps ############################
steps:
    enable: true
    title: "Cómo generar e insertar un código QR en cualquier lugar dentro de un DOCX"
    content: |
      [GroupDocs.Signature](/signature/net/) facilita la generación de códigos QR en varios formatos populares y su colocación en páginas DOCX. Con el soporte de más de 10 tipos de códigos QR, nuestra biblioteca se puede integrar sin problemas en aplicaciones de .NET. Mejora tus documentos con firmas de código QR usando nuestro producto.
      
      1. Adquiere el archivo DOCX o flujo que será firmado con un código QR.
      2. Proporciona el texto necesario a QrCodeSignOptions.
      3. Personaliza parámetros visuales como color, posición, tamaño, etc.
      4. Mantén el documento con el código QR incrustado.
   
    code:
      platform: "net"
      copy_title: "Copiar"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Firmas de muestra"
      install:
        command: "dotnet add package GroupDocs.Signature"
        copy_tip: "haz clic para copiar"
        copy_done: "copiado"
      links:
        #  loop
        - title: "Más ejemplos"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET/"
        #  loop
        - title: "Documentación"
          link: "https://docs.groupdocs.com/signature/net/"
          
      content: |
        ```csharp {style=abap}
        // Inicializa una nueva instancia de Signature con el documento
        using (Signature signature = new Signature("input.docx"))
        {
            // Utiliza QrCodeSignOptions para incrustar un código QR en el documento
            QrCodeSignOptions options = new QrCodeSignOptions("Text Content")
                {
                    // Especifica el tipo de firma y designa su posición en la página
                    EncodeType = QrCodeTypes.QR,
                    Left = 50,
                    Top = 150
                };

            // Mantén el documento con el código QR integrado
            SignResult result = signature.Sign("output.docx", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Integración de firma integral para documentos"
  description: "Con la API de GroupDocs.Signature for .NET, los usuarios pueden generar, modificar, buscar, validar y eliminar una variedad de tipos de firma, optimizando los flujos de trabajo documentales con una precisión inigualable."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "Características Clave de GroupDocs.Signature"
  features:
    # feature loop
    - title: "Firma de documentos con múltiples tipos de firma"
      content: "GroupDocs.Signature permite la aplicación de firmas de Texto, Imagen, Código de Barras, Código QR y Sello a cualquier formato de documento. Las firmas se pueden colocar con precisión en cualquier página, y los metadatos se pueden gestionar sin problemas a través de firmas de metadatos. Protege la integridad de tus documentos incorporando certificados digitales que previenen alteraciones no autorizadas."

    # feature loop
    - title: "Búsqueda y validación de firmas"
      content: "Verifica la autenticidad y precisión de las firmas de documentos a través de un avanzado proceso de validación. Recupera fácilmente una lista detallada de todas las firmas incrustadas en un documento para una supervisión completa."

    # feature loop
    - title: "Modificación de firma personalizable"
      content: "Actualiza y perfecciona las firmas aplicadas anteriormente ajustando contenido, ubicación, color, tamaño y otros atributos para satisfacer tus necesidades específicas."

    # feature loop
    - title: "Eliminación eficiente de firmas"
      content: "Optimiza tu gestión documental eliminando programáticamente firmas no deseadas. Ya sea tratando con certificados digitales u otros tipos de firmas, la eliminación se puede realizar de manera rápida y efectiva."
      
  code_samples_ext:
    # code sample ext loop
    - title: "¿Cómo generar un código QR con varias opciones?"
      content: |
        Este ejemplo demuestra cómo colocar un código QR personalizado en una página DOCX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Recupera el documento a firmar y pásalo a Signature
          using (Signature signature = new Signature("input.docx"))
          {
              // Configura las opciones del código QR con el texto necesario
              QrCodeSignOptions options = new QrCodeSignOptions("Archived on July 11, 2019")
              {
                    // Designa la posición relativa del código QR en la página
                    VerticalAlignment = Domain.VerticalAlignment.Top,
                    HorizontalAlignment = Domain.HorizontalAlignment.Right,

                    // Establece el espaciado de la firma
                    Margin = new Padding() { Top = 20, Right = 20 },

                    // Especifica el color del código QR
                    ForeColor = Color.Red,

                    // Define las opciones de fuente para el mensaje
                    Font = new SignatureFont { Size = 12, FamilyName = "Comic Sans MS" },

                    // Personaliza el color de fondo del código QR y la brocha
                    Background = new Background()
                    {
                        Color = Color.LimeGreen,
                        Transparency = 0.5,
                        Brush = new Domain.Extensions.LinearGradientBrush(Color.LimeGreen, Color.DarkGreen)
                    }
              };

              // Incorpora el código QR en el documento
              SignResult result = signature.Sign("output.docx", options);
          }
          ```
        platform: "net"
        copy_title: "Copiar"
        install:
          command: "dotnet add package GroupDocs.Signature"
          copy_tip: "haz clic para copiar"
          copy_done: "copiado"
        top_links:
          #  loop
          - title: "Descargar resultado"
            icon: "download"
            link: "/examples/signature/formats/signature_qrcode.docx"
        links:
          #  loop
          - title: "Más ejemplos"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET/"
          #  loop
          - title: "Documentación"
            link: "https://docs.groupdocs.com/signature/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "¿Listo para empezar?"
  description: "Prueba las funciones de GroupDocs.Signature de forma gratuita o solicita una licencia"
  items:
    #  loop
    - title: "Descarga de Nuget"
      link: "https://releases.groupdocs.com/signature/net/"
      color: "red"
        #  loop
    - title: "Licenciamiento"
      link: "https://purchase.groupdocs.com/pricing/signature/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Conoce nuestras soluciones de firma"
    exclude: "qrcode"
    description: "Presentamos con orgullo una amplia gama de tipos de firma y características operativas"
    items: 
          
        # operation loop 1
        - name: "Firmas electrónicas"
          operation: "esign"
          link: "/signature/net/esign/docx/"
          description: "Agrega varios tipos de firmas a formatos de archivo soportados"

        # operation loop 2
        - name: "Agregar texto a documentos"
          operation: "text"
          link: "/signature/net/text/docx/"
          description: "Mejora el contenido del documento con firmas de texto personalizables"

        # operation loop 3
        - name: "Firmas de imagen"
          operation: "image"
          link: "/signature/net/image/docx/"
          description: "Coloca cualquier imagen en cualquier posición dentro de un documento"

        # operation loop 4
        - name: "Generar códigos de barras"
          operation: "barcode"
          link: "/signature/net/barcode/docx/"
          description: "Crear e insertar varios códigos de barras en documentos soportados"

        # operation loop 5
        - name: "Generar códigos QR"
          operation: "qrcode"
          link: "/signature/net/qrcode/docx/"
          description: "Generar y utilizar códigos QR para la firma de documentos"
          
        # operation loop 6
        - name: "Certificados digitales"
          operation: "digital"
          link: "/signature/net/digital/docx/"
          description: "Asegura negocios y firma documentos con certificados digitales"

        # operation loop 7
        - name: "Firmas de sello"
          operation: "stamp"
          link: "/signature/net/stamp/docx/"
          description: "Utiliza el Constructor de Sellos para crear sellos personalizados redondos o cuadrados"
          
        # operation loop 8
        - name: "Buscar firmas"
          operation: "search"
          link: "/signature/net/search/docx/"
          description: "Ubica cualquier firma previamente añadida dentro de un documento"
          
        # operation loop 9
        - name: "Verificación de firmas"
          operation: "verify"
          link: "/signature/net/verify/docx/"
          description: "Verifica la autenticidad de las firmas después de que se han aplicado"
          
        # operation loop 10
        - name: "Modificar firmas"
          operation: "modify"
          link: "/signature/net/modify/docx/"
          description: "Edita fácilmente una variedad de firmas dentro de un documento"
          
        # operation loop 11
        - name: "Eliminar firmas"
          operation: "delete"
          link: "/signature/net/delete/docx/"
          description: "Remueve una amplia gama de firmas aplicadas previamente"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Generar códigos QR para otros formatos de documento"
    exclude: "DOCX"
    description: "Mejora todos los formatos estándar de la industria con la capacidad de incrustar códigos QR a través de la API de .NET. Almacena y codifica información crítica en códigos de barras 2D para una fácil escaneabilidad y recuperación de datos."
    items: 
          
        # format loop 1
        - name: "Código QR para PDF"
          format: "PDF"
          link: "/signature/net/qrcode/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 2
        - name: "Código QR para DOCX"
          format: "DOCX"
          link: "/signature/net/qrcode/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Código QR para JPEG"
          format: "JPEG"
          link: "/signature/net/qrcode/jpeg/"
          description: "Imagen JPEG"
          
        # format loop 4
        - name: "Código QR para PPTX"
          format: "PPTX"
          link: "/signature/net/qrcode/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 5
        - name: "Código QR para XLSX"
          format: "XLSX"
          link: "/signature/net/qrcode/xlsx/"
          description: "Hoja de Cálculo XML Abierto de Microsoft Excel"


          

---