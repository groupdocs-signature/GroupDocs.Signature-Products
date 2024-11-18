



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:59
draft: false
lang: es
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Agregar firmas electrónicas digitales a archivos XLSX con JavaScript"
head_description: "Coloca una firma digital en un archivo XLSX usando JavaScript con solo unas pocas líneas de código. Usa GroupDocs.Signature for Node.js via Java para firmar numerosos formatos de archivo."

############################# Header ############################
title: "Protege XLSX con certificados digitales" 
description: "Asegura la seguridad de tus documentos empresariales al incrustar certificados digitales utilizando las avanzadas capacidades de GroupDocs.Signature for Node.js via Java. Ofrecemos opciones flexibles para proteger y autenticar tus documentos."
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
    title: "Acerca de GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "Aprende más"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) es una solución integral de firma diseñada para manejar una variedad de necesidades de procesamiento de documentos. Te permite incorporar texto, imágenes, certificados digitales y sellos en más de 60 formatos de archivo diferentes, incluidos PDF, MS Office, imágenes y archivos ZIP. Además, los documentos firmados pueden ser buscados, verificados, editados o eliminados fácilmente cuando sea necesario.

############################# Steps ############################
steps:
    enable: true
    title: "Guías para asegurar XLSX con certificados digitales en JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) permite a los desarrolladores de Node.js via Java proteger documentos XLSX de modificaciones mediante la utilización de firmas digitales. Mejora tus aplicaciones empresariales con sólidos recursos de seguridad de datos.
      
      1. Pasa el documento XLSX al constructor de la clase Signature.
      2. Aplica un certificado digital y su correspondiente contraseña para asegurar el documento.
      3. Opcionalmente, añade una representación visual de la firma digital en las páginas del documento.
      4. Firma el documento para evitar cualquier alteración futura.
   
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

        // Utiliza Signature para aplicar una firma digital al documento
        const signature = new signatureLib.Signature('input.xlsx');

        // Proporciona el certificado digital y la contraseña requeridos
        const options = new signatureLib.DigitalSignOptions('certificate.pfx');
        options.setPassword('1234567890');

        // Configura los ajustes de la firma visual si es necesario
        options.setPageNumber(1);
        options.setLeft(100);
        options.setTop(100);
        
        // Cifra el documento usando el certificado digital
        const result = signature.sign('output.xlsx', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Optimiza o asegura el contenido del documento con firmas"
  description: "GroupDocs.Signature for Node.js via Java está diseñado para firmar todos los principales formatos de archivo, ofreciéndote la capacidad de agregar, ajustar, verificar o eliminar varios tipos de firmas sin complicaciones."
  image: "/img/signature/features_digital.webp" # 500x500 px
  image_description: "Características clave de GroupDocs.Signature"
  features:
    # feature loop
    - title: "Agrega firmas a tus documentos"
      content: "Coloca fácilmente firmas de Texto, Imagen, Código de Barras, QR-Code o Sello en cualquier página de los documentos compatibles. También puedes insertar o editar metadatos ocultos, como EXIF en imágenes. Protege el contenido de tu documento de alteraciones no autorizadas con certificados digitales."

    # feature loop
    - title: "Localiza y verifica firmas"
      content: "Después de la firma, tu documento puede someterse a múltiples verificaciones. Confirma la integridad del contenido firmado o realiza una búsqueda detallada para listar todas las firmas existentes."

    # feature loop
    - title: "Revisa firmas existentes"
      content: "La mayoría de los tipos de firma permiten ediciones posteriores a la creación. Puedes modificar fácilmente el texto, reposicionar elementos, ajustar colores, redimensionar y hacer otros cambios necesarios."

    # feature loop
    - title: "Elimina firmas innecesarias"
      content: "Nuestra solución permite operaciones CRUD completas para firmas. Si es necesario, puedes eliminar varios tipos de firma, incluidos certificados digitales, de tu documento."
      
  code_samples:
    # code sample loop
    - title: "Proteger documentos con firmas digitales"
      content: |
        Aprende cómo bloquear un documento contra cambios utilizando firmas digitales.
        {{< landing/code title="JavaScript">}}
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')
        
        // Proporciona el documento que requiere firma
        const signature = new signatureLib.Signature('input.xlsx');

        // Utiliza un certificado digital apropiado y su contraseña
        const options = new signatureLib.DigitalSignOptions('certificate.pfx');
        options.setPassword('1234567890');

        // Incluye cualquier información textual adicional
        options.setReason('Security issue');
        options.setContact('John Smith');
        options.setLocation('Office D.W.');

        // Añade elementos visuales como imágenes para la representación de la firma
        options.setImageFilePath('image.png');
        options.setAllPages(true);
        options.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
        options.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);
        options.setWidth(80);
        options.setHeight(60);

        const padding = new signatureLib.Padding();
        padding.setBottom(10);
        padding.setRight(10);
        options.setMargin(padding);
        
        // Guarda el documento asegurado digitalmente en una ubicación específica
        const result = signature.sign('output.xlsx', options);
        ```
        {{< /landing/code >}}


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
    title: "Conoce nuestras funciones principales"
    exclude: "digital"
    description: "Nos enorgullece ofrecer un conjunto completo de opciones y funcionalidades de firma."
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
    title: "Firma documentos en múltiples formatos"
    exclude: "XLSX"
    description: "La API Node.js via Java admite más de 60 formatos, lo que te permite aplicar una variedad de firmas en cualquier página, hacer cumplir la seguridad del contenido con certificados digitales y gestionar eficazmente las firmas dentro del documento."
    items: 
          
        # format loop 1
        - name: "Proteger PDF"
          format: "PDF"
          link: "/signature/nodejs-java/digital/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 2
        - name: "Proteger DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/digital/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Proteger PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/digital/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 4
        - name: "Proteger XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/digital/xlsx/"
          description: "Hoja de Cálculo XML Abierto de Microsoft Excel"


          

---