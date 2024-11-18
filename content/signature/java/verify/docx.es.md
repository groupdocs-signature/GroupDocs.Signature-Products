



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:14
draft: false
lang: es
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Verificar firmas electrónicas en DOCX usando Java"
head_description: "GroupDocs.Signature for Java permite la verificación de firmas colocadas en archivos DOCX. Valide firmas en PDF, documentos de Word, hojas de Excel, Presentaciones, Imágenes o archivos ZIP."

############################# Header ############################
title: "Verificación de firmas electrónicas para DOCX" 
description: "Verifique todas las firmas electrónicas admitidas en archivos PDF, Word, Excel, Presentaciones, Imágenes o ZIP con GroupDocs.Signature for Java."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Descargar versión gratuita"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "Aplicaciones de GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "Aprende más"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) admite operaciones CRUD completas para la firma de documentos y más. Firme más de 60 formatos de documentos, incluidos PDFs, archivos de MS Office, Imágenes y archivos ZIP, con texto, imágenes, códigos de barras, certificados digitales, metadatos y sellos. También están disponibles operaciones adicionales como buscar, verificar, modificar o eliminar firmas.

############################# Steps ############################
steps:
    enable: true
    title: "Pasos para verificar firmas en DOCX usando Java"
    content: |
      [GroupDocs.Signature](/signature/java/) puede verificar la presencia de firmas específicas en un documento DOCX. Los desarrolladores de Java pueden potenciar sus aplicaciones agregando características proporcionadas por nuestra solución.
      
      1. Cargue el archivo DOCX en la instancia de Signature.
      2. Instancie y configure VerifyOptions para lograr el resultado deseado.
      3. Inicie el proceso de verificación.
      4. Revise los resultados de la verificación.
   
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
        // Instanciar un Signature con el documento
        Signature signature = new Signature("input.docx");

        // Crear TextVerifyOptions para validar firmas que contengan texto específico
        TextVerifyOptions options = new TextVerifyOptions();
        options.setText("signature");
        options.setMatchType(TextMatchType.Contains);

        // Verificar las firmas en el documento
        VerificationResult result = signature.verify(options);

        // Procesar los resultados de la verificación
        if (result.isValid())
        {
            System.out.print("\nDocument was verified successfully!");
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Solución integral para la firma de documentos"
  description: "GroupDocs.Signature mejora los populares formatos de documentos de oficina con 7 tipos de firmas y operaciones CRUD completas, ofreciendo una sólida protección para el contenido de sus documentos."
  image: "/img/signature/features_verify.webp" # 500x500 px
  image_description: "Verificación de firmas"
  features:
    # feature loop
    - title: "Firmar documentos corporativos"
      content: "Agregue firmas digitales profesionales a cualquier documento. Nuestra solución admite varios tipos de firmas, incluidos texto, imágenes, códigos de barras, metadatos, sellos y certificados digitales."

    # feature loop
    - title: "Operaciones CRUD de firmas"
      content: "En muchos casos, los documentos firmados requieren procesamiento adicional. Recupere una lista de todas las firmas en un documento, verifíquelas, modifique sus propiedades o elimínelas cuando sea necesario."

    # feature loop
    - title: "Proteger el contenido del documento"
      content: "Proteja los documentos corporativos con certificados digitales para prevenir cambios no autorizados. Incruste metadatos ocultos para proteger aún más el contenido del documento."

    # feature loop
    - title: "Firmas nativas"
      content: "Utilice firmas de texto específicas del documento, como sellos PDF o marcas de agua de Word, para crear documentos profesionales personalizados para uso corporativo."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Verificar firmas de códigos de barras"
      content: |
        Este ejemplo demuestra cómo verificar firmas de códigos de barras en un documento.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Proporcionar el documento que contiene firmas de códigos de barras
          final Signature signature = new Signature("input.docx");

          // Configurar opciones para verificar códigos de barras contra texto específico
          BarcodeVerifyOptions options = new BarcodeVerifyOptions();
          options.setText("12345");
          options.setMatchType(TextMatchType.StartsWith);

          // Verificar las firmas que se aplicaron al documento
          VerificationResult result = signature.verify(options);

          // Mostrar los resultados de la verificación
          if (result.isValid())
          {
              System.out.print("\nDocument was verified successfully!");
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
    title: "Operaciones y tipos de firma admitidos"
    exclude: "verify"
    description: "Explore la gama completa de características y operaciones de firma admitidas por GroupDocs.Signature."
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
          
############################# More Formats #####################
more_formats:
    enable: true
    title: "Verificación de firmas en diferentes formatos de archivo"
    exclude: "DOCX"
    description: "GroupDocs.Signature for Java simplifica el proceso de verificación de todas las firmas en un documento. Establezca parámetros de verificación personalizados para asegurar la integridad de los documentos firmados."
    items: 
          
        # format loop 1
        - name: "Verificar firmas en PDF"
          format: "PDF"
          link: "/signature/java/verify/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 2
        - name: "Verificar firmas en DOCX"
          format: "DOCX"
          link: "/signature/java/verify/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Verificar firmas en PPTX"
          format: "PPTX"
          link: "/signature/java/verify/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 4
        - name: "Validar firmas en XLSX"
          format: "XLSX"
          link: "/signature/java/verify/xlsx/"
          description: "Hoja de Cálculo XML Abierto de Microsoft Excel"


          

---