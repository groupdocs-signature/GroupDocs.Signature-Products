---
############################# Static ############################
layout: "family"
date:  2024-09-26T13:44:48
draft: false

product: "Signature"
product_tag: "signature"

lang: es

############################# Head ############################
head_title: "Aplicaciones de firma digital C# .NET, Java, Node.js"
head_description: "Integre firmas electrónicas en aplicaciones .NET, Java o Node.js con GroupDocs.Signature. Firme formatos de documentos comerciales populares."

############################# Header ############################
title: "Solución de firma electrónica de documentos"
description:  |
  Firme documentos e imágenes digitales en cualquier plataforma utilizando nuestras API flexibles y soluciones basadas en aplicaciones para programadores y usuarios finales.

  Busque y modifique firmas agregadas previamente utilizando métodos avanzados.

  Proteja los documentos de cambios con certificados digitales y controle los metadatos ocultos.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "Elige tu plataforma"
  title: "Independencia de plataforma"
  description: "La biblioteca GroupDocs.Signature admite los siguientes sistemas operativos y marcos:"
  details_link_title: "Aprende más"

  items:
    # items loop
    - title: ".NET"
      description: GroupDocs.Signature .NET 
      color: "blue"
      tag: "net"
      link: "/signature/net/"
      features_link: "https://docs.groupdocs.com/signature/net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    .NET Framework 4.6.2 or higher <br> .NET Core 3.0 or higher <br> .NET 6.0 or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS <br> Microsoft Azure
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio <br> JetBrains Rider <br> Microsoft Visual Code
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats
      

    # items loop
    - title: "Java"
      description: GroupDocs.Signature Java
      color: "red"
      tag: "java"
      link: "/signature/java/"
      features_link: "https://docs.groupdocs.com/signature/java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Java 8 or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    IntelliJ IDEA <br> Eclipse <br> NetBeans
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats

    # items loop
    - title: "Node.js"
      description: GroupDocs.Signature Node.js
      color: "green"
      tag: "nodejs-java"
      link: "/signature/nodejs-java/"
      features_link: "https://docs.groupdocs.com/signature/nodejs-java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Node.js 16+ and J2SE 8.0 (1.8)+
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Atom <br> Visual Studio Code <br> Cualquier otro editor de texto
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats

    # items loop
    - title: "Python"
      description: GroupDocs.Signature Python
      color: "yellow"
      tag: "python-net"
      link: "/signature/python-net/"
      features_link: "https://docs.groupdocs.com/signature/python-net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Python 3.9+ and .Net 6+
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    IDLE <br> PyCharm <br> Visual Studio Code
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats

############################# Features ###############################
features:
  enable: true
  title: "Funciones clave de GroupDocs.Signature"
  description: "Nuestra solución está diseñada para agregar varios tipos de firmas a formatos de archivos y documentos populares. Enriquezca sus procesos de negocio fácilmente."

  items:
    # items loop
    - icon: "additional"
      title: "Enriquece tus datos con firmas"
      content: "Agregue texto, imágenes, marcas de agua, etc. a sus documentos comerciales."

    # items loop
    - icon: "protect"
      title: "Proteger el contenido de los documentos"
      content: "Prohibir cambios de documento sellándolo con un certificado digital."

    # items loop
    - icon: "search"
      title: "Agregue datos ocultos y códigos de barras"
      content: "Utilice metadatos para almacenar información invisible o coloque códigos de barras personalizados en las páginas."

    # items loop
    - icon: "manipulate"
      title: "Manipular firmas"
      content: "Busque, actualice o elimine todas las firmas que se hayan agregado anteriormente."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Proteja sus archivos usando firmas"
  description: "Ejemplos de código GroupDocs.Signature"
  items:
    # code sample loop
    - title: "Generar y agregar código QR"
      content: |
       GroupDocs.Signature nos permite generar y agregar códigos QR a documentos con formatos compatibles. Proporcione la ruta a un documento que debe firmarse y configure el texto deseado y las opciones visuales del código QR. Puede colocar la imagen del código QR generada en cualquier área de cualquier página del documento.
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // Especificar el documento para firmar.
            using (Signature signature = new Signature("source.docx"))
            {
                // Crear opciones de firma de código QR
                QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith")
                {
                    // Establecer opciones de código QR
                    EncodeType = QrCodeTypes.QR,
                    Left = 50,
                    Top = 150,
                };

                // Firmar y guardar el archivo procesado
                SignResult result = signature.Sign("result.docx", options);
            }
            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // Especificar el documento para firmar.
            Signature signature = new Signature("source.docx");

            // Crear opciones de firma de código QR
            QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith");

            // Establecer opciones de código QR
            options.setEncodeType(QrCodeTypes.QR);
            options.setLeft(50);
            options.setTop(100);

            // Firmar y guardar el archivo procesado
            signature.sign("result.docx", options);
            ```
        - language: "TypeScript"
          color: "green"
          content: |
            ```javascript {style=abap}  
            const signatureLib = require('@groupdocs/groupdocs.signature')

            // Especificar el documento para firmar.
            const signature = new signatureLib.Signature('source.docx');

            // Crear opciones de firma de código QR
            const options = new signatureLib.QrCodeSignOptions('JohnSmith');

            // Establecer opciones de código QR
            options.setEncodeType(signatureLib.QrCodeTypes.QR);
            options.setLeft(50);
            options.setTop(100);

            // Firmar y guardar el archivo procesado
            signature.sign('result.docx', options);
            ```
        - language: "Python"
          color: "yellow"
          content: |
            ```python {style=abap}  
            import groupdocs.signature as sg

            def run():

                # Especificar el documento para firmar.
                with sg.Signature('source.docx') as signature:

                    # Crear opciones de firma de código QR
                    options = sg.QrCodeSignOptions('JohnSmith')

                    # Establecer opciones de código QR
                    options.setEncodeType(sg.QrCodeTypes.QR)
                    options.setLeft(50)
                    options.setTop(100)

                    # Firmar y guardar el archivo procesado
                    signature.sign('result.docx', options)
            ```

############################# Supported Formats ###############################
formats:
  enable: true
  title: "Se admiten más de 60 formatos de archivo"
  description: "GroupDocs.Signature admite casi todos los formatos de archivos populares"

############################# Metrics ###############################
metrics:
  enable: true
  title: "Datos estadísticos de nuestra biblioteca"
  description: "Inspeccione métricas clave de productos, revelando información sobre nuestros logros, impacto y crecimiento"

  items:
    # items loop
    - number: "50+"
      title: "Formatos soportados"
      content: "Firma de más de 60 de los formatos de archivos comerciales más populares."

    # items loop
    - number: "500k"
      title: "Descargas NuGet"
      content: "GroupDocs.Signature para .NET es una biblioteca popular con más de 550.000 descargas en NuGet."

    # items loop
    - number: "15k"
      title: "Descargas de Maven"
      content: "Los desarrolladores de Java han descargado GroupDocs.Signature en Maven más de 15.000 veces."

    # items loop
    - number: "140+"
      title: "Clientes felices"
      content: "Los desarrolladores individuales y las principales empresas de todo el mundo utilizan nuestros productos para crear soluciones innovadoras."


############################# Customers ###############################
customers:
  enable: true
  title: "Nuestros clientes felices"
  description: "Las bibliotecas de GroupDocs son utilizadas por marcas distinguidas y reconocidas a nivel mundial en todo el mundo"

  items:
    # items loop
    - title: "BenQ Corporation"
      logo: "benq"
      
    # items loop
    - title: "Nasdaq Stock Market"
      logo: "nasdaq"
      
    # items loop
    - title: "AT&T Inc."
      logo: "att"
      
    # items loop
    - title: "Customer logo AstraZeneca"
      logo: "astrazeneca"
      
    # items loop
    - title: "Central Bank of Argentina"
      logo: "argentinacentralbank"
      
    # items loop
    - title: "Roche Holding AG"
      logo: "roche"
      
    # items loop
    - title: "Capita"
      logo: "capita"
      
    # items loop
    - title: "Axa S.A."
      logo: "axa"
      
    # items loop
    - title: "Instructure Inc."
      logo: "instructure"
      
    # items loop
    - title: "Wipro"
      logo: "wipro"


############################# Actions ###############################
actions:
  enable: true
  title: "¿Listo para comenzar?"
  description: "Pruebe las funciones de GroupDocs.Signature gratis en su plataforma"

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/signature/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/signature/java/"

    # items loop
    - title: "Node.js"
      color: "green"
      link: "/signature/nodejs-java/"      

############################# FAQ ###############################
faq:
  enable: true
  title: "Preguntas frecuentes"
  description: "Explore nuestras preguntas frecuentes"

  items:
    # items loop
    - question: "¿GroupDocs.Signature necesita alguna biblioteca externa para la firma de documentos?"
      answer: "No, GroupDocs.Signature funciona de forma independiente. No existen dependencias de terceros como Adobe Acrobat, Microsoft Office, etc."

    # items loop
    - question: "¿Es posible probar las funciones de GroupDocs.Signature antes de comprar?"
      answer: "¡Absolutamente! GroupDocs.Signature ofrece una prueba gratuita. Instálalo y explora sus características. Tenga en cuenta que las versiones de prueba agregan 'insignias de prueba' a sus documentos y solo procesan las primeras 3 páginas. Para disfrutar de una experiencia completa, obtenga una licencia temporal gratuita de 30 días para acceder a todas las funciones. Consulte los detalles en [licencia temporal](https://purchase.groupdocs.com/temporary-license/)."

    # items loop
    - question: "¿Qué tipos de licencia se proporcionan?"
      answer: "¿Busca una licencia de GroupDocs.Signature? Ofrecemos varias opciones adaptadas a sus necesidades. Elija según el tamaño del equipo, las ubicaciones de implementación (oficina única o lugares de trabajo remotos) y si la distribución al cliente final requiere compartir el SDK/API con los clientes. Alternativamente, opte por una licencia de uso mensual con planes medidos: pague solo por lo que use. Descubra la mejor opción para usted en [precios](https://purchase.groupdocs.com/pricing/signature/net/)."

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "GroupDocs.Signature API de código bajo"
  description: "Firme archivos usando su aplicación a través de nuestra API REST basada en la nube."
  
  items:
    # items loop
    - title: "GroupDocs.Signature Cloud for cURL"
      content: "Utilice la API RESTful de cURL para poner firmas en PDF, Word, Excel, PowerPoint, JPEG y muchos otros formatos de archivo."
      icon: "groupdocs_signature-for-curl"
      link: "https://products.groupdocs.cloud/signature/curl"

    # items loop
    - title: "GroupDocs.Signature Cloud for .NET"
      content: "Enriquezca sus aplicaciones .NET con la firma de documentos a través de Cloud SDK. Proteja los documentos comerciales a su manera."
      icon: "groupdocs_signature-for-net"
      link: "https://products.groupdocs.cloud/signature/net"

    # items loop
    - title: "GroupDocs.Signature Cloud for Java"
      content: "GroupDocs.Signature SDK otorga acceso a varias posibilidades para que sus aplicaciones Java firmen cualquier archivo."
      icon: "groupdocs_signature-for-java"
      link: "https://products.groupdocs.cloud/signature/java"

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Signature aplicaciones web"
  description: "GroupDocs.Signature presenta una aplicación web gratuita donde puedes firmar documentos. Se pueden firmar más de 60 formatos de archivos populares a través de su navegador favorito GRATIS."

  items:
    # items loop
    - title: "GroupDocs.Signature Total"
      content: "Herramienta online para poner firmas en documentos desde cualquier dispositivo."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/signature/total"

    # items loop
    - title: "GroupDocs.Signature DOCX"
      content: "Firme MS Word DOCX en línea."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/signature/docx"

    # items loop
    - title: "GroupDocs.Signature PDF"
      content: "Proteja documentos PDF en línea."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/signature/pdf"


      


---