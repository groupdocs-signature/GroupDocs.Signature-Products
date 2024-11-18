



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:10
draft: false
lang: es
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Firma XLSX electrónicamente a través de C#"
head_description: "Utiliza XLSX para añadir una variedad de tipos de firmas electrónicas a documentos, garantizando seguridad y cumplimiento en formatos como PDF, Word, Excel, Presentaciones e Imágenes."

############################# Header ############################
title: "Firma electrónica de archivos XLSX" 
description: "Incorpora una variedad de firmas electrónicas en tus documentos utilizando GroupDocs.Signature for .NET, asegurando cumplimiento e integridad para formatos como PDFs, Word, Excel, Presentaciones e Imágenes."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Descargar gratis"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "Acerca de la API GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "Aprende más"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) ofrece un conjunto integral de capacidades de firma electrónica. Con ella, puedes agregar, buscar, verificar, actualizar y eliminar firmas digitales a través de una amplia variedad de tipos de documentos, sin necesidad de herramientas de terceros. Soporta la firma de archivos PDF, documentos de Word, hojas de cálculo de Excel, presentaciones de PowerPoint y diversos formatos de imagen sin complicaciones.

############################# Steps ############################
steps:
    enable: true
    title: "Pasos para firmar XLSX utilizando C#"
    content: |
      [GroupDocs.Signature](/signature/net/) facilita la incorporación de firmas personalizadas en archivos XLSX. Los desarrolladores de .NET pueden integrar sin problemas la funcionalidad de firma en sus aplicaciones usando nuestro software.
      
      1. Proporciona el archivo XLSX a la instancia Signature para su firma.
      2. Utiliza SignOptions para especificar los parámetros de la firma.
      3. Configura atributos como tamaño, color y contenido.
      4. Guarda el archivo firmado en el destino deseado.
   
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
        // Carga el documento en una instancia de Signature
        using (Signature signature = new Signature("input.xlsx"))
        {
            // Crea un nuevo objeto QrCodeSignOptions
            QrCodeSignOptions options = new QrCodeSignOptions("QR code text")
            {
                // Configura todas las opciones necesarias
                Left = 50,
                Top = 200,
                ForeColor = Color.Red
            };

            // Guarda el documento firmado en el almacenamiento local
            SignResult result = signature.Sign("output.xlsx", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Firmas electrónicas avanzadas para documentos"
  description: "Nuestra sofisticada API de firma electrónica mejora los flujos de trabajo empresariales, permitiendo la firma, validación, modificación y gestión de firmas electrónicas con capacidades de automatización total."
  image: "/img/signature/features_esign.webp" # 500x500 px
  image_description: "Capacidades de firma electrónica"
  features:
    # feature loop
    - title: "Firma electrónica para documentos de oficina"
      content: "Inserta sin dificultades firmas electrónicas en cualquier posición dentro de un documento. Personaliza y enriquece el contenido con certificados digitales, metadatos, códigos de barras o elementos visuales, asegurando autenticidad y seguridad."

    # feature loop
    - title: "Gestión integral de firmas"
      content: "Una vez firmados, los documentos pueden ser procesados adicionalmente sin complicaciones. Accede a una visión completa de las firmas existentes, permitiendo actualizaciones precisas o eliminación de firmas cuando sea necesario."

    # feature loop
    - title: "Seguridad mejorada del contenido"
      content: "Protege la integridad de tus documentos utilizando certificados digitales. Incorpora o extrae metadatos para un mejor seguimiento y auditoría de documentos, asegurando cumplimiento y autenticidad del contenido."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cómo agregar una firma de imagen a un documento"
      content: |
        Este ejemplo ilustra el procedimiento para aplicar una firma de imagen a una página específica dentro de un documento.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Proporciona el documento fuente como un argumento
          using (Signature signature = new Signature("input.xlsx"))
          {
              // Especifica la ruta a la imagen en la configuración de la firma
              ImageSignOptions options = new ImageSignOptions("image.jpg")
              {
                  // Define las dimensiones y las páginas objetivo para la firma
                  VerticalAlignment = VerticalAlignment.Bottom,
                  HorizontalAlignment = HorizontalAlignment.Right,
                  Height = 150,
                  Width = 200,
                  Margin = new Padding(50),
                  AllPages = true
              };

              // Ejecuta la aplicación de la firma al documento
              SignResult result = signature.Sign("output.xlsx", options);
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
            link: "/examples/signature/formats/signature_esign.xlsx"
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
    title: "Explora el conjunto completo de nuestras funcionalidades"
    exclude: "esign"
    description: "Estamos orgullosos de ofrecer una vasta gama de opciones de firma y operaciones asociadas."
    items: 
          
        # operation loop 1
        - name: "Firmas electrónicas"
          operation: "esign"
          link: "/signature/net/esign/xlsx/"
          description: "Agrega varios tipos de firmas a formatos de archivo soportados"

        # operation loop 2
        - name: "Agregar texto a documentos"
          operation: "text"
          link: "/signature/net/text/xlsx/"
          description: "Mejora el contenido del documento con firmas de texto personalizables"

        # operation loop 3
        - name: "Firmas de imagen"
          operation: "image"
          link: "/signature/net/image/xlsx/"
          description: "Coloca cualquier imagen en cualquier posición dentro de un documento"

        # operation loop 4
        - name: "Generar códigos de barras"
          operation: "barcode"
          link: "/signature/net/barcode/xlsx/"
          description: "Crear e insertar varios códigos de barras en documentos soportados"

        # operation loop 5
        - name: "Generar códigos QR"
          operation: "qrcode"
          link: "/signature/net/qrcode/xlsx/"
          description: "Generar y utilizar códigos QR para la firma de documentos"
          
        # operation loop 6
        - name: "Certificados digitales"
          operation: "digital"
          link: "/signature/net/digital/xlsx/"
          description: "Asegura negocios y firma documentos con certificados digitales"

        # operation loop 7
        - name: "Firmas de sello"
          operation: "stamp"
          link: "/signature/net/stamp/xlsx/"
          description: "Utiliza el Constructor de Sellos para crear sellos personalizados redondos o cuadrados"
          
        # operation loop 8
        - name: "Buscar firmas"
          operation: "search"
          link: "/signature/net/search/xlsx/"
          description: "Ubica cualquier firma previamente añadida dentro de un documento"
          
        # operation loop 9
        - name: "Verificación de firmas"
          operation: "verify"
          link: "/signature/net/verify/xlsx/"
          description: "Verifica la autenticidad de las firmas después de que se han aplicado"
          
        # operation loop 10
        - name: "Modificar firmas"
          operation: "modify"
          link: "/signature/net/modify/xlsx/"
          description: "Edita fácilmente una variedad de firmas dentro de un documento"
          
        # operation loop 11
        - name: "Eliminar firmas"
          operation: "delete"
          link: "/signature/net/delete/xlsx/"
          description: "Remueve una amplia gama de firmas aplicadas previamente"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Firma digitalmente una amplia gama de formatos de archivo"
    exclude: "XLSX"
    description: "La API .NET te permite firmar electrónicamente más de 60 formatos de archivo estándar de la industria, ofreciendo una flexibilidad sin igual en la seguridad de tus documentos comerciales."
    items: 
          
        # format loop 1
        - name: "Firma electrónica PDF"
          format: "PDF"
          link: "/signature/net/esign/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 2
        - name: "Firma electrónica DOCX"
          format: "DOCX"
          link: "/signature/net/esign/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Firma electrónica JPEG"
          format: "JPEG"
          link: "/signature/net/esign/jpeg/"
          description: "Imagen JPEG"
          
        # format loop 4
        - name: "Firma electrónica PPTX"
          format: "PPTX"
          link: "/signature/net/esign/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 5
        - name: "Firma electrónica XLSX"
          format: "XLSX"
          link: "/signature/net/esign/xlsx/"
          description: "Hoja de Cálculo XML Abierto de Microsoft Excel"


          

---