



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:20
draft: false
lang: es
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Cree un código QR para XLSX con Java"
head_description: "La API GroupDocs.Signature permite generar códigos QR para archivos XLSX. Cree códigos QR a partir de su contenido y colóquelos en cualquier página."

############################# Header ############################
title: "Cree códigos QR para XLSX" 
description: "Genere códigos de barras 2D con datos de texto y numéricos y colóquelos en cualquier página de diversos documentos usando GroupDocs.Signature for Java."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Prueba gratuita"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "Aprenda más sobre GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "Aprende más"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) ofrece una amplia gama de características para generar e incrustar varios tipos de firmas en todos los formatos de documento principales. Soporta PDFs, documentos de Word, hojas de cálculo de Excel, presentaciones de PowerPoint e imágenes. Mejore sus documentos con firmas de Texto, Imagen, Código de Barras, Código QR, Metadatos, Digitales y Sello.

############################# Steps ############################
steps:
    enable: true
    title: "Pasos para generar y colocar un código QR en cualquier ubicación de un XLSX"
    content: |
      [GroupDocs.Signature](/signature/java/) puede generar códigos QR en muchos formatos populares y colocarlos en páginas de XLSX. Se soportan más de 10 tipos de códigos QR que pueden integrarse rápidamente en aplicaciones Java. Use nuestro producto para firmar documentos con códigos QR generados.
      
      1. Obtenga el archivo o flujo XLSX que se firmará con un código QR.
      2. Proporcione el texto para QrCodeSignOptions.
      3. Personalice opciones visuales como color, posición, tamaño, etc.
      4. Guarde el archivo con el código QR.
   
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
        // Pase el documento a una nueva instancia de Signature
        Signature signature = new Signature("input.xlsx");

        // Use QrCodeSignOptions para agregar un código QR al documento
        QrCodeSignOptions options = new QrCodeSignOptions("Text Content");

        // Especifique el tipo de firma y la posición en la página
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(50);
        options.setTop(150);

        // Guarde el archivo con el código QR agregado
        signature.sign("output.xlsx", options);

        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Agregue firmas a sus documentos"
  description: "La API GroupDocs.Signature for Java soporta la firma de todos los formatos de archivo populares. Genere, modifique, busque, verifique y elimine diferentes tipos de firmas."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "Características clave de GroupDocs.Signature"
  features:
    # feature loop
    - title: "Firmar documentos"
      content: "GroupDocs.Signature admite la firma con firmas de Texto, Imagen, Código de Barras, Código QR y Sello. Colóquelas en cualquier página de cualquier formato de documento soportado. Administre los metadatos del documento con firmas de metadatos y proteja el contenido de cambios no autorizados usando certificados digitales."

    # feature loop
    - title: "Búsqueda y verificación"
      content: "Asegúrese de que todas las firmas en un documento sean válidas mediante el procedimiento de verificación. Recupere una lista completa de firmas en un documento utilizando la función de búsqueda integrada."

    # feature loop
    - title: "Modificar firmas"
      content: "Modifique fácilmente las propiedades de la firma después de firmar. Ajuste el contenido, la posición, el color, el tamaño y otros atributos según sea necesario."

    # feature loop
    - title: "Eliminar firmas"
      content: "Elimine firmas no deseadas sin complicaciones. Diversos tipos de firmas, incluidos los certificados digitales, pueden ser eliminados programáticamente de los documentos."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cómo personalizar un código QR generado"
      content: |
        Utilice este ejemplo para aprender a colocar un nuevo código QR en una página de XLSX.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Obtenga el documento que necesita ser firmado y páselo a Signature
          Signature signature = new Signature("input.xlsx");

          // Utilice las opciones de código QR para proporcionar texto con la información requerida
          QrCodeSignOptions signOptions = new QrCodeSignOptions("Archived on July 11, 2019");

          // Establezca la posición relativa del código QR en la página
          signOptions.setVerticalAlignment(VerticalAlignment.Top);
          signOptions.setHorizontalAlignment(HorizontalAlignment.Right);

          // Establezca el relleno de la firma
          Padding padding = new Padding();
          padding.setRight(20);
          padding.setTop(20);
          signOptions.setMargin(padding);

          // Especifique el color del código QR
          signOptions.setForeColor(Color.RED);

          // Defina las opciones de fuente para el mensaje
          SignatureFont font = new SignatureFont();
          font.setSize(12);
          font.setFamilyName("Comic Sans MS");
          signOptions.setFont(font);

          // Personalice el color de fondo del código QR y el pincel
          Background background = new Background();
          background.setColor(Color.GREEN);
          background.setTransparency(0.5);
          background.setBrush(new LinearGradientBrush(Color.GREEN, Color.DARK_GRAY, 0));
          signOptions.setBackground(background);

          // Agregue el código QR al documento
          SignResult signResult = signature.sign("output.xlsx", signOptions);
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
            link: "/examples/signature/formats/signature_qrcode.xlsx"
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
    title: "Descubra nuestras ofertas clave"
    exclude: "qrcode"
    description: "Ofrecemos una selección diversa de características de firmas y operaciones avanzadas."
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
    title: "Genere códigos QR para formatos de archivo adicionales"
    exclude: "XLSX"
    description: "Mejore todos los formatos de archivo populares con códigos QR generados usando la API Java. Agregue datos de códigos de barras 2D para un escaneo y procesamiento fáciles."
    items: 
          
        # format loop 1
        - name: "Código QR para PDF"
          format: "PDF"
          link: "/signature/java/qrcode/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 2
        - name: "Código QR para DOCX"
          format: "DOCX"
          link: "/signature/java/qrcode/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Código QR para JPEG"
          format: "JPEG"
          link: "/signature/java/qrcode/jpeg/"
          description: "Imagen JPEG"
          
        # format loop 4
        - name: "Código QR para PPTX"
          format: "PPTX"
          link: "/signature/java/qrcode/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 5
        - name: "Código QR para XLSX"
          format: "XLSX"
          link: "/signature/java/qrcode/xlsx/"
          description: "Hoja de Cálculo XML Abierto de Microsoft Excel"


          

---