---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "API de firma digital de Java, agregar firma electrónica a PDF Imagen de Excel de Word"
head_description: "API de firma digital Java. Biblioteca de firmas electrónicas para firmar digitalmente PDF, Microsoft Word, hojas de cálculo de Excel, presentaciones de PowerPoint y formatos de documentos de imagen."

############################# Header ############################
title: "API de Java para administrar firmas digitales"
description: "Gestione la firma electrónica de tipos de imágenes, códigos QR, códigos de barras, metadatos, texto y sellos en aplicaciones Java para firmar imágenes y formatos de archivos de documentos digitales."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "/border/groupdocs-signature-java.svg"
        product: "GroupDocs.Signature"
        platform: "Java"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Visión de conjunto"

            # button loop
            - link: "#features"
              text: "Características"

            # button loop
            - link: "#support"
              text: "Support"

            # button loop
            - link: "https://products.groupdocs.app/signature"
              text: "Live Demo"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/signature/java"
              text: "Precios"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Visión de conjunto ############################
overview:
    enable: true
    content: |
      GroupDocs.Signature for Java API lo ayuda a desarrollar aplicaciones Java con funcionalidad de firmas electrónicas para firmar documentos digitales de formatos admitidos sin instalar ningún software externo. Admite la manipulación y gestión de varios tipos de firmas electrónicas, como imagen, código de barras, código QR, sello, texto, óptico y metadatos. Todos sus documentos comerciales electrónicos como Office de Microsoft Word, presentaciones de PowerPoint, hojas de cálculo de Excel, imágenes y archivos PDF se pueden firmar digitalmente personalizando las propiedades de la firma, p. sombra, dimensiones, alineación y más según sus requisitos. La biblioteca de firmas digitales es simple y liviana, y consta de un solo archivo DLL que se puede integrar fácilmente dentro de una aplicación Java nueva o existente.

      A través de GroupDocs.Signature para la API de Java, puede cargar todos los certificados registrados del sistema o ubicar las firmas existentes mediante una búsqueda simple y avanzada. Las opciones para trabajar con documentos protegidos con contraseña, la especificación de propiedades de firma comunes (tamaño de texto, opacidad, rotación, verificación, propiedades de fuente, opciones de color, número de página, ancho, parte superior, izquierda, etc.) y el soporte para implementar diferentes tipos de firmas electrónicas lo convierten en un confiable Solución de gestión de firmas electrónicas para documentos digitales.

      GroupDocs.Signature para Java es compatible con todas las versiones de Java y es compatible con los sistemas operativos populares (Windows, Linux, MacOS) que pueden ejecutar el tiempo de ejecución de Java
    tabs:
      enable: true     
      
      ## TAB ONE ##
      tab_one:
        description: |
          A continuación se muestra una descripción general de GroupDocs.Signature para Java:

        right:
          enable: true
          icon: "fab fa-html5"
          title: "Tipos de firma"
          content: |
            * Firma de texto
            * Firma de imagen
            * Firmas digitales
            * Firma de código QR
            * Firma de código de barras
            * Sello Firma
            * Firma de campo de formulario
      
      ## TAB TWO ##
      tab_two:
        description: |
          La API de firma electrónica de Java admite [formatos de archivo de documentos] (https://docs.groupdocs.com/signature/java/supported-document-formats/) como se indica a continuación.

        left:
          enable: true
          table:
            # table loop
            - title: "oficina de Microsoft"
              content: |
                * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF, TXT
                * **Excel:** XLS, XLSX, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
                * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM

        right:
          enable: true
          table:
            # table loop
            - title: "Images & Otros formatos"
              content: |
                * **Imágenes**: JPG, BMP, PNG, TIFF, GIF, DCM, WEBP
                * **Documento abierto**: ODT, OTT, OTS, ODS, ODP, OTP, ODG
                * **Jpeg2000**: JP2, JPF, JPX, J2K, J2C, JPM
                * **Metarchivos**: EMF, WMF, CMX
                * **Portátil**: PDF
                * **Gráficos vectoriales escalables**: CDR, SVG
                * **Adobe Photoshop**: PSD
                * **Otros**: DJVU

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Signature for Java apoya siguiendo Sistemas operativos, Marcos y administradores de paquetes:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Sistemas operativos"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Marcos compatibles"
              content: |
                * Java 7 (1.7) y superior

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Entornos de desarrollo"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "Herramienta de automatización de compilación"
              content: |
                * Maven

############################# Características ############################
features:
    enable: true
    title: "GroupDocs.Signature for Java Características"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Cree, lea, modifique, oculte y elimine firmas electrónicas de formatos de documentos admitidos"

      # feature loop
      - icon: "fas fa-eye"
        content: "Acceso al documento firmado desde flujo, ruta relativa o ruta absoluta"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Agregue Firma de texto como anotación, pegatina, imagen a archivos PDF y configure estilo y color"

      # feature loop
      - icon: "fas fa-code"
        content: "Firme un documento PDF, un archivo de imagen y obtenga resultados en diferentes formatos de archivo"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Firme imágenes digitalmente con Firma de texto como marca de agua y agregue transparencia, rotación a la firma electrónica"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Buscar certificados y firmar documentos de Microsoft Word, Excel y PDF con certificados digitales"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Firme formatos de documentos de procesamiento de textos con marcas de agua de texto nativo"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Use código QR, código de barras para firmar archivos de Word, diapositivas, celdas, PDF e imágenes"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Configure y aplique Sello Firmas para proteger los formatos de archivo admitidos"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Configurar y asignar Firma de imágenes a documentos, hojas de cálculo, presentaciones, imágenes y archivos PDF"

      # feature loop
      - icon: "fas fa-columns"
        content: "Configure las propiedades de la firma, por ejemplo, apariencia, márgenes, alineación, etc.."

      # feature loop
      - icon: "fas fa-file-word"
        content: "Aplicar firma digital a documento protegido por contraseña"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Realice la verificación de texto de documentos PDF utilizando el controlador de firmas"

      # feature loop
      - icon: "fas fa-print"
        content: "Verificación digital de documentos Word, Cell, PDF con contenedores de certificados .CER y .PFX"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Specify Different Measure Unit Types (e.g. Millimeters, Pixels etc.) for PDF Firma de textos"

      # feature loop
      - icon: "fas fa-lock"
        content: "Obtenga información del documento a través de un archivo o URL: agregue firmas de campo de formulario a documentos PDF"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Agregue objetos de datos personalizados, tarjetas virtuales integradas, correo electrónico, EPC, MeCard u objetos de eventos a QR-Code"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Aplique diferentes estilos de pincel a las firmas, por ejemplo, degradado, radial, sólido y pincel de textura"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Firmar documento ubicado en FTP o Azure Cloud Storage"

      # feature loop
      - icon: "fas fa-heading"
        content: "Establezca la alineación del texto dentro de formas para documentos, diapositivas, imágenes y archivos PDF"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Busque, verifique y firme digitalmente documentos de presentación de PowerPoint"

      # feature loop
      - icon: "fas fa-cube"
        content: "Place Signature using Pixels in Cell Documents & Text Positioning for Sello Firmas"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Agregue firmas de metadatos cifrados mientras trabaja con las opciones de firma y búsqueda"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Incruste objetos personalizados en firmas de metadatos en Word, Excel y presentaciones"

    more_feature:
      # more_feature_loop
      - title: "Configure y aplique fácilmente firmas electrónicas"
        content: |
          GroupDocs.Signature para la API de Java permite configurar y agregar firmas electrónicas a los formatos de documentos admitidos. El siguiente es un ejemplo de código que muestra lo simple que es aplicar una firma de texto a un archivo PDF:
          
          ```java
          Signature signature = new Signature("sample.pdf");

          TextSignOptions options = new TextSignOptions("John Smith");
          // establecer la posición de la firma
          options.setLeft(100);
          options.setTop(100);
          
          // establecer rectángulo de firma
          options.setWidth(100);
          options.setHeight(30);

          // establecer el color del texto y la fuente
          options.setForeColor(Color.RED);
          SignatureFont signatureFont = new SignatureFont();
          signatureFont.setSize(12);
          signatureFont.setFamilyName("Comic Sans MS");
          options.setFont(signatureFont);
          options.setSignatureImplementation(TextSignatureImplementation.Sticker)

          // firmar documento para archivar
          signature.sign("sample_signed.pdf", options);
          ```
      # more_feature_loop
      - title: "Tipos de codificación de código de barras admitidos para la firma electrónica"
        content: |
          Con GroupDocs.Signature para la API de Java, puede aplicar firmas de códigos de barras y códigos QR a los formatos de archivo admitidos. GroupDocs.Signature para Java admite una amplia gama de tipos de codificación de códigos de barras para satisfacer la mayoría de los requisitos. Los tipos de codificación de códigos de barras admitidos incluyen Código 11, Código 128, Código 16K/32, Códigos de barra de datos, Bloque de código GS1, ISBN, ISMN, ISSN, ITF16, Pdf147, EAN8, EAN13, EAN14, UPCA, UPCE, ITF14, Code39 Standard y Código 39 extendido.

          De manera similar, GroupDocs.Signature para la API de Java le permite usar tipos de códigos QR, como QR, Aztec y Data Matrix. Los tipos de codificación de QR-Code admitidos incluyen Aztec, DataMatrix, GS1 DataMatrix y GS1 QR.

      # more_feature_loop
      - title: "Buscar firmas y certificados"
        content: |
          A través de GroupDocs.Signature para la API de Java, puede buscar firmas de código QR y código de barras en cualquier documento, presentación, hoja de cálculo, imagen y archivo PDF, y obtener el resultado de la búsqueda. También puede buscar objetos de datos personalizados de documentos firmados con Firma de código QR, así como buscar VCard estándar y objetos de correo electrónico de documentos firmados con QR-Code. También se admite la verificación del texto cifrado de las firmas de códigos QR, así como la búsqueda de firmas de metadatos en documentos PDF. Aplique criterios de búsqueda adicionales para firmas digitales de documentos de Words & Cells.  

          La opción de búsqueda también está disponible para la firma de metadatos para documentos de Word, diapositivas y hojas de cálculo, mientras que la búsqueda de campos de formulario está disponible para documentos PDF.

      # more_feature_loop
      - title: "Configurar las propiedades de la firma electrónica"
        content: |
          Para mejorar la UX de los usuarios finales, GroupDocs.Signature para la API de Java proporciona muchas propiedades que se pueden configurar con bastante facilidad. Puede configurar las opciones de fuente y color (color de fondo, color de primer plano, negrita, cursiva, subrayado, familia de fuentes, tamaño de fuente, etc.), opciones de fondo y borde (color de fondo, transparencia de fondo, color de borde, estilo de guión de borde, peso de borde, Transparencia de borde, etc.), Márgenes de firma (Izquierdo, Superior, Ancho, Alto, Relleno, etc.) y Configuración Firma de imagen Área y Alineación de firma (Alineación horizontal, Alineación vertical, etc.).

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Signature ofrece API de visualización de documentos para otros entornos de desarrollo populares"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Signature for .NET"
          image: "/border/groupdocs-signature-net.svg"
          product: "GroupDocs.Signature"
          platform: ".NET"
          link: "/signature/net/"

############################# Back to top ###############################
back_to_top:
  enable: true
---