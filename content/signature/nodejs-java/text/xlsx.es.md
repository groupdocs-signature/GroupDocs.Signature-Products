



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:55
draft: false
lang: es
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Agregar firmas de texto a XLSX a través de JavaScript"
head_description: "Utiliza la API de JavaScript para integrar sin problemas firmas de texto en documentos XLSX. Nuestra API admite una amplia gama de formatos, incluidos PDF, Word, Excel, Presentaciones, Imágenes y archivos ZIP."

############################# Header ############################
title: "Agregar firmas de texto a XLSX" 
description: "Incorpora firmas de texto personalizadas en tus archivos comerciales con GroupDocs.Signature for Node.js via Java. Toma el control de tus flujos de trabajo documentales mejorándolos con opciones de firma seguras y personalizables."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Comienza la prueba gratuita"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Presentando GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "Aprende más"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) es una solución innovadora diseñada para facilitar la adición de firmas de texto a documentos. Personaliza y coloca firmas en cualquier página, mejorando la eficiencia en el manejo de documentos. Optimiza los flujos de trabajo de tu organización integrando marcas de texto personalizadas que mejoran tanto la funcionalidad como el profesionalismo.

############################# Steps ############################
steps:
    enable: true
    title: "Guía para crear firmas de texto para XLSX usando JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) permite la adición de firmas de texto a documentos XLSX en aplicaciones Node.js via Java. Mejora rápidamente las capacidades de tu producto con nuestras robustas soluciones.
      
      1. Proporciona el documento XLSX como argumento a la clase Signature.
      2. Instancia TextSignOptions con el texto requerido.
      3. Establece las propiedades visuales de la firma de texto.
      4. Agrega la firma de texto a la(s) página(s) deseadas del documento.
   
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

        // Inicializa la clase Signature con la ruta del documento
        const signature = new signatureLib.Signature('input.xlsx');

        // Crea TextSignOptions con el texto de firma requerido
        const options = new signatureLib.TextSignOptions('Approved');

        // Configura el color y las propiedades de fuente del texto
        options.setForeColor(new signatureLib.Color(255, 0, 0));
        const signatureFont = new signatureLib.SignatureFont();
        signatureFont.setSize(12);
        signatureFont.setFamilyName('Comic Sans MS');
        options.setFont(signatureFont);
        
        // Agrega la firma de texto al documento
        const result = signature.sign('output.xlsx', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Control mejorado de firmas de texto"
  description: "Con GroupDocs.Signature for Node.js via Java, puedes mejorar significativamente la gestión de firmas basadas en texto en formatos de documentos clave. La herramienta te permite configurar el estilo, la ubicación y el contenido de las firmas de manera eficaz, permitiendo a las empresas adaptar sus procesos documentales."
  image: "/img/signature/features_text.webp" # 500x500 px
  image_description: "Características centrales de GroupDocs.Signature"
  features:
    # feature loop
    - title: "Firmas de documentos dinámicas"
      content: "Inserta varios tipos de firmas—como texto, imágenes, códigos de barras, códigos QR o sellos—en cualquier página de documentos soportados. Incorpora metadatos para llevar información oculta o aplica certificados digitales para medidas de seguridad avanzadas."

    # feature loop
    - title: "Búsqueda y validación de firmas"
      content: "Verifica la autenticidad de las firmas incrustadas dentro de tus documentos. Realiza búsquedas eficientes para localizar todas las instancias de firmas, asegurando un seguimiento y gestión exhaustivos de los documentos."

    # feature loop
    - title: "Editar o eliminar firmas"
      content: "Modifica o elimina las firmas previamente añadidas según sea necesario. Puedes ajustar la apariencia, la posición o el contenido de cualquier firma para cumplir con requerimientos en evolución, asegurando flexibilidad en el manejo de documentos."

    # feature loop
    - title: "Personalización nativa de firmas"
      content: "Para ciertos tipos de archivos, personaliza la colocación de firmas con características integradas en el documento, como agregar marcas de agua a archivos de Word o sellos personalizados a PDFs, mejorando la singularidad de tus documentos."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Implementar firmas de texto en documentos"
      content: |
        Aprende cómo incrustar firmas de texto en documentos comerciales para optimizar procesos.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // Selecciona el documento que se va a firmar
          const signature = new signatureLib.Signature('input.xlsx');

          // Define las opciones de texto con el contenido especificado
          const options = new signatureLib.TextSignOptions('Rescheduled to 03/04/2025');

          // Establece el tamaño y la posición de la firma en la página
          options.setLeft(100);
          options.setTop(180);
          options.setWidth(230);
          options.setHeight(30);

          // Aplica un espaciado para la firma desde los bordes de la página
          const padding = new signatureLib.Padding();
          padding.setBottom(20);
          padding.setRight(20);
          options.setMargin(padding);

          // Personaliza el color del texto y el estilo de fuente
          options.setForeColor(signatureLib.Color.RED);
          const signatureFont = new signatureLib.SignatureFont();
          signatureFont.setSize(12);
          signatureFont.setFamilyName('Comic Sans MS');
          options.setFont(signatureFont);

          // Agrega un borde a la firma de texto si se desea
          const border = new signatureLib.Border();
          border.setColor(signatureLib.Color.RED);
          border.setDashStyle(signatureLib.DashStyle.Dash);
          border.setTransparency(0.5);
          border.setVisible(true);
          border.setWeight(2);
          options.setBorder(border);

          // Configura el fondo de la firma
          const background = new signatureLib.Background();
          background.setColor(signatureLib.Color.YELLOW);
          background.setTransparency(0.8);
          options.setBackground(background);

          // Opcionalmente, guarda el texto como una imagen para compatibilidad
          options.setSignatureImplementation(signatureLib.TextSignatureImplementation.Image);
          
          // Guarda el documento con la firma de texto añadida
          const result = signature.sign('output.xlsx', options);
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
            link: "/examples/signature/formats/signature_text.xlsx"
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
    title: "Características de gestión de firmas completas"
    exclude: "text"
    description: "Nuestra plataforma ofrece operaciones CRUD completas y características avanzadas para la gestión de siete tipos de firmas distintas, permitiéndote administrar tus firmas documentales con precisión y eficacia."
    items: 
          
        # operation loop 1
        - name: "Firmas electrónicas"
          operation: "esign"
          link: "/signature/nodejs-java/esign/xlsx/"
          description: "Agrega varios tipos de firmas a formatos de archivo soportados"

        # operation loop 2
        - name: "Agregar texto a documentos"
          operation: "text"
          link: "/signature/nodejs-java/text/xlsx/"
          description: "Mejora el contenido del documento con firmas de texto personalizables"

        # operation loop 3
        - name: "Firmas de imagen"
          operation: "image"
          link: "/signature/nodejs-java/image/xlsx/"
          description: "Coloca cualquier imagen en cualquier posición dentro de un documento"

        # operation loop 4
        - name: "Generar códigos de barras"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/xlsx/"
          description: "Crear e insertar varios códigos de barras en documentos soportados"

        # operation loop 5
        - name: "Generar códigos QR"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/xlsx/"
          description: "Generar y utilizar códigos QR para la firma de documentos"
          
        # operation loop 6
        - name: "Certificados digitales"
          operation: "digital"
          link: "/signature/nodejs-java/digital/xlsx/"
          description: "Asegura negocios y firma documentos con certificados digitales"

        # operation loop 7
        - name: "Firmas de sello"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/xlsx/"
          description: "Utiliza el Constructor de Sellos para crear sellos personalizados redondos o cuadrados"
          
        # operation loop 8
        - name: "Buscar firmas"
          operation: "search"
          link: "/signature/nodejs-java/search/xlsx/"
          description: "Ubica cualquier firma previamente añadida dentro de un documento"
          
        # operation loop 9
        - name: "Verificación de firmas"
          operation: "verify"
          link: "/signature/nodejs-java/verify/xlsx/"
          description: "Verifica la autenticidad de las firmas después de que se han aplicado"
          
        # operation loop 10
        - name: "Modificar firmas"
          operation: "modify"
          link: "/signature/nodejs-java/modify/xlsx/"
          description: "Edita fácilmente una variedad de firmas dentro de un documento"
          
        # operation loop 11
        - name: "Eliminar firmas"
          operation: "delete"
          link: "/signature/nodejs-java/delete/xlsx/"
          description: "Remueve una amplia gama de firmas aplicadas previamente"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Aplica firmas de texto en varios formatos"
    exclude: "XLSX"
    description: "Aprovecha las capacidades de la API Node.js via Java para integrar firmas basadas en texto en una amplia gama de formatos de Office. Controla el flujo de información en cada etapa de tu ciclo de vida de documentos al agregar marcas de texto altamente personalizables."
    items: 
          
        # format loop 1
        - name: "Firmas de texto PDF"
          format: "PDF"
          link: "/signature/nodejs-java/text/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 2
        - name: "Firmas de texto DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/text/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Firmas de texto JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/text/jpeg/"
          description: "Imagen JPEG"
          
        # format loop 4
        - name: "Firmas de texto PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/text/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 5
        - name: "Firmas de texto XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/text/xlsx/"
          description: "Hoja de Cálculo XML Abierto de Microsoft Excel"


          

---