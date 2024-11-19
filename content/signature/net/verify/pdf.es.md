



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:35
draft: false
lang: es
format: Pdf
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Verificación de firmas digitales PDF usando C#"
head_description: "Aproveche el potente GroupDocs.Signature for .NET para autenticar firmas incrustadas en archivos PDF. Valide la legitimidad de las firmas en PDF, Word, Excel, Presentaciones, Imágenes y formatos ZIP."

############################# Header ############################
title: "Verificación de firmas digitales PDF" 
description: "Verifique de manera eficiente todas las firmas electrónicas soportadas en múltiples formatos como PDF, Word, Excel, Presentaciones, Imágenes o archivos ZIP con las completas características de GroupDocs.Signature for .NET."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Descarga de versión gratuita"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "Aplicaciones clave de GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "Aprende más"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) admite capacidades completas de CRUD para la gestión de firmas de documentos. Puede firmar más de 60 formatos diferentes, incluyendo PDFs, archivos de MS Office, Imágenes y archivos ZIP, utilizando varios tipos de firma como texto, imágenes, códigos de barras, certificados digitales, metadatos y sellos. Además de firmar, le permite buscar, validar, actualizar o eliminar firmas.

############################# Steps ############################
steps:
    enable: true
    title: "Guía para verificar firmas en PDF usando C#"
    content: |
      [GroupDocs.Signature](/signature/net/) puede autenticar la presencia de firmas específicas dentro de un documento PDF. Los desarrolladores de .NET pueden mejorar sus aplicaciones incorporando funciones proporcionadas por nuestra solución.
      
      1. Cargar el archivo PDF en la instancia de Signature.
      2. Instanciar y configurar VerifyOptions para lograr el resultado de verificación deseado.
      3. Iniciar el proceso de verificación.
      4. Revisar e interpretar los resultados de la verificación.
   
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
        // Inicializar una instancia de Signature con el documento
        using (Signature signature = new Signature("input.pdf"))
        {
            // Configurar TextVerifyOptions para autenticar firmas que contengan texto específico
            TextVerifyOptions options = new TextVerifyOptions()
            {
                Text = "signature",
                MatchType = TextMatchType.Contains
            };

            // Realizar una verificación de las firmas del documento
            VerificationResult result = signature.Verify(options);

            // Analizar e interpretar los resultados de la verificación
            if(result.IsValid)
            {
                Console.WriteLine($"\nDocument was verified successfully!");
                foreach (TextSignature item in result.Succeeded)
                {
                    Console.WriteLine($"\nValid signature is found with text: {item.Text}");
                }
            }
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Firma de documentos avanzada"
  description: "GroupDocs.Signature es una solución integral diseñada para simplificar la firma y autenticación de documentos en formatos ampliamente utilizados. Ofrece 7 tipos de firmas y operaciones completas de CRUD para asegurar la protección y gestión integral del contenido de sus documentos."
  image: "/img/signature/features_verify.webp" # 500x500 px
  image_description: "Funciones de verificación de firmas"
  features:
    # feature loop
    - title: "Optimizar la firma de documentos corporativos"
      content: "Aplique sin problemas firmas digitales personalizadas en cualquier sección de sus documentos. Con soporte para firmas de texto, imagen, código de barras, metadatos, sellos y certificados digitales, GroupDocs.Signature for .NET garantiza que sus documentos cumplan con los estándares corporativos."

    # feature loop
    - title: "Gestión completa del ciclo de vida de las firmas"
      content: "Gestiona fácilmente todo el ciclo de vida de las firmas dentro de los documentos. Acceda, verifique, actualice o elimine cualquier firma según sea necesario, asegurando que sus documentos permanezcan actualizados y precisos."

    # feature loop
    - title: "Protección de la integridad del contenido del documento"
      content: "Asegure sus documentos sensibles incrustando certificados digitales que eviten alteraciones no autorizadas. Además, añada metadatos ocultos para salvaguardar información crítica y hacer cumplir la integridad del contenido."

    # feature loop
    - title: "Firmas nativas personalizadas"
      content: "Aproveche los tipos de firmas específicas para documentos como sellos PDF y marcas de agua de Word. Estas firmas personalizadas son ideales para branding, marcaje de agua o fines de cumplimiento, brindando un toque profesional refinado a sus documentos corporativos."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Verificar firmas de código de barras"
      content: |
        Este ejemplo ilustra el procedimiento para autenticar firmas de código de barras dentro de un documento.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          using (Signature signature = new Signature("input.pdf"))
          {
              // Configurar las opciones de verificación para coincidir los códigos de barras con criterios de texto específicos
              BarcodeVerifyOptions options = new BarcodeVerifyOptions()
              {
                    Text = "12345",
                    MatchType = TextMatchType.StartsWith
              };

              // Autenticar las firmas incrustadas en el documento
              VerificationResult result = signature.Verify(options);

              // Presentar los resultados del proceso de autenticación
              if (result.IsValid)
              {
                  Console.WriteLine($"\nDocument was verified successfully!");
                  foreach (BarcodeSignature item in result.Succeeded)
                  {
                      Console.WriteLine($"\nValid signature is found with text: {item.Text} 
                            and type: {item.EncodeType.TypeName}.");
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
    title: "Operaciones completas y tipos de firma"
    exclude: "verify"
    description: "Explore la amplia gama de características y operaciones de gestión de firmas disponibles con GroupDocs.Signature, que apoyan el control total sobre los procesos de firma de su documento."
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
    title: "Verificación de firmas entre formatos"
    exclude: "PDF"
    description: "GroupDocs.Signature for .NET le permite verificar de manera eficiente las firmas en una amplia gama de formatos de documentos. Establezca parámetros de verificación personalizados para garantizar la integridad y conformidad del documento."
    items: 
          
        # format loop 1
        - name: "Verificar firmas en PDF"
          format: "PDF"
          link: "/signature/net/verify/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 2
        - name: "Verificar firmas en DOCX"
          format: "DOCX"
          link: "/signature/net/verify/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Verificar firmas en PPTX"
          format: "PPTX"
          link: "/signature/net/verify/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 4
        - name: "Validar firmas en XLSX"
          format: "XLSX"
          link: "/signature/net/verify/xlsx/"
          description: "Hoja de Cálculo XML Abierto de Microsoft Excel"


          

---