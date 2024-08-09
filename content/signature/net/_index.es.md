---
############################# Static ############################
layout: "landing"
date: 2024-07-25T14:25:12
draft: false

lang: es
product: "Signature"
product_tag: "signature"
platform: "Net"
platform_tag: "net"

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
head_title: "API de firmas digitales C# .NET - GroupDocs.Signature"
head_description: "Integre el procesamiento de firmas digitales en sus aplicaciones .NET utilizando GroupDocs.Signature. Proteja sus archivos con firmas de forma rápida y eficiente."

############################# Header ############################
title: "Firmar documentos a través de la API .NET"
description: "Firme documentos e imágenes digitales en cualquier plataforma utilizando nuestras API flexibles y soluciones basadas en aplicaciones para programadores y usuarios finales."
words:
  for: "para"

actions:
  main: "Descarga gratuita de NuGet"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "Licencia"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net/"
  title: "¿Listo para comenzar?"
  description: "Pruebe las funciones de GroupDocs.Signature de forma gratuita o solicite una licencia"

release:
  title: "Versión {0} lanzada"
  notes: "Ver qué hay de nuevo"
  downloads: "Descargas"

code:
  title: "Firmar archivos PDF en C#"
  more: "Más ejemplos"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET/"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // Seleccionar documento PDF
    using (Signature signature = new Signature("sample.pdf"))
    {
        // Proporcionar texto
        var options = new TextSignOptions("John Smith")
        {
            // Establecer color
            ForeColor = Color.Red
        };
        // Firmar el documento y guardarlo en un archivo.
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Descripción general de GroupDocs.Signature"
  description: "API para realizar firma de documentos y operaciones relacionadas en aplicaciones .NET"
  features:
    # feature loop
    - title: "Agregar firmas a documentos comerciales en C#"
      content: "Firma de documentos: con GroupDocs.Signature para .NET, puede agregar varios tipos de firmas, como texto, imágenes, códigos de barras y certificados digitales, a documentos PDF y Office. Esta API le permite firmar sus documentos con casi cualquier tipo de datos, incluidos los metadatos ocultos."

    # feature loop
    - title: "Procesamiento de documentos firmados"
      content: "Procesamiento adicional: puede realizar operaciones potentes en documentos firmados utilizando GroupDocs.Signature. Esto incluye buscar firmas existentes en documentos comerciales y verificarlas utilizando criterios específicos. Además, puede recuperar información del documento y obtener una vista previa de las páginas a través de esta API .NET."

    # feature loop
    - title: "Personalización de resultados"
      content: "GroupDocs.Signature para .NET ofrece amplias opciones de personalización. Puede colocar las firmas con precisión en cualquier lugar de la página de un documento y ajustar su apariencia mediante una variedad de configuraciones. Además, esta API permite guardar documentos procesados ​​en una amplia gama de formatos compatibles."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independencia de plataforma"
  description: "GroupDocs.Signature para .NET admite los siguientes sistemas operativos, marcos y administradores de paquetes"
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
    GroupDocs.Signature para .NET admite operaciones con los siguientes [formatos de archivo](https://docs.groupdocs.com/signature/net/supported-document-formats/).
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
  description: "Firmar archivos PDF, documentos de Office e imágenes de forma rápida y precisa"

  items:
    # feature loop
    - icon: "sign"
      title: "Firma de documentos"
      content: "Agregue uno o varios tipos de firmas compatibles con precisión en cualquier posición especificada de los documentos comerciales."

    # feature loop
    - icon: "custom"
      title: "Personalizar firmas"
      content: "Utilice funciones como color, fuente, borde, rotación, etc., para configurar la apariencia de las firmas."

    # feature loop
    - icon: "password"
      title: "Protección de documentos con contraseña"
      content: "Proteja ciertos tipos de documentos estableciendo una contraseña después de firmar."

    # feature loop
    - icon: "protect"
      title: "Protección contra cambios"
      content: "Evite cambios en documentos comerciales importantes después de agregar una firma con un certificado digital."

    # feature loop
    - icon: "convert"
      title: "Convertir archivos firmados a otros formatos"
      content: "Convierta archivos firmados a los formatos deseados, como guardar un documento de Word como PDF."

    # feature loop
    - icon: "preview"
      title: "Extraer vistas previas de páginas"
      content: "Extraiga páginas de documentos firmados como imágenes individuales para su procesamiento futuro."

    # feature loop
    - icon: "search"
      title: "Búsqueda de firmas en documentos."
      content: "Recupera información sobre firmas agregadas previamente en documentos específicos."

    # feature loop
    - icon: "validate"
      title: "Validar documentos firmados"
      content: "Verifique la firma adecuada de documentos utilizando funciones de validación."

    # feature loop
    - icon: "update"
      title: "Actualizar o eliminar firmas"
      content: "Reposicione fácilmente firmas específicas en una página, modifique su texto o elimínelas sin ningún problema."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Ejemplos de código"
  description: "Algunos casos de uso de operaciones típicas de GroupDocs.Signature para .NET"
  items:
    # code sample loop
    - title: "Agregar código QR a PDF"
      content: |
        Agregar [códigos QR](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) a páginas específicas de documentos PDF puede mejorar los procesos comerciales. A continuación se muestra un ejemplo de cómo agregar un código QR usando GroupDocs.Signature.
        {{< landing/code title="Cómo poner código QR a PDF.">}}
        ```csharp {style=abap}
        // Cargar el documento para firmar
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Crea opciones de códigos QR con texto predefinido
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // Configurar el tipo de codificación del código QR y su posición en la página
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // Firme el documento y guárdelo como archivo de resultados.
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Proteger un documento DOCX mediante un certificado digital"
      content: |
        Puede [Proteger un documento](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/) utilizando firmas personales o corporativas almacenadas como certificados digitales. Dichos documentos protegidos no podrán modificarse sin invalidar la firma.
        {{< landing/code title="A continuación se explica cómo garantizar la integridad del documento.">}}
        ```csharp {style=abap}   
        // Cargar el documento a firmar digitalmente
        using (Signature signature = new Signature("file_to_sign.docx"))
        {
            // Especifique las opciones de firma digital y proporcione la ruta al archivo del certificado.
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // Establecer la contraseña del certificado
                Password = "1234567890"
            };
            // Firme el documento y guárdelo en la ruta deseada.
            signature.Sign("digitally_signed.docx", options);
        }
        ```
        {{< /landing/code >}}

---