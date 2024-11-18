



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:16
draft: false
lang: es
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Verifique firmas digitales en PDF mediante JavaScript"
head_description: "Con GroupDocs.Signature for Node.js via Java, puede verificar de manera eficiente la autenticidad de las firmas en documentos PDF. Verifique sin problemas las firmas en PDFs, Word, Excel, Presentaciones, Imágenes, archivos ZIP y más."

############################# Header ############################
title: "Verifique firmas digitales en PDF" 
description: "Asegure la precisión y validez de todas las firmas electrónicas admitidas en una amplia gama de formatos de documentos, incluidos PDF, Word, Excel, Presentaciones, Imágenes y ZIP, utilizando GroupDocs.Signature for Node.js via Java."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Descargar la versión gratuita"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Aplicaciones de GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "Aprende más"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) ofrece una gestión integral de firmas de documentos, incluida la capacidad de firmar más de 60 formatos de archivo. Con soporte para texto, imagen, código de barras, certificados digitales, metadatos, sellos y más, GroupDocs.Signature for Node.js via Java le permite buscar, verificar, actualizar o eliminar firmas sin complicaciones en formatos como PDFs, documentos de MS Office, Imágenes, archivos ZIP y más.

############################# Steps ############################
steps:
    enable: true
    title: "Cómo verificar firmas en PDF utilizando JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) puede autenticar la presencia de firmas específicas en un documento PDF. Los desarrolladores de Node.js via Java pueden mejorar sus aplicaciones al incorporar nuestras características de verificación.
      
      1. Cargue el documento PDF en la instancia Signature.
      2. Cree y configure VerifyOptions para lograr los resultados de verificación deseados.
      3. Inicie el proceso de verificación.
      4. Revise y evalúe los resultados de la verificación.
   
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

        // Instancie un objeto Signature con el documento
        const signature = new signatureLib.Signature('input.pdf');

        // Establezca TextVerifyOptions para validar firmas que incluyen texto específico
        const options = new signatureLib.TextVerifyOptions();
        options.setText('signature');
        options.setMatchType(signatureLib.TextMatchType.Contains);

        // Ejecute el proceso de verificación para las firmas del documento
        const result = signature.verify(options);

        // Interprete y evalúe los resultados de la verificación
        if (result.isValid()) {
            console.log('\nDocument was verified successfully!');
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Tecnología avanzada de firma de documentos"
  description: "GroupDocs.Signature proporciona una solución integral para verificar y gestionar firmas en varios formatos de oficina. Ofreciendo siete tipos de firma y operaciones completas CRUD, permite una gestión fluida de documentos y seguridad del contenido."
  image: "/img/signature/features_verify.webp" # 500x500 px
  image_description: "Funciones de verificación de firmas"
  features:
    # feature loop
    - title: "Firme documentos corporativos con seguridad"
      content: "Aplique firmas digitales, ya sean basadas en texto, imagen, código de barras, metadatos, sellos o certificados digitales, a sus documentos de manera segura y personalizada. GroupDocs.Signature for Node.js via Java asegura un proceso de firma de documentos corporativos fluido y profesional."

    # feature loop
    - title: "Operaciones del ciclo de vida de la firma"
      content: "Gane control total sobre las firmas de documentos. Liste todas las firmas en un archivo, verifique su autenticidad, actualícelas según sea necesario o elimínelas por completo cuando sea necesario, asegurando un procesamiento adecuado de documentos."

    # feature loop
    - title: "Asegure la integridad del documento"
      content: "Utilice certificados digitales para proteger sus documentos de cambios no autorizados. Use metadatos para asegurar y rastrear el contenido del documento, garantizando que permanezca sin alteraciones y confidencial."

    # feature loop
    - title: "Firmas nativas personalizadas"
      content: "Agregue firmas nativas personalizadas como stickers en PDFs o marcas de agua en documentos de Word. Estas opciones personalizables permiten un manejo profesional y seguro de documentos, perfectamente adaptadas a entornos corporativos."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Proceso de verificación de firmas de código de barras"
      content: |
        Este ejemplo ilustra la metodología para autenticar firmas de código de barras incrustadas en un documento.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // Envíe el documento que presenta firmas de código de barras
          const signature = new signatureLib.Signature('input.pdf');

          // Configure los parámetros para validar los códigos de barras contra el texto designado
          const options = new signatureLib.BarcodeVerifyOptions();
          options.setText('12345');
          options.setMatchType(signatureLib.TextMatchType.StartsWith);

          // Autentique las firmas previamente adjuntas al documento
          const result = signature.verify(options);

          // Revise el informe de validación
          if (result.isValid()) {
              console.log('\nDocument was verified successfully!');
          }
          ```
        platform: "nodejs-java"
        copy_title: "Copiar"
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
    title: "Funciones completas y firmas admitidas"
    exclude: "verify"
    description: "Explore las capacidades avanzadas de GroupDocs.Signature, que presenta una amplia gama de herramientas y operaciones para la gestión de firmas, mejorando los flujos de trabajo de documentos."
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
    title: "Validación integral de firmas para varios formatos"
    exclude: "PDF"
    description: "GroupDocs.Signature for Node.js via Java simplifica la verificación de firmas en múltiples formatos de documentos, ofreciendo controles robustos para las verificaciones de firmas. Personalice su proceso de verificación y asegúrese de que los documentos estén firmados adecuadamente."
    items: 
          
        # format loop 1
        - name: "Verificar firmas en PDF"
          format: "PDF"
          link: "/signature/nodejs-java/verify/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 2
        - name: "Verificar firmas en DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/verify/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Verificar firmas en PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/verify/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 4
        - name: "Validar firmas en XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/verify/xlsx/"
          description: "Hoja de Cálculo XML Abierto de Microsoft Excel"


          

---