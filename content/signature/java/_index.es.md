---
############################# Static ############################
layout: "landing"
date: 2024-07-25T14:25:12
draft: false

lang: es
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

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
head_title: "Biblioteca de firmas digitales Java - GroupDocs.Signature"
head_description: "Potencia las aplicaciones Java mediante firmas electrónicas con GroupDocs.Signature. Firme documentos comerciales de forma rápida y sin esfuerzo."

############################# Header ############################
title: "Firmar documentos a través de la API de Java"
description: "Firme documentos e imágenes digitales en cualquier plataforma utilizando nuestras API flexibles y soluciones basadas en aplicaciones para programadores y usuarios finales."
words:
  for: "para"

actions:
  main: "Descarga gratuita de Maven"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-signature/"
  alt: "Licencia"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "¿Listo para comenzar?"
  description: "Pruebe las funciones de GroupDocs.Signature de forma gratuita o solicite una licencia"

release:
  title: "Versión {0} lanzada"
  notes: "Ver qué hay de nuevo"
  downloads: "Descargas"

code:
  title: "Firmar archivos PDF en Java"
  more: "Más ejemplos"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-signature</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Seleccionar documento PDF
    Signature signature = new Signature("sample.pdf");
    
    // Proporcionar texto
    TextSignOptions options = 
        new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // Firmar el documento y guardarlo en un archivo.
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Descripción general de GroupDocs.Signature"
  description: "API para realizar firma de documentos y operaciones relacionadas en aplicaciones Java"
  features:
    # feature loop
    - title: "Documentos comerciales mejorados con firmas digitales en Java"
      content: "Firma rápida y personalizable: GroupDocs.Signature para Java ofrece una amplia gama de opciones de firma digital para archivos PDF, imágenes y documentos de Office. Puede utilizar texto, códigos de barras, códigos QR, certificados digitales, imágenes o metadatos ocultos. El procesamiento de documentos es rápido y eficiente."

    # feature loop
    - title: "Manipular documentos firmados"
      content: "El procesamiento avanzado de documentos implica operaciones potentes en documentos firmados utilizando GroupDocs.Signature para Java. Puede buscar y validar firmas que se hayan agregado a documentos comerciales utilizando varios criterios útiles. Además, podrás acceder a información detallada sobre el documento u obtener imágenes de vista previa de sus páginas."

    # feature loop
    - title: "Variedad de opciones de salida"
      content: "Las sólidas opciones de firma le permiten personalizar la salida de los documentos firmados con GroupDocs.Signature para Java. Puede colocar con precisión cualquier firma en cualquier página del documento y configurar su apariencia de varias maneras. La API de Java permite guardar documentos comerciales firmados en numerosos formatos compatibles y ofrece opciones para protegerlos con contraseñas."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independencia de plataforma"
  description: "GroupDocs.Signature para Java admite los siguientes sistemas operativos, marcos y administradores de paquetes"
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "Formatos de archivo admitidos"
  description: |
    GroupDocs.Signature para Java admite operaciones con los siguientes [formatos de archivo](https://docs.groupdocs.com/signature/java/supported-document-formats/).
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
  title: "Funciones de GroupDocs.Signature"
  description: "Firmar archivos PDF, documentos de Office e imágenes con firmas digitales"

  items:
    # feature loop
    - icon: "sign"
      title: "Agregar firmas"
      content: "Firme un documento utilizando varios tipos de firma admitidos colocando una firma digital con precisión en cualquier posición de cualquier página."

    # feature loop
    - icon: "custom"
      title: "Personalización de resultados"
      content: "Personalice la apariencia de la firma ajustando el color, la fuente, el borde, la rotación y otras características para lograr el resultado deseado."

    # feature loop
    - icon: "password"
      title: "Proteger documentos con contraseña"
      content: "Para muchos tipos de documentos admitidos, puede proteger el documento firmado con una contraseña."

    # feature loop
    - icon: "protect"
      title: "Prevención de cambios no autorizados"
      content: "Proteja los documentos comerciales importantes firmados con un certificado digital contra modificaciones no autorizadas."

    # feature loop
    - icon: "convert"
      title: "Obtención de resultados en los formatos deseados"
      content: "Obtenga fácilmente archivos de resultados firmados en cualquier formato compatible. También puedes convertir documentos de MS Word a PDF sin esfuerzo."

    # feature loop
    - icon: "preview"
      title: "Vista previa del documento"
      content: "Guarde cualquier página de un documento como una imagen para su procesamiento futuro."

    # feature loop
    - icon: "search"
      title: "Buscando firmas"
      content: "Es posible obtener información sobre firmas agregadas previamente en documentos específicos."

    # feature loop
    - icon: "validate"
      title: "Validación de documentos"
      content: "Validar la exactitud de las firmas en cualquier documento firmado."

    # feature loop
    - icon: "update"
      title: "Gestionar firmas"
      content: "Una vez que se coloca una firma en la página de un documento, se puede eliminar, mover o actualizar según sea necesario."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Ejemplos de código"
  description: "Algunos casos de uso de operaciones típicas de GroupDocs.Signature para Java"
  items:
    # code sample loop
    - title: "Mejore el documento PDF con código QR"
      content: |
        Puede resultar valioso mejorar los procesos comerciales agregando [códigos QR](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) a páginas específicas de documentos PDF. Hay un ejemplo de cómo agregar un código QR usando GroupDocs.Signature para Java.
        {{< landing/code title="Mejore el documento PDF con código QR">}}
        ```java {style=abap}
        // Cargar el documento para firmar
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Crea opciones de códigos QR con texto predefinido
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Configurar el tipo de codificación del código QR y su posición en la página
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // Firme el documento y guárdelo como archivo de resultados.
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Utilice firma digital para proteger un DOCX"
      content: |
        Puede [Proteger un documento](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) utilizando firmas personales o corporativas almacenadas como certificados digitales. Los documentos protegidos con certificado no pueden modificarse sin invalidar la firma.
        {{< landing/code title="Utilice firma digital para proteger un DOCX">}}
        ```java {style=abap}   
        // Cargar el documento a firmar digitalmente
        Signature signature = new Signature("file_to_sign.docx");
        
        // Especifique las opciones de firma digital y proporcione la ruta al archivo del certificado.
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // Establecer la contraseña del certificado
        options.setPassword("1234567890");

        // Firme el documento y guárdelo en la ruta deseada.
        signature.sign("digitally_signed.docx", options);
        ```
        {{< /landing/code >}}

---