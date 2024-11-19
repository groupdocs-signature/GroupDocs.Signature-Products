



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:38
draft: false
lang: es
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Modificar firmas PDF con aplicaciones Java"
head_description: "La API de procesamiento de firmas Java permite modificar firmas en archivos PDF, incluyendo PDF, Word, Excel, Presentaciones e Imágenes."

############################# Header ############################
title: "Modificar firmas PDF" 
description: "Modifique una amplia variedad de firmas electrónicas utilizando GroupDocs.Signature for Java en formatos populares como PDF, Word, Excel, Presentaciones e Imágenes."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Descargar gratis"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "Acerca de GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "Aprende más"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) no solo le permite firmar documentos, sino que también proporciona la capacidad de modificar firmas existentes. Actualice fácilmente firmas en formatos ampliamente utilizados como PDF, Word, Excel y Presentaciones.

############################# Steps ############################
steps:
    enable: true
    title: "Pasos para editar firmas de texto en PDF utilizando Java"
    content: |
      [GroupDocs.Signature](/signature/java/) permite a los desarrolladores de Java actualizar el contenido de firmas de texto previamente añadidas a archivos PDF. Mejore las aplicaciones de Java con capacidades robustas.
      
      1. Agregue el archivo PDF a la instancia de Signature.
      2. Recupere una lista de todas las firmas en el documento.
      3. Actualice el contenido de cualquier firma identificada.
      4. Analice los resultados de la modificación.
   
    code:
      platform: "java"
      copy_title: "Copiar"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Firmas de muestra"
      install:
        command_title: "Maven XML"
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-signature</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "haz clic para copiar"
        copy_done: "copiado"
      links:
        #  loop
        - title: "Más ejemplos"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
        #  loop
        - title: "Documentación"
          link: "https://docs.groupdocs.com/signature/java/"
          
      content: |
        ```java {style=abap}
        // Instanciar un objeto Signature con la ruta del documento
        Signature signature = new Signature("input.pdf");

        // Buscar cualquier firma de texto dentro del documento
        TextSearchOptions options = new TextSearchOptions();
        List<TextSignature> signatures = signature.search(TextSignature.class, options);

        if (signatures.size() > 0) {
            // Alterar el texto de la primera firma detectada
            TextSignature textSignature = signatures.get(0);
            textSignature.setText("New Text");
            boolean result = signature.update('output.pdf', textSignature);

            // Validar el resultado de la modificación
            if (result) {
                System.out.print("\nSignature was updated successfully.");
            }
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Gestión de firmas para documentos"
  description: "GroupDocs.Signature for Java le permite agregar, modificar, buscar, verificar y eliminar firmas en todos los principales formatos de archivo industriales."
  image: "/img/signature/features_modify.webp" # 500x500 px
  image_description: "Modificación de firmas"
  features:
    # feature loop
    - title: "Firmas de documentos"
      content: "Nuestro producto se centra principalmente en firmar documentos con firmas de texto, imagen, código de barras o sello. Puede colocarlas en cualquier página y posición. Agregue o modifique metadatos ocultos, como los datos EXIF en imágenes, y proteja el contenido del documento contra cambios no autorizados utilizando certificados digitales."

    # feature loop
    - title: "Búsqueda y verificación de firmas"
      content: "Asegúrese de que las firmas cumplan con sus requisitos verificando los documentos firmados. Puede obtener una lista completa de firmas dentro de un documento a través de la funcionalidad de búsqueda."

    # feature loop
    - title: "Modificar firmas existentes"
      content: "Modificar firmas añadidas previamente es una tarea común. Utilice el proceso de modificación para actualizar el contenido, la apariencia, la posición y otras propiedades de una firma."

    # feature loop
    - title: "Eliminación de firmas"
      content: "Nuestra solución admite completamente todas las operaciones relacionadas con las firmas. Eliminar varios tipos de firmas de un documento es un proceso sencillo."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Modificar firmas de código de barras"
      content: |
        Este ejemplo ilustra el proceso de modificación de firmas de código de barras dentro de un documento.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Utilice un documento que contenga firmas de código de barras
          final Signature signature = new Signature("input.pdf");

          // Buscar firmas de código de barras existentes
          BarcodeSearchOptions options = new BarcodeSearchOptions();
          List<BarcodeSignature> signatures = signature.search(BarcodeSignature.class, options);

          if (signatures.size() > 0)
          {
              // Ajustar la posición del primer código de barras y guardar el documento actualizado
              BarcodeSignature barcodeSignature = signatures.get(0);
              barcodeSignature.setLeft(100);
              barcodeSignature.setTop(100);
              boolean result = signature.update("output.pdf", barcodeSignature);

              // Confirmar el resultado de la modificación
              if (result)
              {
                    System.out.print("\nBarcode was updated successfully.");
              }
          }
          ```
        platform: "java"
        copy_title: "Copiar"
        install:
          command_title: "Maven XML"
          command: |
            <dependencies>
              <dependency>
                <groupId>com.groupdocs</groupId>
                <artifactId>groupdocs-signature</artifactId>
                <version>{0}</version>
              </dependency>
            </dependencies>
            <repositories>
              <repository>
                <id>repository.groupdocs.com</id>
                <name>GroupDocs Repository</name>
                <url>https://repository.groupdocs.com/repo/</url>
              </repository>
            </repositories>
          copy_tip: "haz clic para copiar"
          copy_done: "copiado"
        links:
          #  loop
          - title: "Más ejemplos"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
          #  loop
          - title: "Documentación"
            link: "https://docs.groupdocs.com/signature/java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "¿Listo para empezar?"
  description: "Prueba las funciones de GroupDocs.Signature de forma gratuita o solicita una licencia"
  items:
    #  loop
    - title: "Descarga de Maven"
      link: "https://releases.groupdocs.com/signature/java/"
      color: "red"
        #  loop
    - title: "Licenciamiento"
      link: "https://purchase.groupdocs.com/pricing/signature/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Investigue nuestro portafolio de funciones"
    exclude: "modify"
    description: "Nos enorgullece admitir una amplia variedad de formatos de firma y herramientas operativas."
    items: 
          
        # operation loop 1
        - name: "Firmas electrónicas"
          operation: "esign"
          link: "/signature/java/esign/pdf/"
          description: "Agrega varios tipos de firmas a formatos de archivo soportados"

        # operation loop 2
        - name: "Agregar texto a documentos"
          operation: "text"
          link: "/signature/java/text/pdf/"
          description: "Mejora el contenido del documento con firmas de texto personalizables"

        # operation loop 3
        - name: "Firmas de imagen"
          operation: "image"
          link: "/signature/java/image/pdf/"
          description: "Coloca cualquier imagen en cualquier posición dentro de un documento"

        # operation loop 4
        - name: "Generar códigos de barras"
          operation: "barcode"
          link: "/signature/java/barcode/pdf/"
          description: "Crear e insertar varios códigos de barras en documentos soportados"

        # operation loop 5
        - name: "Generar códigos QR"
          operation: "qrcode"
          link: "/signature/java/qrcode/pdf/"
          description: "Generar y utilizar códigos QR para la firma de documentos"
          
        # operation loop 6
        - name: "Certificados digitales"
          operation: "digital"
          link: "/signature/java/digital/pdf/"
          description: "Asegura negocios y firma documentos con certificados digitales"

        # operation loop 7
        - name: "Firmas de sello"
          operation: "stamp"
          link: "/signature/java/stamp/pdf/"
          description: "Utiliza el Constructor de Sellos para crear sellos personalizados redondos o cuadrados"
          
        # operation loop 8
        - name: "Buscar firmas"
          operation: "search"
          link: "/signature/java/search/pdf/"
          description: "Ubica cualquier firma previamente añadida dentro de un documento"
          
        # operation loop 9
        - name: "Verificación de firmas"
          operation: "verify"
          link: "/signature/java/verify/pdf/"
          description: "Verifica la autenticidad de las firmas después de que se han aplicado"
          
        # operation loop 10
        - name: "Modificar firmas"
          operation: "modify"
          link: "/signature/java/modify/pdf/"
          description: "Edita fácilmente una variedad de firmas dentro de un documento"
          
        # operation loop 11
        - name: "Eliminar firmas"
          operation: "delete"
          link: "/signature/java/delete/pdf/"
          description: "Remueve una amplia gama de firmas aplicadas previamente"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Modificar firmas en varios formatos de archivo"
    exclude: "PDF"
    description: "Los formatos de documento firmados utilizando nuestra API para Java pueden ser modificados. Recupere una lista de firmas de un documento y actualice cualquier propiedad accesible."
    items: 
          
        # format loop 1
        - name: "Modificar firmas en PDF"
          format: "PDF"
          link: "/signature/java/modify/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 2
        - name: "Editar firmas en DOCX"
          format: "DOCX"
          link: "/signature/java/modify/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Editar firmas en PPTX"
          format: "PPTX"
          link: "/signature/java/modify/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 4
        - name: "Modificar firmas en XLSX"
          format: "XLSX"
          link: "/signature/java/modify/xlsx/"
          description: "Hoja de Cálculo XML Abierto de Microsoft Excel"


          

---