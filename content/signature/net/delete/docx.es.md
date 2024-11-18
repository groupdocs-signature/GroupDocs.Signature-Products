



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:19
draft: false
lang: es
format: Docx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Eliminar firmas de DOCX usando C#"
head_description: "La eliminación de firmas digitales, de código de barras, de texto, de imágenes y de metadatos de documentos DOCX firmados se puede realizar con GroupDocs.Signature for .NET."

############################# Header ############################
title: "Elimine firmas de DOCX de manera eficiente" 
description: "Además de firmar documentos empresariales, nuestra solución ofrece herramientas integrales para localizar y eliminar una amplia variedad de firmas mediante GroupDocs.Signature for .NET."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Descargar sin costo"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "Descripción general de GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "Aprende más"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) es una herramienta de firma robusta que facilita la adición de diversos tipos de firmas, que van desde texto e imágenes hasta códigos de barras, certificados digitales y sellos. Con soporte para más de 60 formatos de archivo—incluidos PDF, MS Office, imágenes, ZIP y otros formatos comerciales ampliamente utilizados—esta solución asegura flexibilidad en la gestión de documentos. Además, las firmas aplicadas se pueden localizar, autenticar, modificar o eliminar según sea necesario.

############################# Steps ############################
steps:
    enable: true
    title: "Cómo eliminar firmas electrónicas de DOCX usando C#"
    content: |
      [GroupDocs.Signature](/signature/net/) simplifica la tarea para los desarrolladores de .NET de eliminar firmas electrónicas en archivos DOCX implementando algunos pasos sencillos.
      
      1. Proporcione la ruta del archivo DOCX a una instancia de la clase Signature.
      2. Invoque el método Search para recuperar todas las firmas dentro del documento.
      3. Elimine una o más de las firmas recuperadas.
      4. Examine los resultados del procesamiento del documento.
   
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
        // Pase el documento que contiene firmas a la instancia de Signature
        using (Signature signature = new Signature("input.docx"))
        {
            // Recupere las firmas digitales presentes en el documento
            DigitalSearchOptions options = new DigitalSearchOptions();

            List<DigitalSignature> signatures = signature.Search<DigitalSignature>(options);

            // Elimine la primera firma digital identificada
            if(signatures.Count > 0)
            {
                DigitalSignature digitalSignature = signatures[0];
                bool result = signature.Delete(digitalSignature);

                // Elimine la primera firma digital identificada
                if(result)
                {
                    Console.WriteLine($"Digital signature in DOCX was deleted successfully");
                }
            }
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Optimice la gestión de documentos con herramientas avanzadas de firma"
  description: "GroupDocs.Signature for .NET está meticulosamente diseñado para mejorar la firma y el procesamiento de formatos de archivos comerciales, lo que permite la adición, modificación, verificación o eliminación de firmas."
  image: "/img/signature/features_delete.webp" # 500x500 px
  image_description: "Explore las características versátiles de GroupDocs.Signature"
  features:
    # feature loop
    - title: "Firma de documentos"
      content: "Incorpore sin esfuerzo firmas de texto, imagen, código de barras, código QR o sello en cualquier página de documentos compatibles. Además, utilice metadatos ocultos como EXIF en imágenes o proteja la integridad del documento con certificados digitales, previniendo alteraciones no autorizadas."

    # feature loop
    - title: "Búsqueda y verificación de firmas"
      content: "Aproveche nuestras herramientas para asegurar la autenticidad de las firmas dentro de sus documentos. Realice búsquedas exhaustivas para recuperar una lista completa de todas las firmas, asegurando una gestión integral de documentos."

    # feature loop
    - title: "Modificación de firmas"
      content: "Refine fácilmente las firmas previamente añadidas ajustando el texto, repositionando o alterando colores para satisfacer sus necesidades específicas."

    # feature loop
    - title: "Eliminación de firmas"
      content: "Nuestra solución proporciona capacidades completas de CRUD para firmas, permitiéndole eliminar de manera eficiente una variedad de tipos de firmas de sus documentos cuando sea necesario."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Eliminar todas las firmas de código de barras"
      content: |
        Descubra cómo eliminar todas las firmas de código de barras incrustadas en un documento.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Suministre un documento que contenga firmas de código de barras
          using (Signature signature = new Signature("input.docx"))
          {
              // Elimine todas las firmas de código de barras
              DeleteResult result = signature.Delete(SignatureType.Barcode);

              // Evalúe el resultado del proceso de eliminación
              if (result.Succeeded.Count > 0)
              {
                  Console.WriteLine("Following DOCX barcode signatures were deleted:");                        
                  int number = 1;
                  foreach (BarcodeSignature temp in result.Succeeded)
                  {
                      Console.WriteLine($"Signature #{number++}: Type: {temp.SignatureType} 
                            Id:{temp.SignatureId}, Text: {temp.Text}");
                  }
              }
          }
          ```
        platform: "net"
        copy_title: "Copiar"
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
    title: "Descubra nuestras características destacadas"
    exclude: "delete"
    description: "Nos complace ofrecer una amplia selección de tipos de firma y operaciones admitidas."
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
    title: "Eliminar firmas en múltiples formatos de archivo"
    exclude: "DOCX"
    description: "GroupDocs.Signature for .NET está diseñado para facilitar la eliminación de firmas de una amplia gama de más de 60 formatos de archivo, asegurando una amplia compatibilidad y funcionalidad."
    items: 
          
        # format loop 1
        - name: "Eliminar firmas en PDF"
          format: "PDF"
          link: "/signature/net/delete/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 2
        - name: "Eliminar firmas en DOCX"
          format: "DOCX"
          link: "/signature/net/delete/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Eliminar firmas en PPTX"
          format: "PPTX"
          link: "/signature/net/delete/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 4
        - name: "Eliminar firmas en XLSX"
          format: "XLSX"
          link: "/signature/net/delete/xlsx/"
          description: "Hoja de Cálculo XML Abierto de Microsoft Excel"


          

---