



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:31
draft: false
lang: es
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Buscar firma digital en XLSX por Java"
head_description: "Aprovecha la API de GroupDocs.Signature for Java para buscar firmas dentro de archivos XLSX. Encuentra firmas en PDFs, Word, Excel, Presentaciones e Imágenes."

############################# Header ############################
title: "Buscar firmas digitales en XLSX" 
description: "Recupera una lista completa de firmas electrónicas incrustadas en archivos PDF, Word, Excel, Presentaciones o Imágenes utilizando GroupDocs.Signature for Java."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Descarga gratuita"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "Acerca de GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "Aprende más"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) ofrece potentes características para firmar documentos. Soporta la adición de texto, imágenes, códigos de barras, certificados digitales y sellos a archivos en más de 60 formatos, incluidos PDFs, documentos de MS Office, Imágenes, archivos ZIP y otros formatos comerciales habituales. Además, puedes buscar, verificar, modificar o eliminar firmas en cualquier momento.

############################# Steps ############################
steps:
    enable: true
    title: "Pasos para buscar firmas en XLSX usando Java"
    content: |
      [GroupDocs.Signature](/signature/java/) proporciona un potente motor para buscar cualquier firma digital dentro de archivos XLSX. Los desarrolladores de Java pueden mejorar sus aplicaciones con nuestra solución.
      
      1. Proporciona la ruta del archivo XLSX para buscar firmas.
      2. Usa SearchOptions para refinar los resultados de búsqueda.
      3. Ejecuta el método Search para obtener los resultados.
      4. Analiza la lista de firmas encontradas.
   
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

        // Crea una instancia de Signature con la ruta del documento
        final Signature signature = new Signature("input.xlsx");

        // Instancia TextSearchOptions para abarcar todas las páginas
        TextSearchOptions options = new TextSearchOptions();
        options.setAllPages(true);

        // Busca firmas de texto dentro del documento
        List<TextSignature> signatures = signature.search(TextSignature.class, options);
        System.out.print("\nSource document contains following text signature(s).");

        // Lista las firmas encontradas para un análisis posterior
        for (TextSignature textSignature : signatures) {
            System.out.print("Found Text signature at page " + textSignature.getPageNumber() 
                + " with type [" + textSignature.getSignatureImplementation() + "] and 
                text '" + textSignature.getText() + "'.");
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Solución integral para la firma de documentos"
  description: "Nos complace presentar nuestra solución de firma de documentos, compatible con todos los formatos de documentos principales. Agrega una amplia gama de firmas para mejorar tus documentos o asegurar su contenido."
  image: "/img/signature/features_search.webp" # 500x500 px
  image_description: "Búsqueda de firmas"
  features:
    # feature loop
    - title: "Firmar documentos comerciales"
      content: "Inserta firmas digitales en cualquier posición de cualquier página de un documento. Utiliza una variedad de tipos de firma, como texto, imágenes, códigos de barras, metadatos, sellos o certificados digitales."

    # feature loop
    - title: "Gestionar firmas"
      content: "Después de firmar, los documentos pueden requerir procesamiento adicional. Busca todas las firmas disponibles y actualízalas o elimínalas cuando sea necesario."

    # feature loop
    - title: "Proteger el contenido del documento"
      content: "Gestiona los metadatos ocultos incrustados en el documento. Agrega nuevos metadatos o elimina entradas existentes. Utiliza certificados digitales corporativos para proteger el contenido del documento de alteraciones no autorizadas."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Buscar firmas de imagen"
      content: |
        Este ejemplo demuestra cómo encontrar una firma de imagen en un documento específico.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Pasa el documento fuente como un parámetro del constructor
          final Signature signature = new Signature("input.xlsx");

          // Busca cualquier firma con un tipo de texto
          List<ImageSignature> signatures = signature.search(ImageSignature.class, SignatureType.Image);
          System.out.print("\nSource document contains following image signature(s).");

          // Muestra los resultados con las propiedades de las firmas encontradas
          for (ImageSignature imageSignature : signatures)
          {
              System.out.print("Image signature found at page "+imageSignature.getPageNumber()+
                    " with size "+imageSignature.getSize()+". Created "+imageSignature.getCreatedOn()+
                    ", modified "+imageSignature.getModifiedOn());
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
    title: "Operaciones soportadas"
    exclude: "search"
    description: "Nuestro producto ofrece una API flexible para firmar documentos y gestionar firmas después de la firma."
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
    title: "Buscar firmas en varios formatos de archivo"
    exclude: "XLSX"
    description: "La API GroupDocs.Signature for Java te permite recuperar la lista de firmas de cualquier archivo firmado. Extrae firmas de formatos de archivo populares para procesamiento adicional."
    items: 
          
        # format loop 1
        - name: "Buscar firmas en PDF"
          format: "PDF"
          link: "/signature/java/search/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 2
        - name: "Encontrar firmas en DOCX"
          format: "DOCX"
          link: "/signature/java/search/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Encontrar firmas en PPTX"
          format: "PPTX"
          link: "/signature/java/search/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 4
        - name: "Buscar firmas en XLSX"
          format: "XLSX"
          link: "/signature/java/search/xlsx/"
          description: "Hoja de Cálculo XML Abierto de Microsoft Excel"


          

---