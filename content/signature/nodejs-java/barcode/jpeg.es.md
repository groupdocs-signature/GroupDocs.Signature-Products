



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:07
draft: false
lang: es
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Generar código de barras para JPEG utilizando aplicaciones JavaScript"
head_description: "Genera rápidamente e incrusta una firma de código de barras en un documento JPEG con JavaScript usando solo unas pocas líneas de código. GroupDocs.Signature admite la firma en múltiples formatos de archivo."

############################# Header ############################
title: "Genera y añade códigos de barras en JPEG sin esfuerzo" 
description: "Utiliza GroupDocs.Signature for Node.js via Java para incorporar códigos de barras en tus documentos empresariales, colocándolos exactamente donde los necesites. Nuestra solución ofrece amplias opciones de personalización para adaptar las firmas de código de barras a tus requisitos."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Descargar Ahora – ¡Es Gratis!"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Una introducción a GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "Aprende más"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) es una poderosa herramienta de firma de documentos, que admite una diversa gama de tipos de firmas, incluyendo texto, imágenes, códigos de barras, certificados digitales y sellos. Con compatibilidad en más de 60 formatos de archivo, como PDFs, archivos de MS Office, imágenes y archivos ZIP, permite una gestión integral de documentos. Las firmas dentro de los documentos pueden ser buscadas, verificadas, modificadas o eliminadas según sea necesario.

############################# Steps ############################
steps:
    enable: true
    title: "Cómo generar e incrustar códigos de barras en archivos JPEG"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) permite la generación y colocación de códigos de barras en una variedad de formatos populares en páginas JPEG. Con soporte para más de 60 tipos de códigos de barras, las aplicaciones Node.js via Java se pueden mejorar fácilmente con funciones de firma de códigos de barras integrando nuestra biblioteca.
      
      1. Proporcionar el archivo JPEG o flujo para su procesamiento.
      2. Pasar el texto del código de barras a una instancia de BarcodeSignOptions.
      3. Ajustar la configuración del código de barras, como posición, tamaño, etc.
      4. Guardar el documento con el código de barras recién añadido.
   
    code:
      platform: "nodejs-java"
      copy_title: "Copiar"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Firmas de muestra"
      install:
        command: "npm i @groupdocs/groupdocs.signature"
        copy_tip: "haz clic para copiar"
        copy_done: "copiado"
      links:
        #  loop
        - title: "Más ejemplos"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
        #  loop
        - title: "Documentación"
          link: "https://docs.groupdocs.com/signature/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')

        // Instanciar un objeto Signature con la ruta del documento
        const signature = new signatureLib.Signature('input.jpeg');

        // Utilizar BarcodeSignOptions para integrar un código de barras en el documento
        const options = new signatureLib.BarcodeSignOptions('Business data');

        // Configurar el tipo de código de barras y parámetros adicionales
        options.setEncodeType(signatureLib.BarcodeTypes.Code128);
        options.setLeft(100);
        options.setTop(100);
  
        // Guardar el documento firmado
        signature.sign('output.jpeg', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Aumenta y protege tus documentos con opciones avanzadas de firma"
  description: "La biblioteca GroupDocs.Signature for Node.js via Java está diseñada para facilitar la firma y la gestión posterior de formatos de documento populares. Añade, modifica, verifica o elimina rápidamente una amplia gama de firmas."
  image: "/img/signature/features_barcode.webp" # 500x500 px
  image_description: "Funcionalidades clave de GroupDocs.Signature"
  features:
    # feature loop
    - title: "Firma dinámica de documentos"
      content: "Firma cualquier página de tus documentos utilizando una variedad de tipos de firma, incluyendo texto, imágenes, códigos de barras, códigos QR y sellos. Además, puedes incrustar metadatos ocultos, como datos EXIF en imágenes, o asegurar el documento contra ediciones no autorizadas utilizando certificados digitales."

    # feature loop
    - title: "Verificación y búsqueda de firmas robustas"
      content: "Nuestra solución proporciona herramientas extensas para gestionar documentos firmados. Verifica la autenticidad de las firmas para garantizar la integridad del documento y utiliza la función de búsqueda para listar todas las firmas incrustadas dentro de un documento."

    # feature loop
    - title: "Modifica firmas con facilidad"
      content: "La mayoría de las firmas añadidas anteriormente se pueden modificar con facilidad. Actualiza el texto, repositiona o cambia la apariencia de la firma para adaptarla a tus necesidades."

    # feature loop
    - title: "Eliminación de firmas simplificada"
      content: "Con un soporte integral para operaciones CRUD, nuestra herramienta permite la eliminación eficiente de firmas de tus documentos, asegurando que solo las firmas más relevantes permanezcan."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cómo aplicar una firma de código de barras"
      content: |
        Este ejemplo ilustra cómo incrustar un código de barras personalizado en las páginas del documento JPEG.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // Proporcionar el documento a firmar.
          const signature = new signatureLib.Signature('input.jpeg');

          // Utilizar BarcodeSignOptions para integrar un código de barras en el documento
          const signOptions = new signatureLib.BarcodeSignOptions('Accepted');
          signOptions.setEncodeType(signatureLib.BarcodeTypes.Code39FullASCII);

          // Configurar el tipo de código de barras y parámetros adicionales
          signOptions.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          signOptions.setHorizontalAlignment(signatureLib.HorizontalAlignment.Left);

          // Definir el relleno del código de barras desde el borde de la página.
          const padding = new signatureLib.Padding();
          padding.setLeft(20);
          padding.setTop(180);
          signOptions.setMargin(padding);

          // Elegir el color de las barras.
          signOptions.setForeColor(signatureLib.Color.RED);

          // Especificar el estilo de fuente para el mensaje.
          const font = new signatureLib.SignatureFont();
          font.setSize(12);
          font.setFamilyName('Arial');
          signOptions.setFont(font);

          // Indicar la posición del mensaje.
          signOptions.setCodeTextAlignment(signatureLib.CodeTextAlignment.Above);

          // Firmar y guardar el documento.
          signature.sign('output.jpeg', signOptions);

          ```
        platform: "nodejs-java"
        copy_title: "Copiar"
        install:
          command: "npm i @groupdocs/groupdocs.signature"
          copy_tip: "haz clic para copiar"
          copy_done: "copiado"
        top_links:
          #  loop
          - title: "Descargar resultado"
            icon: "download"
            link: "/examples/signature/formats/signature_barcode.jpeg"
        links:
          #  loop
          - title: "Más ejemplos"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
          #  loop
          - title: "Documentación"
            link: "https://docs.groupdocs.com/signature/nodejs-java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "¿Listo para empezar?"
  description: "Prueba las funciones de GroupDocs.Signature de forma gratuita o solicita una licencia"
  items:
    #  loop
    - title: "Descarga de NPM"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      color: "red"
        #  loop
    - title: "Licenciamiento"
      link: "https://purchase.groupdocs.com/pricing/signature/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Profundiza en nuestras características principales"
    exclude: "barcode"
    description: "Experimenta una amplia gama de tipos de firma y herramientas que ofrecemos."
    items: 
          
        # operation loop 1
        - name: "Firmas electrónicas"
          operation: "esign"
          link: "/signature/nodejs-java/esign/jpeg/"
          description: "Agrega varios tipos de firmas a formatos de archivo soportados"

        # operation loop 2
        - name: "Agregar texto a documentos"
          operation: "text"
          link: "/signature/nodejs-java/text/jpeg/"
          description: "Mejora el contenido del documento con firmas de texto personalizables"

        # operation loop 3
        - name: "Firmas de imagen"
          operation: "image"
          link: "/signature/nodejs-java/image/jpeg/"
          description: "Coloca cualquier imagen en cualquier posición dentro de un documento"

        # operation loop 4
        - name: "Generar códigos de barras"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/jpeg/"
          description: "Crear e insertar varios códigos de barras en documentos soportados"

        # operation loop 5
        - name: "Generar códigos QR"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/jpeg/"
          description: "Generar y utilizar códigos QR para la firma de documentos"
          
        # operation loop 6
        - name: "Certificados digitales"
          operation: "digital"
          link: "/signature/nodejs-java/digital/pdf/"
          description: "Asegura negocios y firma documentos con certificados digitales"

        # operation loop 7
        - name: "Firmas de sello"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/jpeg/"
          description: "Utiliza el Constructor de Sellos para crear sellos personalizados redondos o cuadrados"
          
        # operation loop 8
        - name: "Buscar firmas"
          operation: "search"
          link: "/signature/nodejs-java/search/pdf/"
          description: "Ubica cualquier firma previamente añadida dentro de un documento"
          
        # operation loop 9
        - name: "Verificación de firmas"
          operation: "verify"
          link: "/signature/nodejs-java/verify/pdf/"
          description: "Verifica la autenticidad de las firmas después de que se han aplicado"
          
        # operation loop 10
        - name: "Modificar firmas"
          operation: "modify"
          link: "/signature/nodejs-java/modify/pdf/"
          description: "Edita fácilmente una variedad de firmas dentro de un documento"
          
        # operation loop 11
        - name: "Eliminar firmas"
          operation: "delete"
          link: "/signature/nodejs-java/delete/pdf/"
          description: "Remueve una amplia gama de firmas aplicadas previamente"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Firma en múltiples formatos de documento"
    exclude: "JPEG"
    description: "La API Node.js via Java te permite firmar más de 60 formatos diferentes. Ya sea añadiendo firmas a páginas específicas o colocándolas con precisión, nuestra herramienta facilita la aplicación de varios tipos de firmas."
    items: 
          
        # format loop 1
        - name: "Agregar código de barras a PDF"
          format: "PDF"
          link: "/signature/nodejs-java/barcode/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 2
        - name: "Agregar código de barras a DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/barcode/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Agregar código de barras a JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/barcode/jpeg/"
          description: "Imagen JPEG"
          
        # format loop 4
        - name: "Agregar código de barras a PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/barcode/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 5
        - name: "Agregar código de barras a XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/barcode/xlsx/"
          description: "Hoja de Cálculo XML Abierto de Microsoft Excel"


          

---