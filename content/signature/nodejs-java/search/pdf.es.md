



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:32
draft: false
lang: es
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Buscar firmas electrónicas en archivos PDF con JavaScript"
head_description: "Aprovecha el poder de la API GroupDocs.Signature for Node.js via Java para detectar y buscar firmas electrónicas en PDFs, documentos de Word, hojas de cálculo de Excel, presentaciones e imágenes."

############################# Header ############################
title: "Buscar firmas electrónicas en PDF" 
description: "Descubre y recupera información detallada sobre todas las firmas incorporadas en archivos PDF, Word, Excel, presentaciones e imágenes utilizando las herramientas avanzadas que ofrece GroupDocs.Signature for Node.js via Java."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Comienza gratis"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Descripción general de GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "Aprende más"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) ofrece un marco robusto para gestionar firmas digitales a través de una amplia gama de tipos de archivo. Con soporte para más de 60 formatos como PDF, documentos de Microsoft Office, imágenes y archivos ZIP, la API permite a los usuarios aplicar, localizar, verificar, actualizar o eliminar una variedad de tipos de firma, incluidas texto, imágenes, códigos de barras, certificados digitales y más.

############################# Steps ############################
steps:
    enable: true
    title: "Guía para buscar firmas en PDF utilizando JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) proporciona una herramienta poderosa para localizar firmas digitales dentro de archivos PDF. Los desarrolladores de Node.js via Java pueden ampliar fácilmente la funcionalidad de su aplicación con nuestra solución.
      
      1. Especifica la ruta del archivo PDF para la búsqueda de firmas.
      2. Utiliza SearchOptions para filtrar los resultados de búsqueda.
      3. Ejecuta el método Search para encontrar las firmas.
      4. Revisa la lista de firmas descubiertas.
   
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

        // Crea un objeto Signature utilizando la ruta del documento
        const signature = new signatureLib.Signature('input.pdf');

        // Configura TextSearchOptions para incluir cada página
        const options = new signatureLib.TextSearchOptions();
        options.setAllPages(true);

        // Realiza una búsqueda para localizar todas las firmas de texto dentro del documento
        const signatures = signature.search(signatureLib.TextSignature.class, options).toArray();
        console.log(`\nSource document contains the following text signature(s).`);

        // Agrega las firmas descubiertas para un análisis completo
        for (const textSignature of signatures) {
            console.log(`Found Text signature at page ${textSignature.getPageNumber()} 
            with type [${textSignature.getSignatureImplementation()}] and text '${textSignature.getText()}'.`);
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Solución completa para la gestión de firmas"
  description: "GroupDocs.Signature for Node.js via Java proporciona una solución integral para añadir, modificar, buscar y verificar firmas electrónicas en formatos de documentos populares. Potencia tus flujos de trabajo con características avanzadas de firma de documentos."
  image: "/img/signature/features_search.webp" # 500x500 px
  image_description: "Funciones de detección de firmas"
  features:
    # feature loop
    - title: "Firmar digitalmente archivos comerciales"
      content: "Añade firmas electrónicas como texto, imágenes, códigos de barras y certificados digitales en cualquier ubicación de tus documentos. GroupDocs.Signature soporta la firma en PDFs, Word, Excel, imágenes y más, asegurando una gestión flexible de documentos."

    # feature loop
    - title: "Gestión eficiente de firmas"
      content: "Después de firmar, localiza fácilmente todas las firmas incrustadas en un documento. La API permite una búsqueda y recuperación exhaustiva de firmas, así como la capacidad de actualizarlas o eliminarlas."

    # feature loop
    - title: "Seguridad del documento y gestión de metadatos"
      content: "Asegura la integridad de tus documentos incrustando o eliminando metadatos ocultos. Protege tus archivos de cambios no autorizados utilizando certificados digitales para sellar y autenticar el contenido del documento."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Identificación de firmas de imagen"
      content: |
        Este ejemplo ilustra cómo detectar una firma de imagen dentro de un documento específico.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // Proporciona el documento fuente como parámetro al constructor
          const signature = new signatureLib.Signature('input.pdf');

          // Busca cualquier firma que sea de tipo texto
          const signatures = signature.search(signatureLib.ImageSignature.class, signatureLib.SignatureType.Image).toArray();
          console.log(`\nSource document contains the following image signature(s).`);

          // Muestra los hallazgos con propiedades completas de las firmas detectadas
          for (const imageSignature of signatures) {
              console.log(`Found Image signature at page ${imageSignature.getPageNumber()} 
              and size ${imageSignature.getSize()}.`);
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
    title: "Funcionalidades clave"
    exclude: "search"
    description: "Nuestra API integral ofrece una variedad de operaciones diseñadas para optimizar la gestión de firmas de documentos, desde la firma hasta el posprocesamiento y la verificación."
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
    title: "Localiza firmas en múltiples tipos de archivos"
    exclude: "PDF"
    description: "Con la API GroupDocs.Signature for Node.js via Java, puedes buscar y recuperar eficientemente firmas electrónicas de una amplia gama de formatos de archivo compatibles, facilitando una integración perfecta en tus flujos de trabajo documentales."
    items: 
          
        # format loop 1
        - name: "Buscar firmas en PDF"
          format: "PDF"
          link: "/signature/nodejs-java/search/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 2
        - name: "Encontrar firmas en DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/search/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Encontrar firmas en PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/search/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 4
        - name: "Buscar firmas en XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/search/xlsx/"
          description: "Hoja de Cálculo XML Abierto de Microsoft Excel"


          

---