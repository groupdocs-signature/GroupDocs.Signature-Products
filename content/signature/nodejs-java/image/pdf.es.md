



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:10
draft: false
lang: es
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Añadiendo firmas de imagen a archivos PDF con JavaScript"
head_description: "Coloca la firma de imagen en archivos PDF para Node.js utilizando unas pocas líneas de código. Utiliza la API de GroupDocs.Signature for Node.js via Java para agregar imágenes."

############################# Header ############################
title: "Firma archivos PDF utilizando firmas de imagen" 
description: "Aprovecha las capacidades de GroupDocs.Signature for Node.js via Java para incrustar imágenes en una multitud de formatos de documentos de oficina, como PDFs, Word, Excel y varios formatos de imagen. Agregar una imagen de firma ejecutiva puede mejorar significativamente la profesionalidad y credibilidad de tus documentos, creando una presentación refinada y pulida."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Descargar gratis"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Presentamos GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "Aprende más"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) permite a los usuarios incorporar firmas de imagen en cualquier ubicación dentro de sus documentos. Esta herramienta permite a las empresas optimizar sus flujos de trabajo al añadir imágenes a PDFs, Word, Excel, PowerPoint y formatos de imagen populares, mejorando la eficiencia en la gestión de documentos.

############################# Steps ############################
steps:
    enable: true
    title: "Guía para añadir imágenes en PDF utilizando JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) permite a las aplicaciones Node.js via Java integrar firmas de imagen sin problemas en documentos PDF. Mejora las capacidades de tu aplicación con nuestra biblioteca integral.
      
      1. Instancia Signature con el documento PDF
      2. Utiliza ImageSignOptions para especificar la imagen de firma
      3. Posiciona la imagen con precisión en cualquier página
      4. Guarda el documento firmado en la ubicación deseada
   
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

        // Inicializa Signature con la ruta al documento
        const signature = new signatureLib.Signature('input.pdf');

        // Configura ImageSignOptions para incluir la firma de imagen deseada
        const options = new signatureLib.ImageSignOptions('company_logo.jpg');

        // Coloca la imagen en la esquina superior izquierda de todas las páginas
        options.setAllPages(true);
        options.setLeft(100);
        options.setTop(200);
        
        // Guarda el documento con la firma de imagen aplicada
        const result = signature.sign('output.pdf', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Capacidades avanzadas de firma de documentos"
  description: "Nuestra API ofrece un conjunto de características que simplifican la firma electrónica. Puedes agregar, modificar, eliminar, buscar y verificar múltiples tipos de firmas, incluidas las firmas de imagen, con eficacia."
  image: "/img/signature/features_image.webp" # 500x500 px
  image_description: "Firmas de imagen"
  features:
    # feature loop
    - title: "Incorpora imágenes en documentos de oficina"
      content: "Coloca firmas de imagen en cualquier parte de tu documento, ya sea en archivos PDFs, Word o Excel. Mejora tus documentos añadiendo imágenes, códigos de barras, metadatos o certificados digitales para añadir funcionalidad."

    # feature loop
    - title: "Buscar y validar firmas"
      content: "Asegura la autenticidad de tus documentos firmados verificando las firmas. Utiliza la funcionalidad de búsqueda para recuperar y revisar todas las firmas incrustadas en tu documento."

    # feature loop
    - title: "Modificar firmas existentes"
      content: "Nuestra API permite a los usuarios actualizar y ajustar las firmas según sea necesario. Modifica el tamaño, la posición u otros atributos de cualquier firma previamente añadida para mayor flexibilidad en el manejo de documentos."

    # feature loop
    - title: "Eliminar firmas innecesarias"
      content: "Gestiona eficientemente tus documentos eliminando firmas que ya no son necesarias. Nuestra API soporta operaciones CRUD completas para casi todos los tipos de firmas."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Mejora los documentos con firmas de imagen"
      content: |
        Aprende cómo incorporar imágenes en documentos empresariales para añadir información suplementaria.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // Selecciona el documento a ser firmado
          const signature = new signatureLib.Signature('input.pdf');

          // Configura las opciones de imagen con la ruta de la imagen
          const options = new signatureLib.ImageSignOptions('manager_signature.jpg');

          // Ajusta el tamaño de la firma de imagen
          options.setWidth(100);
          options.setHeight(100);

          // Coloca la imagen en la esquina inferior derecha
          options.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          options.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);

          // Aplica un margen desde las esquinas de la página si es necesario
          const padding = new signatureLib.Padding();
          padding.setRight(120);
          padding.setBottom(120);
          options.setMargin(padding);

          // Opcionalmente, añade un borde personalizado a la imagen
          const border = new signatureLib.Border();
          border.setColor(signatureLib.Color.RED);
          border.setDashStyle(signatureLib.DashStyle.DashDotDot);
          border.setWeight(5);
          border.setVisible(true);
          options.setBorder(border);

          // Rota la firma de imagen para una apariencia óptima
          options.setRotationAngle(45);

          // Guarda el documento actualizado en la ubicación deseada
          const result = signature.sign('output.pdf', options);
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
            link: "/examples/signature/formats/signature_image.pdf"
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
    title: "Descubre las funciones que ofrecemos"
    exclude: "image"
    description: "Estamos orgullosos de presentar una amplia selección de métodos y operaciones de firma."
    items: 
          
        # operation loop 1
        - name: "Firmas electrónicas"
          operation: "esign"
          link: "/signature/nodejs-java/esign/pdf/"
          description: "Agrega varios tipos de firmas a formatos de archivo soportados"

        # operation loop 2
        - name: "Agregar texto a documentos"
          operation: "text"
          link: "/signature/nodejs-java/text/pdf/"
          description: "Mejora el contenido del documento con firmas de texto personalizables"

        # operation loop 3
        - name: "Firmas de imagen"
          operation: "image"
          link: "/signature/nodejs-java/image/pdf/"
          description: "Coloca cualquier imagen en cualquier posición dentro de un documento"

        # operation loop 4
        - name: "Generar códigos de barras"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/pdf/"
          description: "Crear e insertar varios códigos de barras en documentos soportados"

        # operation loop 5
        - name: "Generar códigos QR"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/pdf/"
          description: "Generar y utilizar códigos QR para la firma de documentos"
          
        # operation loop 6
        - name: "Certificados digitales"
          operation: "digital"
          link: "/signature/nodejs-java/digital/pdf/"
          description: "Asegura negocios y firma documentos con certificados digitales"

        # operation loop 7
        - name: "Firmas de sello"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/pdf/"
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
    title: "Agregar imágenes a varios tipos de archivos"
    exclude: "PDF"
    description: "La API de Node.js via Java te permite incrustar imágenes en una amplia gama de formatos de documento. Personaliza el tamaño, la colocación y la posición en la página para mejorar tu proceso de firma de documentos."
    items: 
          
        # format loop 1
        - name: "Firmar PDF con imagen"
          format: "PDF"
          link: "/signature/nodejs-java/image/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 2
        - name: "Firmar DOCX con imagen"
          format: "DOCX"
          link: "/signature/nodejs-java/image/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Firmar JPEG con imagen"
          format: "JPEG"
          link: "/signature/nodejs-java/image/jpeg/"
          description: "Imagen JPEG"
          
        # format loop 4
        - name: "Firmar PPTX con imagen"
          format: "PPTX"
          link: "/signature/nodejs-java/image/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 5
        - name: "Firmar XLSX con imagen"
          format: "XLSX"
          link: "/signature/nodejs-java/image/xlsx/"
          description: "Hoja de Cálculo XML Abierto de Microsoft Excel"


          

---