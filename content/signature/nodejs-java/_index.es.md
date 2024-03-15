---
############################# Static ############################
layout: "landing"
date: 2024-03-15T20:32:51
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Node.js
lang: es
#productCode: nodejs-java
#otherformats: 
#breadcrumb: Put  signature on  for JavaScript
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: "API de firma digital de Node.js - GroupDocs.Signature"
head_description: "Integre firmas electrónicas seguras en aplicaciones Node.js con GroupDocs.Signature. Optimice los flujos de trabajo de firma de documentos de forma fácil y eficiente."

############################# Header ############################
title: "Firmar documentos<br>con la API de Node.js"
description: "Firme documentos e imágenes digitales en cualquier plataforma utilizando nuestras API flexibles y soluciones basadas en aplicaciones para programadores y usuarios finales."
words:
  for: "para"

actions:
  main: "Descargar desde NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "Licencia"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "¿Listo para comenzar?"
  description: "Pruebe las funciones de GroupDocs.Signature de forma gratuita o solicite una licencia"

release:
  title: "Versión {0} lanzada"
  notes: "Ver qué hay de nuevo"
  downloads: "Descargas"

code:
  title: "Firmar archivos PDF con Node.js"
  more: "Más ejemplos"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.signature"
  content: |
    ```javascript {style=abap}   
    // Seleccionar documento PDF
    let signature = new Signature("sample.pdf");
    
    // Proporcionar texto
    let options = new TextSignOptions("John Smith");
    
    // Establecer color
    options.ForeColor = Color.Red;
    
    // Firmar el documento y guardarlo en un archivo.
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Descripción general de GroupDocs.Signature"
  description: "Biblioteca de firma de documentos lista para ser utilizada en aplicaciones Node.js"
  features:
    # feature loop
    - title: "Solución de firmas digitales para documentos comerciales con Node.js"
      content: "GroupDocs.Signature for Node.js via Java ofrece un conjunto completo de opciones de firma digital para PDF, documentos de Office e imágenes. Se encuentran disponibles textos, códigos de barras, imágenes, certificados digitales y metadatos. El procesamiento de documentos optimizado garantiza la eficiencia."

    # feature loop
    - title: "Manipulación avanzada de documentos firmados"
      content: "GroupDocs.Signature le permite procesar documentos firmados. Busque y valide firmas utilizando diversos criterios. Además, extraiga información detallada del documento o genere imágenes de vista previa de las páginas."

    # feature loop
    - title: "Diversos formatos de salida"
      content: "Nuestra solución proporciona un amplio control sobre el formato de salida de los documentos firmados. Coloque con precisión las firmas en cualquier página y personalice su apariencia. Guarde documentos firmados en numerosos formatos compatibles y, opcionalmente, protéjalos con contraseñas."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independencia de plataforma"
  description: "GroupDocs.Signature for Node.js via Java realiza el procesamiento de documentos con varios sistemas operativos"
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "Formatos de archivo admitidos"
  description: |
    GroupDocs.Signature for Node.js via Java facilita las operaciones para los [formatos de archivo populares](https://docs.groupdocs.com/signature/java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Formatos de Microsoft Office
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Imágenes y otros formatos
        * **Portátil:** PDF
        * **Imágenes:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Otros formatos de oficina:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Otros formatos
        * **Web:** HTML, MHTML
        * **Archivo:** ZIP, TAR, 7Z
        * **Certificados:** PFX

############################# Features ############################
features:
  enable: true
  title: "Características de GroupDocs.Signature"
  description: "Firme archivos PDF, documentos de Office e imágenes con firmas digitales"

  items:
    # feature loop
    - icon: "sign"
      title: "Firmas comerciales"
      content: "Emplee varios tipos de firma para firmar documentos. Coloque firmas digitales con precisión en cualquier ubicación de la página."

    # feature loop
    - icon: "custom"
      title: "Personalización de la apariencia de la firma"
      content: "Adapte los aspectos visuales de las firmas ajustando el color, la fuente, los bordes, la rotación y más para lograr el resultado deseado."

    # feature loop
    - icon: "password"
      title: "Documentos protegidos con contraseña"
      content: "Para muchos formatos de documentos admitidos, proteja los documentos firmados con una contraseña para mayor seguridad."

    # feature loop
    - icon: "protect"
      title: "Prevención de modificaciones no autorizadas"
      content: "Proteja los documentos comerciales cruciales firmados con certificados digitales contra modificaciones no autorizadas."

    # feature loop
    - icon: "convert"
      title: "Formatos de salida deseados"
      content: "Obtenga documentos firmados sin esfuerzo en cualquier formato compatible. Convierta documentos de MS Word a formato PDF con facilidad."

    # feature loop
    - icon: "preview"
      title: "Vista previa de documentos"
      content: "Guarde páginas de documentos individuales como imágenes para necesidades futuras."

    # feature loop
    - icon: "search"
      title: "Búsqueda de firma"
      content: "Recupere información sobre firmas agregadas previamente en sus documentos."

    # feature loop
    - icon: "validate"
      title: "Validación de documentos"
      content: "Verificar la autenticidad de las firmas presentadas en cualquier documento."

    # feature loop
    - icon: "update"
      title: "Gestión de firmas"
      content: "Elimine, reubique o modifique las firmas colocadas en cualquier página del documento."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Ejemplos de código"
  description: "Ejemplos ilustrativos que muestran operaciones típicas de GroupDocs.Signature for Node.js via Java"
  items:
    # code sample loop
    - title: "Marcar PDF con códigos QR"
      content: |
        La incorporación de [códigos de barras](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) en páginas de documentos PDF específicas puede optimizar los procesos comerciales. Esta sección proporciona un ejemplo de cómo agregar un código QR usando GroupDocs.Signature for Node.js via Java.
        {{< landing/code title="Cómo poner código QR a PDF.">}}
        ```javascript {style=abap}
        // Cargar el documento para firmar
        let signature = new Signature("file_to_sign.pdf");
        
        // Crea opciones de códigos QR con texto predefinido
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Configurar el tipo de codificación del código QR y su posición en la página
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // Firme el documento y guárdelo como archivo de resultados.
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Proteger un DOCX con una firma digital"
      content: |
        [Protege tus Documentos](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) mediante firmas basadas en certificados digitales. La firma digital protege sus documentos comerciales contra cambios de contenido.
        {{< landing/code title="A continuación se explica cómo garantizar la integridad del documento.">}}
        ```javascript {style=abap}   
        // Cargar el documento a firmar digitalmente
        let signature = new Signature("file_to_sign.docx");
        
        // Especifique las opciones de firma digital y proporcione la ruta al archivo del certificado.
        let options = new DigitalSignOptions("certificate.pfx");

        // Establecer la contraseña del certificado
        options.Password = "1234567890";

        // Firme el documento y guárdelo en la ruta deseada.
        signature.Sign("digitally_signed.docx", options);

        ```
        {{< /landing/code >}}

---
