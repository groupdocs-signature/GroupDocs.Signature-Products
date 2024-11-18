



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:08
draft: false
lang: es
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Firmas electrónicas de archivos XLSX con aplicaciones Java"
head_description: "Utiliza la API de Java para procesar archivos XLSX y aplicar diversos tipos de firmas, incluyendo PDF, Word, Excel, Presentaciones e Imágenes."

############################# Header ############################
title: "Firmas electrónicas para XLSX" 
description: "Agrega una amplia gama de firmas electrónicas utilizando GroupDocs.Signature for Java a todos los formatos comerciales populares, incluyendo PDF, Word, Excel, Presentaciones e Imágenes."
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
    title: "Acerca de la API GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "Aprende más"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) ofrece características avanzadas de firma electrónica. Úsala para agregar, buscar, verificar, modificar y eliminar varios tipos de firmas electrónicas en documentos e imágenes sin la necesidad de software externo. Firma PDFs, documentos de Word, hojas de cálculo de Excel, presentaciones de PowerPoint y formatos de imagen populares.

############################# Steps ############################
steps:
    enable: true
    title: "Pasos para firmar XLSX usando Java"
    content: |
      [GroupDocs.Signature](/signature/java/) permite agregar firmas personalizadas a archivos XLSX. Los desarrolladores de Java pueden integrar la funcionalidad de firma en sus aplicaciones utilizando nuestro software.
      
      1. Proporciona el archivo XLSX que se va a firmar a la instancia de Signature.
      2. Utiliza SignOptions para definir los detalles de la firma.
      3. Personaliza diversas propiedades como tamaño, color y contenido.
      4. Guarda el archivo firmado en la ubicación deseada.
   
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
        // Carga el documento en una instancia de Signature
        Signature signature = new Signature("input.xlsx");

        // Crea un objeto de QrCodeSignOptions
        QrCodeSignOptions options = new QrCodeSignOptions("QR code text");

        // Configura todas las opciones deseadas
        options.setLeft(100);
        options.setTop(100);
        options.setForeColor(Color.RED);

        // Guarda el archivo con el código QR agregado en el disco local
        signature.sign("output.xlsx", options);
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Firmas electrónicas de documentos"
  description: "Nuestra API de firma electrónica optimiza los procesos comerciales. Firma, busca, actualiza, elimina y verifica diversas firmas de manera programática."
  image: "/img/signature/features_esign.webp" # 500x500 px
  image_description: "Firmas electrónicas"
  features:
    # feature loop
    - title: "Firma documentos de oficina"
      content: "Coloca firmas electrónicas en cualquier posición de cualquier página de un documento. Mejora el contenido del documento con texto, imágenes, códigos de barras, metadatos o certificados digitales."

    # feature loop
    - title: "Gestión de firmas"
      content: "Después de firmar, los documentos pueden ser procesados aún más. Recupera una lista de todas las firmas presentes, modifícalas o elimínalas según sea necesario."

    # feature loop
    - title: "Control avanzado de contenido"
      content: "Protege documentos empresariales contra cambios no autorizados con certificados digitales corporativos. Agrega o extrae entradas de metadatos ocultos disponibles en todos los tipos de documentos."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cómo agregar una firma de imagen a un documento"
      content: |
        Este ejemplo demuestra cómo colocar una firma de imagen en una página específica de un documento.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Proporciona el documento fuente como un parámetro
          Signature signature = new Signature("input.xlsx");

          // Especifica la ruta de la imagen en las opciones de firma
          ImageSignOptions options = new ImageSignOptions("image.jpg");

          // Establece el tamaño y las páginas objetivo para la firma
          options.setVerticalAlignment(VerticalAlignment.Bottom);
          options.setHorizontalAlignment(HorizontalAlignment.Right);
          options.setHeight(150);
          options.setWidth(200);
          Padding padding = new Padding(50);
          options.setMargin(padding);
          options.setAllPages(true);

          // Aplica la firma al documento
          signature.sign("output.xlsx", options);

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
        top_links:
          #  loop
          - title: "Descargar resultado"
            icon: "download"
            link: "/examples/signature/formats/signature_esign.xlsx"
        links:
          #  loop
          - title: "Más ejemplos"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
          #  loop
          - title: "Documentación"
            link: "https://docs.groupdocs.com/signature/java/"
            

            


############################## Actions ############################

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
    title: "Explora nuestras características clave"
    exclude: "esign"
    description: "Estamos orgullosos de ofrecer una amplia gama de firmas y operaciones compatibles."
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
    title: "Firma formatos de archivo populares con firmas electrónicas"
    exclude: "XLSX"
    description: "La API de firma electrónica para Java permite el procesamiento de todos los formatos de archivo y documento empresariales modernos."
    items: 
          
        # format loop 1
        - name: "Firma electrónica PDF"
          format: "PDF"
          link: "/signature/java/esign/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 2
        - name: "Firma electrónica DOCX"
          format: "DOCX"
          link: "/signature/java/esign/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Firma electrónica JPEG"
          format: "JPEG"
          link: "/signature/java/esign/jpeg/"
          description: "Imagen JPEG"
          
        # format loop 4
        - name: "Firma electrónica PPTX"
          format: "PPTX"
          link: "/signature/java/esign/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 5
        - name: "Firma electrónica XLSX"
          format: "XLSX"
          link: "/signature/java/esign/xlsx/"
          description: "Hoja de Cálculo XML Abierto de Microsoft Excel"


          

---