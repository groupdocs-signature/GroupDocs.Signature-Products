



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:09
draft: false
lang: es
format: Pdf
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Agregar firmas de imagen a archivos PDF con C#"
head_description: "Coloque una firma de imagen en un archivo PDF para .NET utilizando unas pocas líneas de código. Utilice la API de GroupDocs.Signature for .NET para agregar imágenes."

############################# Header ############################
title: "Agregue una firma de imagen a archivos PDF" 
description: "Utilice GroupDocs.Signature for .NET para integrar sin problemas imágenes en una amplia gama de formatos de documentos de oficina, incluidos PDFs, Word, Excel y archivos de imagen. Incorporar una imagen de la firma de su jefe puede crear una impresión profesional destacada, elevando el atractivo visual y la autenticidad de sus documentos."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Descargar gratuitamente"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "Descubra GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "Aprende más"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) ofrece capacidades integrales para incrustar firmas de imagen en cualquier ubicación de cualquier página dentro de sus documentos empresariales. Mejore sus flujos de trabajo operativos integrando imágenes en PDFs, documentos de Word, hojas de cálculo de Excel, presentaciones de PowerPoint y una variedad de formatos de imagen populares a través de nuestra robusta biblioteca.

############################# Steps ############################
steps:
    enable: true
    title: "Cómo agregar una imagen en cualquier lugar de un PDF usando C#"
    content: |
      Utilice [GroupDocs.Signature](/signature/net/) para dotar a las aplicaciones .NET con la capacidad de incrustar firmas con precisión en cualquier página de documentos PDF. Mejore las capacidades de su producto integrando nuestra solución sin problemas.
      
      1. Instancie la clase Signature con el documento PDF.
      2. Utilice ImageSignOptions para especificar la imagen de la firma.
      3. Posicione la imagen con precisión en cualquier ubicación deseada de la página.
      4. Guarde el nuevo documento firmado en una ubicación especificada.
   
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
        // Inicialice Signature con la ruta al documento
        using (Signature signature = new Signature("input.pdf"))
        {
            // Configure ImageSignOptions utilizando una imagen para la firma
            ImageSignOptions options = new ImageSignOptions("company_logo.jpg")
            {
                // Posicione la imagen en la esquina superior izquierda de todas las páginas
                AllPages = true,
                Left = 100,
                Top = 200
            };

            // Guarde el documento firmado
            SignResult result = signature.Sign("output.pdf", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Soluciones integrales para la firma de documentos"
  description: "Nos complace presentar una amplia gama de funcionalidades de firma soportadas por nuestra API. Agregue, modifique, elimine, busque y verifique varios tipos de firmas, incluyendo las basadas en imágenes, sin esfuerzo."
  image: "/img/signature/features_image.webp" # 500x500 px
  image_description: "Firma de Imágenes"
  features:
    # feature loop
    - title: "Incrustar imágenes en documentos de oficina"
      content: "Inserte sin inconvenientes firmas electrónicas e imágenes en cualquier posición designada en cualquier página de un documento. Mejore el contenido de su documento con texto, imágenes, códigos de barras, metadatos o certificados digitales para aumentar la funcionalidad y seguridad."

    # feature loop
    - title: "Búsqueda y verificación de firmas"
      content: "Gestione documentos firmados verificando la autenticidad e integridad de las firmas. Recupere una lista completa de todas las firmas dentro de un documento y examine sus atributos específicos."

    # feature loop
    - title: "Modificar firmas"
      content: "Ocasionalmente, las firmas dentro de los documentos pueden requerir actualizaciones. Ajuste sin dificultad el contenido, la apariencia, el tamaño o la posición de las firmas existentes para satisfacer los requisitos cambiantes."

    # feature loop
    - title: "Eliminar firmas redundantes"
      content: "Nuestra API facilita operaciones CRUD completas para la mayoría de los tipos de firma. Puede eliminar eficientemente firmas de casi todos los formatos de documento compatibles cuando sea necesario."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Asegure el contenido del documento con firmas de imagen"
      content: |
        Descubra cómo enriquecer los documentos empresariales incrustando imágenes, proporcionando información suplementaria.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Seleccione el documento a firmar
          using (Signature signature = new Signature("input.pdf"))
          {
              // Cree opciones de imagen con la ruta de la imagen especificada
              ImageSignOptions options = new ImageSignOptions("manager_signature.jpg")
              {
                    // Defina las dimensiones de la firma de imagen
                    Width = 100,
                    Height = 100,

                    // Posicione la imagen en la esquina inferior derecha
                    VerticalAlignment = VerticalAlignment.Bottom,
                    HorizontalAlignment = HorizontalAlignment.Right,

                    // Aplique el relleno necesario desde los bordes de la página
                    Margin = new Padding() { Bottom = 120, Right = 120 },

                    // Opcionalmente, añada un borde personalizado a la imagen
                    Border = new Border()
                    {
                        Visible = true,
                        Color = Color.Red,
                        DashStyle = DashStyle.DashDotDot,
                        Weight = 5
                    },

                    // Gire la firma para una alineación óptima
                    RotationAngle = 45
              };

              // Guarde el documento actualizado en la ubicación deseada
              SignResult result = signature.Sign("output.pdf", options);
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
            link: "/examples/signature/formats/signature_image.pdf"
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
    title: "Comprenda nuestras ofertas de características"
    exclude: "image"
    description: "Explore un conjunto diverso de tipos de firma y operaciones robustas proporcionadas por nuestra plataforma"
    items: 
          
        # operation loop 1
        - name: "Firmas electrónicas"
          operation: "esign"
          link: "/signature/net/esign/pdf/"
          description: "Agrega varios tipos de firmas a formatos de archivo soportados"

        # operation loop 2
        - name: "Agregar texto a documentos"
          operation: "text"
          link: "/signature/net/text/pdf/"
          description: "Mejora el contenido del documento con firmas de texto personalizables"

        # operation loop 3
        - name: "Firmas de imagen"
          operation: "image"
          link: "/signature/net/image/pdf/"
          description: "Coloca cualquier imagen en cualquier posición dentro de un documento"

        # operation loop 4
        - name: "Generar códigos de barras"
          operation: "barcode"
          link: "/signature/net/barcode/pdf/"
          description: "Crear e insertar varios códigos de barras en documentos soportados"

        # operation loop 5
        - name: "Generar códigos QR"
          operation: "qrcode"
          link: "/signature/net/qrcode/pdf/"
          description: "Generar y utilizar códigos QR para la firma de documentos"
          
        # operation loop 6
        - name: "Certificados digitales"
          operation: "digital"
          link: "/signature/net/digital/pdf/"
          description: "Asegura negocios y firma documentos con certificados digitales"

        # operation loop 7
        - name: "Firmas de sello"
          operation: "stamp"
          link: "/signature/net/stamp/pdf/"
          description: "Utiliza el Constructor de Sellos para crear sellos personalizados redondos o cuadrados"
          
        # operation loop 8
        - name: "Buscar firmas"
          operation: "search"
          link: "/signature/net/search/pdf/"
          description: "Ubica cualquier firma previamente añadida dentro de un documento"
          
        # operation loop 9
        - name: "Verificación de firmas"
          operation: "verify"
          link: "/signature/net/verify/pdf/"
          description: "Verifica la autenticidad de las firmas después de que se han aplicado"
          
        # operation loop 10
        - name: "Modificar firmas"
          operation: "modify"
          link: "/signature/net/modify/pdf/"
          description: "Edita fácilmente una variedad de firmas dentro de un documento"
          
        # operation loop 11
        - name: "Eliminar firmas"
          operation: "delete"
          link: "/signature/net/delete/pdf/"
          description: "Remueve una amplia gama de firmas aplicadas previamente"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Integre imágenes en diversos formatos de archivo"
    exclude: "PDF"
    description: "Aproveche la API de .NET para añadir formatos de imagen compatibles a una amplia variedad de documentos. Redimensione, posicione, seleccione páginas específicas y aplique firmas basadas en imágenes a sus documentos sin complicaciones."
    items: 
          
        # format loop 1
        - name: "Firmar PDF con imagen"
          format: "PDF"
          link: "/signature/net/image/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 2
        - name: "Firmar DOCX con imagen"
          format: "DOCX"
          link: "/signature/net/image/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Firmar JPEG con imagen"
          format: "JPEG"
          link: "/signature/net/image/jpeg/"
          description: "Imagen JPEG"
          
        # format loop 4
        - name: "Firmar PPTX con imagen"
          format: "PPTX"
          link: "/signature/net/image/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 5
        - name: "Firmar XLSX con imagen"
          format: "XLSX"
          link: "/signature/net/image/xlsx/"
          description: "Hoja de Cálculo XML Abierto de Microsoft Excel"


          

---