



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:47
draft: false
lang: es
format: Docx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Sellos redondos y cuadrados DOCX a través de C#"
head_description: "Utiliza GroupDocs.Signature for .NET para generar e incrustar sellos personalizados en archivos DOCX."

############################# Header ############################
title: "Generar sellos para archivos DOCX" 
description: "Integra sin esfuerzo sellos diseñados a medida en cualquier sección de tus documentos utilizando GroupDocs.Signature for .NET, ofreciendo una amplia flexibilidad para la colocación y configuración de sellos para satisfacer tus necesidades empresariales."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Obtén tu descarga gratuita"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "Resumen de GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "Aprende más"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) es una herramienta versátil que permite la inserción de múltiples tipos de firmas en documentos, incluidos los sellos personalizables. Soportando más de 60 formatos de archivo, desde PDFs y documentos de Word hasta imágenes y archivos ZIP, puedes enriquecer tus documentos con texto, imagen, código de barras, metadatos, certificados digitales y sellos. Además, tienes control total para buscar, validar, modificar o eliminar cualquier firma aplicada a tus archivos.

############################# Steps ############################
steps:
    enable: true
    title: "Cómo incrustar un sello en DOCX usando C#"
    content: |
      [GroupDocs.Signature](/signature/net/) ofrece una robusta funcionalidad de creación de sellos, ideal para mejorar las aplicaciones .NET. Aprovecha esta herramienta para diseñar e implementar sellos altamente personalizados en las páginas de tus documentos.
      
      1. Proporciona el documento DOCX que debe ser sellado.
      2. Utiliza StampSignOptions para configurar meticulosamente todos los parámetros necesarios.
      3. Añade múltiples líneas de sello según tus requerimientos.
      4. Aplica el sello configurado y guarda el documento modificado.
   
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
        // Integra la ruta del documento con la instancia de Signature
        using (Signature signature = new Signature("input.docx"))
        {
            // Inicializa StampSignOptions con el contenido de firma requerido
            StampSignOptions options = new StampSignOptions();
            options.Height = 180;
            options.Width = 180;

            // Incorpora una o múltiples líneas de sello
            options.OuterLines.Add(
                new StampLine()
                {
                    Text = "* The Best Company *",
                    TextRepeatType = StampTextRepeatType.FullTextRepeat,
                    Font = new SignatureFont() { Size = 12, FamilyName = "Arial" },
                    Height = 22,
                    TextBottomIntent = 6,
                    TextColor = Color.WhiteSmoke,
                    BackgroundColor = Color.DarkSlateBlue
                }
            );

            // Preserva el documento con el sello aplicado
            SignResult result = signature.Sign("output.docx", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Aprovecha las firmas para asegurar y mejorar la integridad del documento"
  description: "Con la biblioteca GroupDocs.Signature for .NET, puedes integrar sin problemas la funcionalidad de firma en tus documentos. Añade, modifica, verifica o elimina sellos personalizados y otros tipos de firma, ofreciendo flexibilidad y precisión para la gestión segura de documentos."
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "Firmas de sellos impulsadas por GroupDocs.Signature"
  features:
    # feature loop
    - title: "Firma de documentos integral"
      content: "Mejora tus documentos colocando firmas, incluidos texto, imágenes, códigos de barras, códigos QR y sellos, en cualquier posición o página dentro del archivo. Además, gestiona metadatos incrustados y aplica certificados digitales para salvaguardar contra cambios no autorizados."

    # feature loop
    - title: "Búsqueda y validación de firmas eficiente"
      content: "Después de firmar, verifica la autenticidad y la integridad de las firmas del documento. Utiliza la funcionalidad de búsqueda avanzada para recuperar y gestionar todos los datos de firma incrustados en el documento."

    # feature loop
    - title: "Modificar y personalizar firmas"
      content: "Ajusta las firmas insertadas anteriormente según sea necesario. Ya sea que necesites cambiar el contenido, la posición, el tamaño o el color, nuestra solución ofrece total flexibilidad para la modificación de firmas."

    # feature loop
    - title: "Elimina firmas sin esfuerzo"
      content: "Cuando sea necesario eliminar firmas, GroupDocs.Signature for .NET proporciona un conjunto completo de herramientas para borrar cualquier tipo de firma, incluidos sellos, certificados digitales y más, asegurando que tus documentos se mantengan actualizados y cumplan con la normativa."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Implementar sellos personalizados en documentos"
      content: |
        Descubre cómo crear e integrar sellos personalizados que contengan detalles textuales críticos en tus documentos.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Suministra el documento que será sellado
          using (Signature signature = new Signature("input.docx"))
          {
              // Inicializa las opciones de sello con las configuraciones deseadas
              StampSignOptions options = new StampSignOptions()
              {
                    // Define las dimensiones y la posición del sello en la página
                    Height = 200,
                    Width = 200,
                    VerticalAlignment = VerticalAlignment.Bottom,
                    HorizontalAlignment = HorizontalAlignment.Right,
                    AllPages = true
              };

              // Incorpora líneas circulares exteriores con texto
              options.OuterLines.Add(
                    new StampLine()
                    {
                        Text = "* The best  choice *",
                        TextRepeatType = StampTextRepeatType.FullTextRepeat,
                        Font = new SignatureFont() { Size = 12, FamilyName = "Arial" },
                        Height = 22,
                        TextBottomIntent = 6,
                        TextColor = Color.WhiteSmoke,
                        BackgroundColor = Color.DarkSlateBlue
                    }
              );

              // Integra líneas cuadradas interiores si es necesario
              options.InnerLines.Add(
                    new StampLine()
                    { 
                        Text = "Company #1",
                        TextColor = Color.MediumVioletRed,
                        Font = new SignatureFont() { Size = 20, Bold = true },
                        Height = 40
                    }
              );

              // Finaliza y guarda el documento sellado
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
            link: "/examples/signature/formats/signature_stamp.docx"
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
    title: "Explora las funcionalidades clave"
    exclude: "stamp"
    description: "Descubre una amplia gama de opciones para crear, gestionar y eliminar varios tipos de firmas, asegurando un control completo sobre tus flujos de trabajo de documentos."
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
    title: "Aplica sellos en varios formatos de documento"
    exclude: "DOCX"
    description: "La API GroupDocs.Signature te permite incrustar sellos en más de 60 tipos de archivos estándar de la industria. Aplica sellos personalizados en cualquier ubicación dentro de tus documentos, lo que permite un mejor seguimiento y personalización de los documentos."
    items: 
          
        # format loop 1
        - name: "Sellar PDF"
          format: "PDF"
          link: "/signature/net/stamp/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 2
        - name: "Sellar DOCX"
          format: "DOCX"
          link: "/signature/net/stamp/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Sellar JPEG"
          format: "JPEG"
          link: "/signature/net/stamp/jpeg/"
          description: "Imagen JPEG"
          
        # format loop 4
        - name: "Sellar PPTX"
          format: "PPTX"
          link: "/signature/net/stamp/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 5
        - name: "Sellar XLSX"
          format: "XLSX"
          link: "/signature/net/stamp/xlsx/"
          description: "Hoja de Cálculo XML Abierto de Microsoft Excel"


          

---