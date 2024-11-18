



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:46
draft: false
lang: es
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Añadir sellos a DOCX usando Java"
head_description: "Aproveche GroupDocs.Signature y Java para crear sellos personalizados y colocarlos en cualquier página dentro de los documentos DOCX."

############################# Header ############################
title: "Añadir sellos personalizados a DOCX" 
description: "Diseñe y aplique sellos redondos o cuadrados a cualquier sección de sus documentos utilizando GroupDocs.Signature for Java. Nuestra solución ofrece amplias opciones de personalización para atender todas sus necesidades comerciales."
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
       [GroupDocs.Signature for Java](/signature/java/) es una herramienta robusta que le permite añadir diversas firmas de sello a los documentos. Soporta más de 60 formatos de archivo diferentes, incluidos PDFs, Word, Excel, imágenes y archivos ZIP. Puede aplicar firmas de texto, imagen, código de barras, metadatos, certificado digital y firmas de sello. Además de añadir firmas, puede buscarlas, verificar, modificar y eliminarlas.

############################# Steps ############################
steps:
    enable: true
    title: "Pasos para añadir sellos a DOCX a través de Java"
    content: |
      [GroupDocs.Signature](/signature/java/) proporciona un constructor de sellos que puede ser muy beneficioso para aplicaciones Java. Úselo para crear sellos bien personalizados para las páginas de su documento.
      
      1. Proporcione el documento DOCX que debe ser sellado.
      2. Utilice StampSignOptions para configurar todos los parámetros necesarios.
      3. Agregue tantas líneas como sea necesario.
      4. Aplique el sello y guarde el documento.
   
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
        // Utilice la ruta del documento con el objeto Signature
        Signature signature = new Signature("input.docx");

        // Instancie StampSignOptions con el texto de firma deseado
        StampSignOptions options = new StampSignOptions();
        options.Height = 180;
        options.Width = 180;

        // Agregue una o más líneas de sello
        StampLine outerLine = new StampLine();
        outerLine.setText("* The Best Company *");
        outerLine.setTextRepeatType(StampTextRepeatType.FullTextRepeat);
        outerLine.getFont().setSize(12);
        outerLine.setHeight(22);
        outerLine.setTextBottomIntent(6);
        outerLine.setTextColor(Color.WHITE);
        outerLine.setBackgroundColor(Color.BLUE);
        options.getOuterLines().add(outerLine);

        // Guarde el documento sellado
        SignResult result = signature.sign("output.docx", options);
        ```        

############################# More features ############################
more_features:
  enable: true
  title: "Proteja el contenido de su documento con firmas"
  description: "La biblioteca GroupDocs.Signature for Java está diseñada para firmar y gestionar firmas en formatos de archivo populares. Agregue, modifique, verifique o elimine sellos y otros tipos de firmas sin esfuerzo."
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "Firmas de sello con GroupDocs.Signature"
  features:
    # feature loop
    - title: "Firme sus documentos"
      content: "Aplique firmas personalizables a cualquier parte de su documento. Elija entre varios tipos de firma, incluidos texto, imágenes, códigos de barras, códigos QR y sellos. Además, se pueden agregar o modificar metadatos ocultos para mejorar la seguridad del documento."

    # feature loop
    - title: "Busque y valide firmas"
      content: "Una vez que un documento esté firmado, utilice nuestras herramientas de verificación para garantizar que el contenido de la firma sea válido. Busque y recupere una lista de todas las firmas para su posterior procesamiento."

    # feature loop
    - title: "Actualice firmas según sea necesario"
      content: "Modifique una amplia gama de firmas aplicadas a un documento. Actualice propiedades como tamaño, color, posición, contenido y más."

    # feature loop
    - title: "Elimine firmas"
      content: "¿Necesita eliminar firmas de un documento? Nuestra API admite completamente la eliminación de firmas, lo que facilita la gestión eficaz de sus documentos."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Añadir sellos personalizados a documentos utilizando firmas especiales"
      content: |
        Aprenda a generar y añadir sellos personalizados con información textual importante a sus documentos.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Proporcione el documento que debe ser sellado
          Signature signature = new Signature("input.docx");

          // Instancie el objeto de opciones de sello
          StampSignOptions options = new StampSignOptions();

          // Establezca el tamaño y la posición en la página
          options.setHeight(200);
          options.setWidth(200);
          options.setVerticalAlignment(VerticalAlignment.Bottom);
          options.setHorizontalAlignment(HorizontalAlignment.Right);
          options.setAllPages(true);

          // Agregue una o más líneas externas redondas con texto
          StampLine outerLine1 = new StampLine();
          outerLine1.setText("* The best  choice *");
          outerLine1.setTextRepeatType(StampTextRepeatType.FullTextRepeat);
          SignatureFont signatureFont1 = new SignatureFont();
          signatureFont1.setSize(12);
          signatureFont1.setFamilyName("Arial");
          outerLine1.setFont(signatureFont1);
          outerLine1.setHeight(30);
          outerLine1.setTextBottomIntent(6);
          outerLine1.setTextColor(Color.WHITE);
          outerLine1.setBackgroundColor(Color.BLUE);
          options.getOuterLines().add(outerLine1);

          // Agregue una o más líneas internas cuadradas
          StampLine innerLine1 = new StampLine();
          innerLine1.setText("Company #1");
          innerLine1.setTextColor(Color.RED);
          SignatureFont signFont1 = new SignatureFont();
          signFont1.setSize(20);
          signFont1.setBold(true);
          innerLine1.setFont(signFont1);
          innerLine1.setHeight(40);
          options.getInnerLines().add(innerLine1);

          // Guarde el documento sellado
          SignResult result = signature.sign("output.docx", options);
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
            link: "/examples/signature/formats/signature_stamp.docx"
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
    title: "Explore nuestras características principales"
    exclude: "stamp"
    description: "Utilice una amplia gama de opciones para agregar, gestionar y eliminar firmas."
    items: 
          
        # operation loop 1
        - name: "Firmas electrónicas"
          operation: "esign"
          link: "/signature/java/esign/docx/"
          description: "Agrega varios tipos de firmas a formatos de archivo soportados"

        # operation loop 2
        - name: "Agregar texto a documentos"
          operation: "text"
          link: "/signature/java/text/docx/"
          description: "Mejora el contenido del documento con firmas de texto personalizables"

        # operation loop 3
        - name: "Firmas de imagen"
          operation: "image"
          link: "/signature/java/image/docx/"
          description: "Coloca cualquier imagen en cualquier posición dentro de un documento"

        # operation loop 4
        - name: "Generar códigos de barras"
          operation: "barcode"
          link: "/signature/java/barcode/docx/"
          description: "Crear e insertar varios códigos de barras en documentos soportados"

        # operation loop 5
        - name: "Generar códigos QR"
          operation: "qrcode"
          link: "/signature/java/qrcode/docx/"
          description: "Generar y utilizar códigos QR para la firma de documentos"
          
        # operation loop 6
        - name: "Certificados digitales"
          operation: "digital"
          link: "/signature/java/digital/docx/"
          description: "Asegura negocios y firma documentos con certificados digitales"

        # operation loop 7
        - name: "Firmas de sello"
          operation: "stamp"
          link: "/signature/java/stamp/docx/"
          description: "Utiliza el Constructor de Sellos para crear sellos personalizados redondos o cuadrados"
          
        # operation loop 8
        - name: "Buscar firmas"
          operation: "search"
          link: "/signature/java/search/docx/"
          description: "Ubica cualquier firma previamente añadida dentro de un documento"
          
        # operation loop 9
        - name: "Verificación de firmas"
          operation: "verify"
          link: "/signature/java/verify/docx/"
          description: "Verifica la autenticidad de las firmas después de que se han aplicado"
          
        # operation loop 10
        - name: "Modificar firmas"
          operation: "modify"
          link: "/signature/java/modify/docx/"
          description: "Edita fácilmente una variedad de firmas dentro de un documento"
          
        # operation loop 11
        - name: "Eliminar firmas"
          operation: "delete"
          link: "/signature/java/delete/docx/"
          description: "Remueve una amplia gama de firmas aplicadas previamente"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Añada sellos en múltiples formatos de archivo"
    exclude: "DOCX"
    description: "La API de GroupDocs.Signature soporta la estampación de documentos en más de 60 formatos. Coloque sellos en cualquier página o área para mejorar la gestión y personalización de documentos."
    items: 
          
        # format loop 1
        - name: "Sellar PDF"
          format: "PDF"
          link: "/signature/java/stamp/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 2
        - name: "Sellar DOCX"
          format: "DOCX"
          link: "/signature/java/stamp/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Sellar JPEG"
          format: "JPEG"
          link: "/signature/java/stamp/jpeg/"
          description: "Imagen JPEG"
          
        # format loop 4
        - name: "Sellar PPTX"
          format: "PPTX"
          link: "/signature/java/stamp/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 5
        - name: "Sellar XLSX"
          format: "XLSX"
          link: "/signature/java/stamp/xlsx/"
          description: "Hoja de Cálculo XML Abierto de Microsoft Excel"


          

---