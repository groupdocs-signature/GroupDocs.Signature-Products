



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:06
draft: false
lang: es
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Generar código de barras para XLSX utilizando la API C#"
head_description: "Genera una firma de código de barras y asegura el documento XLSX utilizando C# con solo unas pocas líneas de código. Utiliza GroupDocs.Signature para firmar una amplia gama de formatos de archivo."

############################# Header ############################
title: "Generar código de barras para documentos XLSX" 
description: "Aprovecha GroupDocs.Signature for .NET para colocar códigos de barras en cualquier parte de tus documentos comerciales. Nuestra API ofrece amplias opciones de personalización para las firmas de códigos de barras."
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
    title: "Descripción general de GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "Aprende más"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) es una solución sofisticada para la firma de documentos que admite una amplia variedad de tipos de firma, incluyendo texto, imágenes, códigos de barras, certificados digitales y sellos. Compatible con más de 60 formatos de archivo, como PDF, MS Office, imágenes, archivos ZIP y más, esta herramienta te permite no solo aplicar firmas, sino también buscarlas, verificarlas, modificarlas o eliminarlas según sea necesario.

############################# Steps ############################
steps:
    enable: true
    title: "Pasos para generar e incrustar un código de barras en un archivo XLSX"
    content: |
      [GroupDocs.Signature](/signature/net/) facilita la generación de códigos de barras en numerosos formatos populares y su colocación en páginas de XLSX. Con más de 60 tipos de códigos de barras compatibles, las aplicaciones .NET se pueden ampliar sin esfuerzo con funciones de firma de códigos de barras al integrar nuestra biblioteca.
      
      1. Proporciona el archivo o flujo XLSX para su procesamiento.
      2. Pasa el texto del código de barras a la instancia BarcodeSignOptions.
      3. Ajusta las opciones del código de barras, como posición, tamaño, etc.
      4. Guarda el archivo con el código de barras recién agregado.
   
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
        // Crea un nuevo objeto Signature con la ruta del documento
        using (Signature signature = new Signature("input.xlsx"))
        {
            // Emplea BarcodeSignOptions para agregar un código de barras al documento
            BarcodeSignOptions options = new BarcodeSignOptions("Business data")
            {
                // Configura el tipo de código de barras y propiedades adicionales
                EncodeType = BarcodeTypes.Code128,
                Left = 50,
                Top = 150
            };

            // Guarda el archivo firmado
            SignResult result = signature.Sign("output.xlsx", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Mejora y protege tus documentos con capacidades avanzadas de firma"
  description: "La biblioteca GroupDocs.Signature for .NET está diseñada para facilitar la firma y el procesamiento de documentos de manera integral a través de formatos de archivo ampliamente utilizados. Puedes agregar, ajustar, verificar o eliminar diferentes tipos de firmas con facilidad."
  image: "/img/signature/features_barcode.webp" # 500x500 px
  image_description: "Características clave de GroupDocs.Signature"
  features:
    # feature loop
    - title: "Firma de documentos versátil"
      content: "Firma eficientemente cualquier página dentro de documentos compatibles usando texto, imágenes, códigos de barras, códigos QR o sellos. Además, puedes incrustar metadatos ocultos, como datos EXIF en imágenes, o proteger el contenido de tu documento contra alteraciones no autorizadas usando certificados digitales."

    # feature loop
    - title: "Búsqueda y verificación de firmas completas"
      content: "Nuestra herramienta ofrece funcionalidades robustas para trabajar con documentos firmados. Asegura la integridad de tus documentos verificando firmas, y recupera fácilmente una lista completa de todas las firmas dentro de un documento a través de nuestra función de búsqueda."

    # feature loop
    - title: "Edición de firmas sin complicaciones"
      content: "Casi todas las firmas aplicadas previamente pueden ser modificadas. Actualiza convenientemente el texto, ajusta la posición o cambia los colores según tus necesidades."

    # feature loop
    - title: "Eliminación eficiente de firmas"
      content: "Nuestro enfoque admite por completo operaciones CRUD para firmas, lo que permite la rápida eliminación de cualquier firma no deseada o desactualizada de tus documentos."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cómo generar una firma de código de barras"
      content: |
        Este ejemplo muestra cómo incrustar un código de barras personalizado en las páginas de un documento XLSX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          using (Signature signature = new Signature("input.xlsx"))
          {
              // Formula las opciones de firma con el texto deseado
              BarcodeSignOptions options = new BarcodeSignOptions("Accepted")
              {
                  EncodeType = BarcodeTypes.Code39FullASCII,

                  // Determina la posición relativa del código de barras en la página
                  VerticalAlignment = Domain.VerticalAlignment.Top,
                  HorizontalAlignment = Domain.HorizontalAlignment.Left,

                  // Define el relleno del código de barras desde el borde de la página
                  Margin = new Padding() { Top = 180, Right = 20 },

                  // Especifica el color de las barras
                  ForeColor = Color.Red,

                  // Selecciona el estilo de fuente del mensaje
                  Font = new SignatureFont { Size = 12, FamilyName = "Arial" },

                  // Indica la posición del mensaje
                  CodeTextAlignment = CodeTextAlignment.Above
              };

              // Firma y guarda el documento
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
            link: "/examples/signature/formats/signature_barcode.xlsx"
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
    title: "Descubre nuestras características principales"
    exclude: "barcode"
    description: "Ofrecemos una impresionante selección de opciones y operaciones de firma."
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
    title: "Firma documentos en una variedad de formatos"
    exclude: "XLSX"
    description: "Nuestra API .NET admite la firma de más de 60 formatos diferentes. Coloca sin esfuerzo varios tipos de firmas en cualquier página o en cualquier posición deseada dentro de tus documentos."
    items: 
          
        # format loop 1
        - name: "Agregar código de barras a PDF"
          format: "PDF"
          link: "/signature/net/barcode/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 2
        - name: "Agregar código de barras a DOCX"
          format: "DOCX"
          link: "/signature/net/barcode/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Agregar código de barras a JPEG"
          format: "JPEG"
          link: "/signature/net/barcode/jpeg/"
          description: "Imagen JPEG"
          
        # format loop 4
        - name: "Agregar código de barras a PPTX"
          format: "PPTX"
          link: "/signature/net/barcode/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 5
        - name: "Agregar código de barras a XLSX"
          format: "XLSX"
          link: "/signature/net/barcode/xlsx/"
          description: "Hoja de Cálculo XML Abierto de Microsoft Excel"


          

---