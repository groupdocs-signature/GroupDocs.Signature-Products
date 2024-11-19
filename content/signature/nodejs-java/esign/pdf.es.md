



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:29
draft: false
lang: es
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Firmar PDF con firmas electrónicas en JavaScript"
head_description: "Aprovecha las capacidades de la API de JavaScript para firmar digitalmente y proteger archivos PDF, incluidos PDFs, documentos de Word, hojas de Excel, presentaciones y formatos de imagen."

############################# Header ############################
title: "Firma electrónicamente archivos PDF" 
description: "Utiliza GroupDocs.Signature for Node.js via Java para insertar diversas firmas digitales en tus documentos, asegurando la integridad de los datos y el cumplimiento para archivos como PDFs, Word, Excel, presentaciones y formatos de imagen."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Descargar ahora gratis"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Resumen de la API GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "Aprende más"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) ofrece un conjunto robusto de herramientas para agregar firmas electrónicas. Con su API intuitiva, puedes firmar, buscar, verificar, modificar y eliminar firmas de varios tipos de archivos sin necesidad de software externo. Soporta la firma fluida de PDFs, documentos de Word, hojas de Excel, diapositivas de PowerPoint y numerosos formatos de imagen.

############################# Steps ############################
steps:
    enable: true
    title: "Pasos para firmar PDF usando JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) simplifica el proceso de agregar firmas personalizadas a archivos PDF. Los desarrolladores de Node.js via Java pueden incorporar sin esfuerzo la funcionalidad de firma en sus aplicaciones.
      
      1. Carga el documento PDF en la instancia de Signature.
      2. Configura SignOptions para definir los atributos de la firma.
      3. Ajusta propiedades como tamaño, color y contenido según sea necesario.
      4. Guarda el documento firmado en la ubicación especificada.
   
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

        // Importa el documento en una instancia de Signature
        const signature = new signatureLib.Signature('input.pdf');

        // Crea un objeto QrCodeSignOptions
        const options = new signatureLib.QrCodeSignOptions('QR code text');
        
        // Especifica todas las opciones requeridas
        options.setLeft(100);
        options.setTop(100);
        options.setForeColor(new Color(255, 0, 0));

        // Guarda el documento firmado en el disco local
        signature.sign('output.pdf', options);
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Capacidades avanzadas de firmas digitales"
  description: "Nuestra API avanzada optimiza las operaciones comerciales al facilitar la firma, verificación, modificación y gestión automatizada de firmas electrónicas para una variedad de documentos."
  image: "/img/signature/features_esign.webp" # 500x500 px
  image_description: "Características de firma digital"
  features:
    # feature loop
    - title: "Firma digital para archivos de oficina"
      content: "Agrega firmas digitales a cualquier página o posición dentro de un documento. Personaliza tus firmas con opciones como certificados digitales, metadatos, códigos de barras o elementos visuales para mejorar la seguridad e integridad del documento."

    # feature loop
    - title: "Control integral de firmas"
      content: "Una vez firmado un documento, puedes gestionar sus firmas sin esfuerzo. Recupera una lista completa de todas las firmas, lo que te permite realizar actualizaciones o eliminarlas según sea necesario."

    # feature loop
    - title: "Fortalece la seguridad del documento"
      content: "Utiliza certificados digitales para proteger tus documentos contra manipulaciones. Puedes incrustar o extraer metadatos para mejorar la trazabilidad y auditoría, asegurando el cumplimiento y la autenticidad del documento."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cómo aplicar una firma de imagen a un documento"
      content: |
        Esta guía detalla el proceso para fijar una firma de imagen a una página designada dentro de un documento.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
        
          // Proporciona el documento fuente como un parámetro de entrada
          const signature = new signatureLib.Signature('input.pdf');

          // Especifica la ruta del archivo de imagen en las opciones de configuración de la firma
          const options = new signatureLib.ImageSignOptions('image.jpg');

          // Configura las dimensiones y especifica las páginas objetivo para la firma
          options.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          options.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);
          options.setHeight(150);
          options.setWidth(200);
          options.setMargin(new signatureLib.Padding(50));
          options.setAllPages(true);

          // Implementa la aplicación de la firma al documento
          signature.sign('output.pdf', options);

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
            link: "/examples/signature/formats/signature_esign.pdf"
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
    title: "Visita nuestras amplias capacidades"
    exclude: "esign"
    description: "Ofrecemos una amplia gama de tipos de firma y operaciones ricas en características."
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
    title: "Firma digitalmente múltiples tipos de archivos"
    exclude: "PDF"
    description: "La API Node.js via Java te permite aplicar firmas digitales a más de 60 formatos de archivo, brindándote amplia flexibilidad para asegurar tus documentos críticos para el negocio."
    items: 
          
        # format loop 1
        - name: "Firma electrónica PDF"
          format: "PDF"
          link: "/signature/nodejs-java/esign/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 2
        - name: "Firma electrónica DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/esign/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Firma electrónica JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/esign/jpeg/"
          description: "Imagen JPEG"
          
        # format loop 4
        - name: "Firma electrónica PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/esign/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 5
        - name: "Firma electrónica XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/esign/xlsx/"
          description: "Hoja de Cálculo XML Abierto de Microsoft Excel"


          

---