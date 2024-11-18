



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:57
draft: false
lang: es
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Añadiendo firmas electrónicas digitales a archivos XLSX con Java"
head_description: "Coloca una firma digital en un archivo XLSX utilizando Java con solo unas pocas líneas de código. Usa GroupDocs.Signature for Java para firmar numerosos formatos de archivo."

############################# Header ############################
title: "Firmar XLSX con firmas digitales" 
description: "Protege el contenido de tus documentos comerciales sellándolos con certificados digitales utilizando las funciones de GroupDocs.Signature for Java. Ofrecemos múltiples formas de marcar y asegurar tus documentos."
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
       [GroupDocs.Signature for Java](/signature/java/) es una solución integral de firma que admite varios tipos de procesamiento de documentos. Puedes agregar texto, imágenes, certificados digitales y sellos a archivos en más de 60 formatos, incluyendo PDF, MS Office, imágenes, archivos ZIP y otros formatos comerciales populares. Además, los documentos firmados pueden ser buscados, verificados, modificados o eliminados automáticamente de manera conveniente.

############################# Steps ############################
steps:
    enable: true
    title: "Pasos para proteger XLSX con certificados digitales en Java"
    content: |
      [GroupDocs.Signature](/signature/java/) permite a los desarrolladores de Java prevenir cambios en documentos XLSX mediante firmas digitales. Potencia tus aplicaciones comerciales con la capacidad de asegurar datos importantes.
      
      1. Pasa el documento XLSX al constructor de la clase Signature.
      2. Usa un certificado digital y su contraseña para proteger el documento.
      3. Opcionalmente, agrega una representación visual de la firma digital en las páginas del documento.
      4. Firma el documento para prevenir futuros cambios.
   
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
        // Utiliza Signature con el documento para la firma digital
        Signature signature = new Signature("input.xlsx");

        // Proporciona un certificado digital y una contraseña
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");
        options.setPassword("1234567890");

        // Configura una representación visual si es necesario
        options.setPageNumber(1);
        options.setLeft(100);
        options.setTop(100);

        // Protege el documento con un certificado digital
        SignResult result = signature.sign("output.xlsx", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Mejora o protege el contenido del documento con firmas"
  description: "La biblioteca GroupDocs.Signature for Java es capaz de firmar todos los formatos de archivo populares. Agrega, modifica, verifica o elimina varios tipos de firmas automáticamente para optimizar tus procesos comerciales."
  image: "/img/signature/features_digital.webp" # 500x500 px
  image_description: "Características de GroupDocs.Signature"
  features:
    # feature loop
    - title: "Agregar firmas a documentos"
      content: "Las firmas de texto, imagen, código de barras, QR-Code o sello pueden ser añadidas con precisión a cualquier página de cualquier documento compatible. Metadatos ocultos como EXIF pueden ser añadidos o editados en imágenes y la mayoría de los tipos de archivo. Protege el contenido del documento de cambios no autorizados utilizando firmas digitales."

    # feature loop
    - title: "Búsqueda y verificación de firmas"
      content: "Los documentos pueden ser procesados de varias formas después de firmarlos. Verifica los documentos firmados para asegurarte de que han sido procesados correctamente. Si necesitas más control, recupera una lista de todas las firmas mediante búsqueda."

    # feature loop
    - title: "Editar firmas"
      content: "La mayoría de los tipos de firmas soportan modificaciones adicionales. Puedes corregir texto, cambiar posición, color, tamaño y más."

    # feature loop
    - title: "Eliminar firmas innecesarias"
      content: "Nuestra solución soporta operaciones completas de CRUD para firmas. Muchos tipos de firmas, incluidos los certificados digitales, pueden ser eliminados de un documento cuando sea necesario."
      
  code_samples:
    # code sample loop
    - title: "Proteger documentos con firmas digitales"
      content: |
        Aprende cómo asegurar un documento de cambios utilizando firmas digitales.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        // Proporciona un documento para firmar
        Signature signature = new Signature("input.xlsx");

        // Usa un certificado digital válido con contraseña
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");
        options.setPassword("1234567890");

        // Especifica datos de texto adicionales
        options.setReason("Security issue");
        options.setContact("John Smith");
        options.setLocation("Office D.W.");

        // Utiliza una imagen y otras opciones para la representación visual
        options.setImageFilePath("image.png");

        options.setAllPages(true);
        options.setVerticalAlignment(VerticalAlignment.Bottom);
        options.setHorizontalAlignment(HorizontalAlignment.Right);
        options.setWidth(80);
        options.setHeight(60);

        Padding padding = new Padding();
        padding.setBottom(10);
        padding.setRight(10);
        options.setMargin(padding);

        // Guarda el documento protegido en una ubicación diferente
        SignResult result = signature.sign("output.xlsx", options);
        ```
        {{< /landing/code >}}


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
    title: "Examina nuestro completo conjunto de características"
    exclude: "digital"
    description: "Nos enorgullece la extensa funcionalidad y soporte de firmas que nuestra plataforma ofrece."
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
    title: "Firmar documentos en otros formatos"
    exclude: "XLSX"
    description: "La API Java permite procesar más de 60 formatos. Crea y añade varias firmas a cualquier página, sella el contenido con certificados digitales y gestiona y edita firmas existentes dentro del documento."
    items: 
          
        # format loop 1
        - name: "Proteger PDF"
          format: "PDF"
          link: "/signature/java/digital/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 2
        - name: "Proteger DOCX"
          format: "DOCX"
          link: "/signature/java/digital/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Proteger PPTX"
          format: "PPTX"
          link: "/signature/java/digital/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 4
        - name: "Proteger XLSX"
          format: "XLSX"
          link: "/signature/java/digital/xlsx/"
          description: "Hoja de Cálculo XML Abierto de Microsoft Excel"


          

---