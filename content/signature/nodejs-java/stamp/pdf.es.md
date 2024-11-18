



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:48
draft: false
lang: es
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Generar y añadir sellos a PDF mediante JavaScript"
head_description: "Aproveche el poder de GroupDocs.Signature y JavaScript para generar y colocar sellos personalizados en cualquier página de sus documentos PDF."

############################# Header ############################
title: "Inserte sellos personalizados en archivos PDF" 
description: "Utilice GroupDocs.Signature for Node.js via Java para generar sellos a medida e insertarlos en cualquier ubicación de sus documentos. Nuestra plataforma ofrece amplias opciones para personalizar sellos de acuerdo a sus requisitos empresariales específicos."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Prueba gratuita"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "¿Qué es GroupDocs.Signature for Node.js via Java?"
    link: "/signature/nodejs-java/"
    link_title: "Aprende más"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) proporciona una solución robusta y versátil para la firma de documentos. Permite a los usuarios añadir sellos y otros tipos de firmas en más de 60 formatos diferentes, como PDFs, Word, Excel, archivos de imagen y archivos ZIP. La plataforma permite insertar texto, imágenes, códigos de barras, códigos QR, metadatos, certificados digitales y firmas de sellos. Además de firmar, puede buscar, verificar, modificar o eliminar cualquier firma presente en sus documentos.

############################# Steps ############################
steps:
    enable: true
    title: "Guía para incrustar sellos en PDF usando JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) proporciona una herramienta poderosa para crear e incrustar sellos, lo que puede mejorar significativamente las aplicaciones Node.js via Java. Utilice esta característica para crear y aplicar sellos personalizados a las páginas de su documento.
      
      1. Introduzca el documento PDF que necesita ser sellado.
      2. Despliegue StampSignOptions para definir todos los parámetros esenciales.
      3. Inserte tantas líneas de sello como sea necesario.
      4. Aplique el sello y guarde el documento finalizado.
   
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

        // Asocie la ruta del documento con la instancia de Signature
        const signature = new signatureLib.Signature('input.pdf');

        // Cree StampSignOptions con el contenido de firma necesario
        const options = new signatureLib.StampSignOptions();
        options.Height = 180;
        options.Width = 180;

        // Incorpore una o más líneas de sello
        const outerLine = new signatureLib.StampLine();
        outerLine.setText("* The Best Company *");
        outerLine.setTextRepeatType(signatureLib.StampTextRepeatType.FullTextRepeat);
        outerLine.getFont().setSize(12);
        outerLine.setHeight(22);
        outerLine.setTextBottomIntent(6);
        outerLine.setTextColor(signatureLib.Color.WHITE);
        outerLine.setBackgroundColor(signatureLib.Color.BLUE);
        options.getOuterLines().add(outerLine);

        // Guarde el documento con el sello aplicado
        const result = signature.sign('output.pdf', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Fortalezca la seguridad de sus documentos con firmas"
  description: "Con GroupDocs.Signature for Node.js via Java, puede añadir, editar, validar o eliminar sellos y otros tipos de firmas en todos los formatos de documentos populares. La API simplifica el proceso de gestión de firmas para mejorar la integridad y personalización del documento."
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "Características de GroupDocs.Signature"
  features:
    # feature loop
    - title: "Firma de documentos personalizadas"
      content: "Aplique firmas como texto, imágenes, códigos de barras, códigos QR y sellos a cualquier parte de su documento. Esta herramienta también permite la inclusión de metadatos ocultos y certificados digitales para proteger aún más su contenido de modificaciones no autorizadas."

    # feature loop
    - title: "Búsqueda y verificación de firmas"
      content: "Después de que un documento ha sido firmado, use nuestro sistema de verificación para asegurar la integridad de las firmas. Además, nuestra plataforma le permite buscar y recuperar información detallada sobre todas las firmas aplicadas a un documento."

    # feature loop
    - title: "Modificar firmas según sea necesario"
      content: "Ajuste y actualice firmas aplicadas anteriormente según sea necesario. Ya sea cambiando el contenido, color, tamaño o posición de la firma, GroupDocs.Signature for Node.js via Java ofrece opciones completas de personalización."

    # feature loop
    - title: "Eliminar firmas no deseadas"
      content: "Elimine fácilmente cualquier firma innecesaria de sus documentos. Nuestra API admite la eliminación de una amplia gama de tipos de firmas, incluidos sellos y certificados digitales, brindándole flexibilidad total para gestionar sus documentos."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Integrar sellos personalizados en documentos"
      content: |
        Aprenda cómo diseñar y aplicar sellos personalizados que contengan texto esencial a sus documentos.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // Proporcione el documento para sellar
          const signature = new signatureLib.Signature('input.pdf');

          // Configure las opciones de sello con las configuraciones deseadas
          const options = new signatureLib.StampSignOptions();

          // Especifique las dimensiones y la posición del sello en la página
          options.setHeight(200);
          options.setWidth(200);
          options.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          options.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);
          options.setAllPages(true);

          // Incluya líneas circulares exteriores con texto personalizado
          const outerLine1 = new signatureLib.StampLine();
          outerLine1.setText('* The best  choice *');
          outerLine1.setTextRepeatType(signatureLib.StampTextRepeatType.FullTextRepeat);
          const signatureFont1 = new signatureLib.SignatureFont();
          signatureFont1.setSize(12);
          signatureFont1.setFamilyName('Arial');
          outerLine1.setFont(signatureFont1);
          outerLine1.setHeight(30);
          outerLine1.setTextBottomIntent(6);
          outerLine1.setTextColor(signatureLib.Color.WHITE);
          outerLine1.setBackgroundColor(signatureLib.Color.BLUE);
          options.getOuterLines().add(outerLine1);

          // Agregue líneas cuadradas interiores según sea necesario
          const innerLine1 = new signatureLib.StampLine();
          innerLine1.setText('Company #1');
          innerLine1.setTextColor(signatureLib.Color.RED);
          const signFont1 = new signatureLib.SignatureFont();
          signFont1.setSize(20);
          signFont1.setBold(true);
          innerLine1.setFont(signFont1);
          innerLine1.setHeight(40);
          options.getInnerLines().add(innerLine1);
          
          // Guarde el documento sellado
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
            link: "/examples/signature/formats/signature_stamp.pdf"
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
    title: "Explore características clave"
    exclude: "stamp"
    description: "Nuestra solución ofrece una variedad de herramientas para crear, gestionar y eliminar diferentes tipos de firmas, otorgando a los usuarios control total sobre sus flujos de trabajo de documentos."
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
    title: "Aplique firmas de sello en múltiples tipos de archivos"
    exclude: "PDF"
    description: "La API de GroupDocs.Signature admite firmas de sello en más de 60 formatos de archivo, permitiendo a los usuarios colocar sellos personalizados en cualquier página o área, mejorando la accesibilidad y seguridad del documento."
    items: 
          
        # format loop 1
        - name: "Sellar PDF"
          format: "PDF"
          link: "/signature/nodejs-java/stamp/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 2
        - name: "Sellar DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/stamp/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Sellar JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/stamp/jpeg/"
          description: "Imagen JPEG"
          
        # format loop 4
        - name: "Sellar PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/stamp/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 5
        - name: "Sellar XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/stamp/xlsx/"
          description: "Hoja de Cálculo XML Abierto de Microsoft Excel"


          

---