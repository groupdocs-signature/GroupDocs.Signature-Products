



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:17
draft: false
lang: es
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Añadiendo firmas electrónicas digitales a archivos XLSX con C#"
head_description: "Coloca una firma digital en un archivo XLSX utilizando C# con solo unas pocas líneas de código. Usa GroupDocs.Signature for .NET para firmar numerosos formatos de archivo."

############################# Header ############################
title: "eFirmar XLSX con firmas digitales" 
description: "Protege la integridad de tus documentos comerciales sellándolos con certificados digitales utilizando las robustas características de GroupDocs.Signature for .NET. Ofrecemos soluciones versátiles para marcar y asegurar tus documentos."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Descargar gratis"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "Acerca de GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "Aprende más"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) es una solución de firma sofisticada que facilita una amplia gama de tareas de procesamiento de documentos. Permite incrustar texto, imágenes, certificados digitales y sellos en archivos de más de 60 formatos, incluyendo PDF, MS Office, imágenes, archivos ZIP y otros formatos comerciales esenciales. Además, los documentos firmados pueden ser fácilmente buscados, verificados, modificados o eliminados según sea necesario.

############################# Steps ############################
steps:
    enable: true
    title: "Cómo asegurar XLSX con certificados digitales en C#"
    content: |
      [GroupDocs.Signature](/signature/net/) capacita a los desarrolladores de .NET para proteger documentos XLSX contra alteraciones usando firmas digitales. Aumenta tus aplicaciones comerciales con capacidades robustas de protección de datos.
      
      1. Pasa el documento XLSX al constructor de la clase Signature.
      2. Utiliza un certificado digital y su contraseña para asegurar el documento.
      3. Opcionalmente, añade una representación visual de la firma digital en las páginas del documento.
      4. Firma el documento para asegurarte de que permanezca inalterado.
   
    code:
      platform: "net"
      copy_title: "Copiar"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Firmas de muestra"
      install:
        command: "dotnet add package GroupDocs.Signature"
        copy_tip: "haz clic para copiar"
        copy_done: "copiado"
      links:
        #  loop
        - title: "Más ejemplos"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET/"
        #  loop
        - title: "Documentación"
          link: "https://docs.groupdocs.com/signature/net/"
          
      content: |
        ```csharp {style=abap}
        // Aprovecha Signature para firmar digitalmente el documento
        using (Signature signature = new Signature("input.xlsx"))
        {
            // Proporciona el certificado digital y la contraseña asociada
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                Password = "1234567890",

                // Configura la representación visual si es necesario
                PageNumber = 1,
                Left = 50,
                Top = 50
            };

            // Asegura el documento con el certificado digital
            SignResult result = signature.Sign("output.xlsx", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Mejora o protege el contenido del documento con firmas"
  description: "La biblioteca GroupDocs.Signature for .NET está diseñada para firmar todos los formatos de archivo prevalentes. Agiliza tus procesos comerciales al añadir, modificar, verificar o eliminar fácilmente una variedad de firmas."
  image: "/img/signature/features_digital.webp" # 500x500 px
  image_description: "Características clave de GroupDocs.Signature"
  features:
    # feature loop
    - title: "Incorporar firmas en documentos"
      content: "Incrusta firmas de Texto, Imagen, Código de Barra, Código QR o Sello con precisión en cualquier página de cualquier documento soportado. También puedes añadir o editar metadatos ocultos, como EXIF, en imágenes y la mayoría de los tipos de archivo. Asegura la integridad del contenido de tu documento con firmas digitales."

    # feature loop
    - title: "Buscar y verificar firmas"
      content: "El procesamiento posterior a la firma ofrece numerosas posibilidades. Verifica que tus documentos firmados se hayan procesado correctamente. Para un mayor control, recupera una lista completa de todas las firmas a través de la función de búsqueda."

    # feature loop
    - title: "Modificar firmas"
      content: "La mayoría de los tipos de firma son completamente editables. Tienes la flexibilidad de ajustar texto, reposicionar elementos, cambiar colores, redimensionar y más."

    # feature loop
    - title: "Eliminar firmas redundantes"
      content: "Nuestra solución proporciona operaciones completas CRUD para firmas. Si es necesario, puedes eliminar una variedad de tipos de firma, incluidos los certificados digitales, de tu documento."
      
  code_samples:
    # code sample loop
    - title: "Asegura documentos con firmas digitales"
      content: |
        Descubre cómo prevenir modificaciones en documentos usando firmas digitales.
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        // Proporciona el documento a firmar
        using (Signature signature = new Signature("input.xlsx"))
        {
            // Usa un certificado digital válido con la contraseña correspondiente
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                Password = "1234567890",

                // Especifica cualquier información adicional de texto
                Reason = "Security issue",
                Contact = "John Smith",
                Location = "Office D.W.",

                // Incorpora una imagen y otras opciones para la representación visual
                ImageFilePath = "image.png",
                AllPages = true,
                VerticalAlignment = VerticalAlignment.Center,
                HorizontalAlignment = HorizontalAlignment.Left,
                Width = 60,
                Height = 80,

                Margin = new Padding() {  Bottom = 10, Right = 10 }
            };

            // Guarda el documento asegurado en una ubicación designada
            SignResult result = signature.Sign("output.xlsx", options);
        }
        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "¿Listo para empezar?"
  description: "Prueba las funciones de GroupDocs.Signature de forma gratuita o solicita una licencia"
  items:
    #  loop
    - title: "Descarga de Nuget"
      link: "https://releases.groupdocs.com/signature/net/"
      color: "red"
        #  loop
    - title: "Licenciamiento"
      link: "https://purchase.groupdocs.com/pricing/signature/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Descubre nuestras características destacadas"
    exclude: "digital"
    description: "Ofrecemos una rica variedad de formatos de firma y operaciones potentes."
    items: 
          
        # operation loop 1
        - name: "Firmas electrónicas"
          operation: "esign"
          link: "/signature/net/esign/xlsx/"
          description: "Agrega varios tipos de firmas a formatos de archivo soportados"

        # operation loop 2
        - name: "Agregar texto a documentos"
          operation: "text"
          link: "/signature/net/text/xlsx/"
          description: "Mejora el contenido del documento con firmas de texto personalizables"

        # operation loop 3
        - name: "Firmas de imagen"
          operation: "image"
          link: "/signature/net/image/xlsx/"
          description: "Coloca cualquier imagen en cualquier posición dentro de un documento"

        # operation loop 4
        - name: "Generar códigos de barras"
          operation: "barcode"
          link: "/signature/net/barcode/xlsx/"
          description: "Crear e insertar varios códigos de barras en documentos soportados"

        # operation loop 5
        - name: "Generar códigos QR"
          operation: "qrcode"
          link: "/signature/net/qrcode/xlsx/"
          description: "Generar y utilizar códigos QR para la firma de documentos"
          
        # operation loop 6
        - name: "Certificados digitales"
          operation: "digital"
          link: "/signature/net/digital/xlsx/"
          description: "Asegura negocios y firma documentos con certificados digitales"

        # operation loop 7
        - name: "Firmas de sello"
          operation: "stamp"
          link: "/signature/net/stamp/xlsx/"
          description: "Utiliza el Constructor de Sellos para crear sellos personalizados redondos o cuadrados"
          
        # operation loop 8
        - name: "Buscar firmas"
          operation: "search"
          link: "/signature/net/search/xlsx/"
          description: "Ubica cualquier firma previamente añadida dentro de un documento"
          
        # operation loop 9
        - name: "Verificación de firmas"
          operation: "verify"
          link: "/signature/net/verify/xlsx/"
          description: "Verifica la autenticidad de las firmas después de que se han aplicado"
          
        # operation loop 10
        - name: "Modificar firmas"
          operation: "modify"
          link: "/signature/net/modify/xlsx/"
          description: "Edita fácilmente una variedad de firmas dentro de un documento"
          
        # operation loop 11
        - name: "Eliminar firmas"
          operation: "delete"
          link: "/signature/net/delete/xlsx/"
          description: "Remueve una amplia gama de firmas aplicadas previamente"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Firmar documentos en varios formatos"
    exclude: "XLSX"
    description: "La API .NET te permite procesar más de 60 formatos diferentes. Puedes crear e incrustar diversas firmas en cualquier página, aplicar certificados digitales para la seguridad del contenido y gestionar eficazmente las firmas existentes dentro del documento."
    items: 
          
        # format loop 1
        - name: "Proteger PDF"
          format: "PDF"
          link: "/signature/net/digital/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 2
        - name: "Proteger DOCX"
          format: "DOCX"
          link: "/signature/net/digital/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Proteger PPTX"
          format: "PPTX"
          link: "/signature/net/digital/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 4
        - name: "Proteger XLSX"
          format: "XLSX"
          link: "/signature/net/digital/xlsx/"
          description: "Hoja de Cálculo XML Abierto de Microsoft Excel"


          

---