



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:19
draft: false
lang: es
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Eliminar firmas de XLSX usando Java"
head_description: "La eliminación de firmas digitales, de código de barras, de texto, de imágenes y de metadatos de documentos XLSX firmados se puede realizar utilizando GroupDocs.Signature for Java."

############################# Header ############################
title: "Eliminar firmas de XLSX" 
description: "Nuestra solución no solo te permite firmar documentos comerciales, sino que también ofrece la capacidad de localizar y eliminar varios tipos de firmas utilizando GroupDocs.Signature for Java."
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
       [GroupDocs.Signature for Java](/signature/java/) ofrece una solución integral de firmas, capaz de manejar varios tipos de firmas como texto, imágenes, códigos de barras, certificados digitales y sellos. Esta herramienta admite más de 60 formatos de archivo diferentes, incluidos PDF, documentos de MS Office, archivos de imagen, archivos ZIP y muchos otros formatos de uso común. Además, una vez que se aplican las firmas, se pueden buscar, verificar, editar o eliminar fácilmente cuando sea necesario.

############################# Steps ############################
steps:
    enable: true
    title: "Pasos para eliminar firmas electrónicas de XLSX usando Java"
    content: |
      [GroupDocs.Signature](/signature/java/) facilita a los desarrolladores de Java eliminar firmas electrónicas en archivos XLSX usando sus aplicaciones siguiendo unos pocos pasos simples.
      
      1. Pasa la ruta de XLSX a una instancia de la clase Signature.
      2. Utiliza el método Search para recuperar firmas del documento.
      3. Elimina una o más de las firmas ubicadas.
      4. Analiza los resultados del procesamiento del documento.
   
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
        // Pasa el documento que contiene las firmas que deben ser eliminadas a Signature
        Signature signature = new Signature("input.xlsx");

        // Recupera las firmas digitales presentes en el documento
        DigitalSearchOptions options = new DigitalSearchOptions();
        List<DigitalSignature> signatures = signature.search(DigitalSignature.class, options);

        // Elimina la primera firma digital ubicada
        if(signatures.size() > 0)
        {
            DigitalSignature digitalSignature = signatures.get(0);
            boolean result = signature.delete("output.xlsx", digitalSignature);

            // Procesa el resultado de la eliminación
            if(result)
            {
                System.out.print("\nDigital XLSX signature was deleted successfully");
            }
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Mejora los procesos comerciales con la gestión de firmas"
  description: "GroupDocs.Signature for Java está diseñado para firmar y gestionar formatos de archivo comerciales, permitiéndote agregar, modificar, verificar o eliminar firmas según sea necesario."
  image: "/img/signature/features_delete.webp" # 500x500 px
  image_description: "Capacidades de GroupDocs.Signature"
  features:
    # feature loop
    - title: "Firmar documentos"
      content: "Agrega firmas de texto, imagen, código de barras, código QR o sello a cualquier página de documentos compatibles. Utiliza metadatos ocultos como EXIF en imágenes o protege el contenido del documento contra modificaciones no autorizadas con certificados digitales."

    # feature loop
    - title: "Búsqueda y verificación"
      content: "Maximiza el potencial de los documentos firmados verificando las firmas para asegurar su validez. También puedes recuperar una lista completa de todas las firmas presentes en un documento a través de una búsqueda simple."

    # feature loop
    - title: "Modificar firmas"
      content: "La mayoría de las firmas agregadas previamente pueden ser ajustadas. Puedes modificar fácilmente el texto, reposicionar la firma o cambiar su color."

    # feature loop
    - title: "Eliminar firmas"
      content: "Nuestra solución admite completamente las operaciones CRUD para firmas, lo que te permite eliminar varios tipos de firmas de un documento según sea necesario."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Eliminar todas las firmas de código de barras"
      content: |
        Aprende cómo eliminar todas las firmas de código de barras incrustadas en un documento.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Proporciona un documento que contiene firmas de código de barras
          Signature signature = new Signature("input.xlsx");

          // Elimina todas las firmas de código de barras
          DeleteResult result = signature.delete("output.xlsx", SignatureType.Barcode);

          // Procesa el resultado de la eliminación
          if (result.getSucceeded().size() > 0)
          {
              System.out.print("\nFollowing XLSX barcode signatures were deleted:");
              int number = 1;
              for (BaseSignature temp : result.getSucceeded())
              {
                    System.out.print("Signature #"+number++ +
                    ": Type: "+temp.getSignatureType()+" Id:"+temp.getSignatureId()+
                    ", Text: "+((BarcodeSignature)temp).getText());
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
    title: "Conoce nuestras características clave"
    exclude: "delete"
    description: "Explora las diversas operaciones y métodos de firma disponibles con nuestra plataforma"
    items: 
          
        # operation loop 1
        - name: "Firmas electrónicas"
          operation: "esign"
          link: "/signature/java/esign/xlsx/"
          description: "Agrega varios tipos de firmas a formatos de archivo soportados"

        # operation loop 2
        - name: "Agregar texto a documentos"
          operation: "text"
          link: "/signature/java/text/xlsx/"
          description: "Mejora el contenido del documento con firmas de texto personalizables"

        # operation loop 3
        - name: "Firmas de imagen"
          operation: "image"
          link: "/signature/java/image/xlsx/"
          description: "Coloca cualquier imagen en cualquier posición dentro de un documento"

        # operation loop 4
        - name: "Generar códigos de barras"
          operation: "barcode"
          link: "/signature/java/barcode/xlsx/"
          description: "Crear e insertar varios códigos de barras en documentos soportados"

        # operation loop 5
        - name: "Generar códigos QR"
          operation: "qrcode"
          link: "/signature/java/qrcode/xlsx/"
          description: "Generar y utilizar códigos QR para la firma de documentos"
          
        # operation loop 6
        - name: "Certificados digitales"
          operation: "digital"
          link: "/signature/java/digital/xlsx/"
          description: "Asegura negocios y firma documentos con certificados digitales"

        # operation loop 7
        - name: "Firmas de sello"
          operation: "stamp"
          link: "/signature/java/stamp/xlsx/"
          description: "Utiliza el Constructor de Sellos para crear sellos personalizados redondos o cuadrados"
          
        # operation loop 8
        - name: "Buscar firmas"
          operation: "search"
          link: "/signature/java/search/xlsx/"
          description: "Ubica cualquier firma previamente añadida dentro de un documento"
          
        # operation loop 9
        - name: "Verificación de firmas"
          operation: "verify"
          link: "/signature/java/verify/xlsx/"
          description: "Verifica la autenticidad de las firmas después de que se han aplicado"
          
        # operation loop 10
        - name: "Modificar firmas"
          operation: "modify"
          link: "/signature/java/modify/xlsx/"
          description: "Edita fácilmente una variedad de firmas dentro de un documento"
          
        # operation loop 11
        - name: "Eliminar firmas"
          operation: "delete"
          link: "/signature/java/delete/xlsx/"
          description: "Remueve una amplia gama de firmas aplicadas previamente"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Eliminar firmas de varios formatos de archivo"
    exclude: "XLSX"
    description: "Nuestra solución GroupDocs.Signature for Java admite la eliminación de firmas de más de 60 formatos de archivo diferentes."
    items: 
          
        # format loop 1
        - name: "Eliminar firmas en PDF"
          format: "PDF"
          link: "/signature/java/delete/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 2
        - name: "Eliminar firmas en DOCX"
          format: "DOCX"
          link: "/signature/java/delete/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Eliminar firmas en PPTX"
          format: "PPTX"
          link: "/signature/java/delete/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 4
        - name: "Eliminar firmas en XLSX"
          format: "XLSX"
          link: "/signature/java/delete/xlsx/"
          description: "Hoja de Cálculo XML Abierto de Microsoft Excel"


          

---