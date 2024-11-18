



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:03
draft: false
lang: es
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Generar códigos QR en documentos JPEG con JavaScript"
head_description: "Utiliza la API de GroupDocs.Signature para crear e integrar códigos de barras 2D en archivos JPEG. Coloca códigos QR en cualquier página del documento sin complicaciones."

############################# Header ############################
title: "Crea códigos QR para JPEG" 
description: "Crea e incrusta códigos de barras 2D con contenido personalizable, incluyendo texto y datos numéricos, en varios tipos de documentos como PDF, Word, Excel e Imágenes con GroupDocs.Signature for Node.js via Java."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Pruébalo Gratis"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Explora las capacidades de GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "Aprende más"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) ofrece herramientas avanzadas de mejora de documentos, permitiendo la generación e incrustación de múltiples tipos de firma, incluyendo códigos QR, en formatos de archivo populares. Firma y asegura PDFs, documentos de Word, hojas de Excel, presentaciones de PowerPoint e imágenes con firmas de Texto, Imagen, Código de Barras, Código QR, Metadatos, Digitales y Sello.

############################# Steps ############################
steps:
    enable: true
    title: "Guía para generar e incrustar un código QR en cualquier lugar de un JPEG"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) permite la creación de códigos QR en varios formatos ampliamente utilizados y su integración en páginas de JPEG. Con más de 10 tipos distintos de códigos QR, nuestra solución puede ser incorporada sin problemas en aplicaciones Node.js via Java, enriqueciendo sus capacidades de firma con códigos QR.
      
      1. Proporciona el archivo JPEG o el flujo de datos para la firma del código QR.
      2. Introduce el texto deseado en la instancia de QrCodeSignOptions.
      3. Ajusta configuraciones visuales como color, posición, tamaño, etc.
      4. Guarda el documento que contiene el código QR.
   
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

        // Crea una instancia de Signature y pasa la ruta del documento.
        const signature = new signatureLib.Signature('input.jpeg');

        // Utiliza QrCodeSignOptions para insertar un código QR en el documento.
        // Create QR code sign options
        const options = new signatureLib.QrCodeSignOptions('Text Content');

        // Define el tipo de firma y su colocación en la página.
        options.setEncodeType(signatureLib.QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);
  
        // Almacena el documento con el código QR recién agregado.
        signature.sign('output.jpeg', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Integración integral de firmas y códigos QR"
  description: "Con la API de GroupDocs.Signature for Node.js via Java, puedes gestionar un amplio espectro de firmas. Genera, personaliza, valida, busca y elimina firmas sin dificultad en diferentes tipos de documentos, ofreciendo una flexibilidad inigualable para tus flujos de trabajo."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "Características de firma y código QR"
  features:
    # feature loop
    - title: "Firma de documentos en múltiples formatos"
      content: "Añade múltiples tipos de firmas, incluyendo Texto, Imagen, Código de Barras, Código QR y Sello a cualquier formato de documento compatible. Colócalas en cualquier página y gestiona los metadatos del documento. Asegura la seguridad del documento a través de certificados digitales para prevenir cambios no autorizados."

    # feature loop
    - title: "Validación de firmas eficaz"
      content: "Valida todas las firmas dentro de un documento para asegurarte de que cumplan con los estándares requeridos. Recupera y revisa firmas fácilmente a través de la funcionalidad de búsqueda incorporada."

    # feature loop
    - title: "Edición de firmas flexible"
      content: "Actualiza o modifica firmas existentes, ajustando aspectos como contenido, ubicación, tamaño y color, para adaptarse a las necesidades de tu documento después de la firma inicial."

    # feature loop
    - title: "Eliminación de firmas simplificada"
      content: "Elimina cualquier firma no deseada u obsoleta, incluyendo certificados digitales, sin complicaciones. El control total sobre la gestión de firmas garantiza un documento limpio y bien organizado."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Personalizando un código QR generado"
      content: |
        Este ejemplo detalla el proceso de añadir un código QR personalizado a una página de JPEG.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // Obtén el documento a firmar y pásalo a Signature.
          const signature = new signatureLib.Signature('input.jpeg');

          // Configura las opciones del código QR con el texto requerido.
          const signOptions = new signatureLib.QrCodeSignOptions('Archived on July 11, 2019');

          // Determina la posición del código QR en la página.
          signOptions.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          signOptions.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);

          // Especifica el relleno de la firma.
          const padding = new signatureLib.Padding();
          padding.setRight(20);
          padding.setTop(20);
          signOptions.setMargin(padding);

          // Elige el color del código QR.
          signOptions.setForeColor(signatureLib.Color.RED);

          // Define las opciones de fuente para el mensaje acompañante.
          const font = new signatureLib.SignatureFont();
          font.setSize(12);
          font.setFamilyName("Comic Sans MS");
          signOptions.setFont(font);

          // Personaliza el color de fondo y el cepillo para el código QR.
          const background = new signatureLib.Background();
          background.setColor(signatureLib.Color.GREEN);
          background.setTransparency(0.5);
          background.setBrush(new signatureLib.LinearGradientBrush(signatureLib.Color.GREEN, signatureLib.Color.DARK_GRAY, 0));
          signOptions.setBackground(background);

          // Incorpora el código QR en el documento.
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
            link: "/examples/signature/formats/signature_qrcode.jpeg"
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
    title: "Entiende nuestras principales capacidades"
    exclude: "qrcode"
    description: "Ofrecemos una amplia selección de formatos de firma y operaciones adaptadas a tus necesidades."
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
    title: "Integra códigos QR con varios formatos de archivo"
    exclude: "JPEG"
    description: "Aprovecha la API de Node.js via Java para generar códigos QR e incrustarlos en una variedad de formatos de archivo ampliamente utilizados. Encapsula datos importantes en estos códigos para una integración fluida y recuperación futura."
    items: 
          
        # format loop 1
        - name: "Código QR para PDF"
          format: "PDF"
          link: "/signature/nodejs-java/qrcode/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 2
        - name: "Código QR para DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/qrcode/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Código QR para JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/qrcode/jpeg/"
          description: "Imagen JPEG"
          
        # format loop 4
        - name: "Código QR para PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/qrcode/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 5
        - name: "Código QR para XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/qrcode/xlsx/"
          description: "Hoja de Cálculo XML Abierto de Microsoft Excel"


          

---