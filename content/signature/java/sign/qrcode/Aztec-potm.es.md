---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Qrcode
codetype: Aztec
fileformat: Potm
productName: Java
lang: es
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Qrcode signature on Potm for Java

############################# Head ############################
head_title: "Firme electrónicamente Potm documento con Aztec Código QR en Java"
head_description: "Cree el código QR Aztec y colóquelo en el archivo Potm usando Java con un fragmento corto de código Java. Utilice la API de firma de documentos de GroupDocs para firmar electrónicamente sus documentos y archivos comerciales con código QR."

############################# Header ############################
title: "Genere la firma del código QR Aztec para el documento Potm en Java"
description: "Firme electrónicamente sus Potm documentos y contratos con Aztec QR Code. Genere la firma del código QR de forma rápida y sencilla."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "Acerca de GroupDocs.Signature for Java API de firmas de código QR"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) es una API madura para crear y generar firmas de código QR para los documentos. Los usuarios pueden generar firmas de código QR proporcionando texto para descargarlo o compartirlo en las redes sociales como imagen. ¡El documento firmado se puede escanear con API o simplemente con la cámara del móvil! Firme electrónicamente sus contratos comerciales y documentos oficiales agregando la firma del código QR y manipúlelo. Cualquier firma de código QR contendrá información personalizada única para identificar al firmante o autorizar el documento. Además, el contenido del código QR se puede cifrar y descifrar con claves personales mediante programación. Eso abre muchas capacidades para compartir datos confidenciales dentro de los documentos públicos. Después de que el usuario que firma puede actualizar, verificar, eliminar, obtener una vista previa o buscar los códigos QR en archivos PDF, documentos de MS Word, libros de trabajo de MS Excel, presentaciones de MS PowerPoint, archivos de Adobe Photoshop y varios formatos de imagen. Los códigos QR se pueden personalizar adicionalmente.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Pasos para firmar Potm con Qrcode en Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) proporciona la capacidad de firmar documentos Potm con Qrcode firmas de forma rápida y sencilla.
        
        * Cree una instancia de la clase Signature que proporcione el archivo Potm que se supone que debe firmar como ruta o flujo de memoria
        * Cree una instancia de la clase SignOptions y configure todos los datos solicitados.
        * Invoque el método Signature.Sign() pasando la salida Potm archivo o flujo de memoria

    title_right: " Requisitos del sistema"
    content_right: |
        GroupDocs.Signature for Java son compatibles con todas las principales plataformas y sistemas operativos. Antes de ejecutar el código a continuación, asegúrese de tener instalados los siguientes requisitos previos en su sistema.

        * Sistemas operativos: Microsoft Windows, Linux, Mac OS
        * Entornos de desarrollo: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Obtén el último GroupDocs.Signature for Java de [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Potm file
        String filePath = "input.potm";
        // Set up output file
        String outputFilePath = "output.potm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(QrCodeTypes.Aztec);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Potm document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Firma de Potm documentos con Qrcode Live Demo"
    content: |
       Firme el archivo Potm con varias firmas ahora mismo visitando el sitio web de [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demostración en línea gratuita esperándote.

              
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Aztec QrCode"
          content: |
            Aztec Code es una simbología matricial bidimensional (2-D) de propósito general que está diseñada para tener mayor precisión que otras simbologías 2-D. Un símbolo de código azteca puede codificar hasta 3832 dígitos numéricos; 3.067 caracteres alfabéticos; o 1.914 bytes de datos.
          characterset: |
             Los 256 caracteres ASCII.
          textcapacity: |
             Hasta 3832 dígitos numéricos o 3067 caracteres alfabéticos o 1914 bytes de datos.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAK0AAACtCAYAAADCr/9DAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAALEoAACxKAXd6dE0AAAp7SURBVHhe7ZJBjuA6DsX6/pf+s+KiAc6D2pFcSUEEuCMsO9Gf/5blY+zSLp9jl3b5HLu0y+fYpV0+xy7t8jl2aZfPsUu7fI5d2uVz7NIun2OXdvkcu7TL59ilXT7HLu3yOXZpl8+xS7t8jl3a5XPs0i6fY5d2+Ry7tMvnuLq0f/78aTdhPb4Jux8mrK+YsL7iTa5Os8c+NWE9vgm7Hyasr5iwvuJNrk6zxz41YT2+CbsfJqyvmLC+4k2uTrPHPjVhPb4Jux8mrK+YsL7iTa5Os8c+NWE9vgm7Hyasr5iwvuJNrk6zxz41YT2+CbsfJqyvmLC+4k2uTrPHPjVhPb4Jux8mrK+YsL7iTV7z9+xD4AQ2BxPWf82E9ZiwHruZ2YgD7LE4gc3BhPVfM2E9JqzHbmY24gB7LE5gczBh/ddMWI8J67GbmY04wB6LE9gcTFj/NRPWY8J67GZmIw6wx+IENgcT1n/NhPWYsB67mdmIA+yxOIHNwYT1XzNhPSasx25mNuIAeyxOYHMwYf3XTFiPCeuxm5mN+D/Yg/AUO+upp9hZFRPW45uw+2E3V19uD8JT7KynnmJnVUxYj2/C7ofdXH25PQhPsbOeeoqdVTFhPb4Jux92c/Xl9iA8xc566il2VsWE9fgm7H7YzdWX24PwFDvrqafYWRUT1uObsPthN1dfbg/CU+ysp55iZ1VMWI9vwu6H3Vx9uT0IT7GznnqKnVUxYT2+CbsfdtN+ol36jSasn3QCm4MJ6yveZJdWsH7SCWwOJqyveJNdWsH6SSewOZiwvuJNdmkF6yedwOZgwvqKN9mlFayfdAKbgwnrK95kl1awftIJbA4mrK94k11awfpJJ7A5mLC+4k3uTjvEPtJTE9Zjwnq8jd0BJ7A52M39r3mAfYinJqzHhPV4G7sDTmBzsJv7X/MA+xBPTViPCevxNnYHnMDmYDf3v+YB9iGemrAeE9bjbewOOIHNwW7uf80D7EM8NWE9JqzH29gdcAKbg93c/5oH2Id4asJ6TFiPt7E74AQ2B7u5/zUPsA/x1IT1mLAeb2N3wAlsDnbTfqJdGhPWY8L6dcaE9djNLu1aNmE9drNLu5ZNWI/d7NKuZRPWYze7tGvZhPXYzS7tWjZhPXazS7uWTViP3fSfGLAH4QQ2B38D9q6nJqzHm+zSfhh711MT1uNNdmk/jL3rqQnr8Sa7tB/G3vXUhPV4k13aD2PvemrCerzJLu2HsXc9NWE93mSX9sPYu56asB5v0j7NHvTUU+wsTFj/Uyasx4T1mLC+YjftJ9qln3qKnYUJ63/KhPWYsB4T1lfspv1Eu/RTT7GzMGH9T5mwHhPWY8L6it20n2iXfuopdhYmrP8pE9ZjwnpMWF+xm/YT7dJPPcXOwoT1P2XCekxYjwnrK3bTfqJd+qmn2FmYsP6nTFiPCesxYX3FbtpPtEs/9RQ7CxPW/5QJ6zFhPSasr9hN/4mH2GMrJqzHhPU4gc3BhPUVE9ZjwnrsZuYvHGCPrZiwHhPW4wQ2BxPWV0xYjwnrsZuZv3CAPbZiwnpMWI8T2BxMWF8xYT0mrMduZv7CAfbYignrMWE9TmBzMGF9xYT1mLAeu5n5CwfYYysmrMeE9TiBzcGE9RUT1mPCeuxm5i8cYI+tmLAeE9bjBDYHE9ZXTFiPCeuxm5m/cIA9tmLCekxYjxPYHExYXzFhPSasx25m/sIB9tiKCesxYT0mrMeE9ZiwvuIENge7mXnBAfbYignrMWE9JqzHhPWYsL7iBDYHu5l5wQH22IoJ6zFhPSasx4T1mLC+4gQ2B7uZecEB9tiKCesxYT0mrMeE9ZiwvuIENge7mXnBAfbYignrMWE9JqzHhPWYsL7iBDYHu5l5wQH22IoJ6zFhPSasx4T1mLC+4gQ2B7uZecEB9tiKCesxYT0mrMeE9ZiwvuIENge7aT/RLo0J6zFhfcWE9TiBzcGE9RUT1mPCeuym/US7NCasx4T1FRPW4wQ2BxPWV0xYjwnrsZv2E+3SmLAeE9ZXTFiPE9gcTFhfMWE9JqzHbtpPtEtjwnpMWF8xYT1OYHMwYX3FhPWYsB67aT/RLo0J6zFhfcWE9TiBzcGE9RUT1mPCeuym/US7NCasx4T1FRPW4wQ2BxPWV0xYjwnrsZv2E+3SmLAeE9ZXTFiPE9gcTFhfMWE9JqzHbtpPtEtPmrAeE9b/lAnrJ30Lu7SC9T9lwvpJ38IurWD9T5mwftK3sEsrWP9TJqyf9C3s0grW/5QJ6yd9C7u0gvU/ZcL6Sd/CLq1g/U+ZsH7St3D1JvYhMGH9U38D9q6KCesxYT12c/Xv2YMwYf1TfwP2rooJ6zFhPXZz9e/ZgzBh/VN/A/auignrMWE9dnP179mDMGH9U38D9q6KCesxYT12c/Xv2YMwYf1TfwP2rooJ6zFhPXZz9e/ZgzBh/VN/A/auignrMWE9dnP179mDMGH9U38D9q6KCesxYT1285q/Z4+tmLB+zSasr9jNLu36lwnrK3azS7v+ZcL6it3s0q5/mbC+Yje7tOtfJqyv2M0u7fqXCesrdrNLu/5lwvqK3VxdWnvQU29jd8CE9RUnsDmYsB5vcnWaPfapt7E7YML6ihPYHExYjze5Os0e+9Tb2B0wYX3FCWwOJqzHm1ydZo996m3sDpiwvuIENgcT1uNNrk6zxz71NnYHTFhfcQKbgwnr8SZXp9ljn3obuwMmrK84gc3BhPV4k6vT7LFPvY3dARPWV5zA5mDCerzJ/b9+gH2kSRPW4yl2VsUJbA6+hV1aMWE9nmJnVZzA5uBb2KUVE9bjKXZWxQlsDr6FXVoxYT2eYmdVnMDm4FvYpRUT1uMpdlbFCWwOvoVdWjFhPZ5iZ1WcwObgW9ilFRPW4yl2VsUJbA6+hfab2GMxYT2eYmdVPMXOqpiwHhPW4wQ2B7tpP9EujQnr8RQ7q+IpdlbFhPWYsB4nsDnYTfuJdmlMWI+n2FkVT7GzKiasx4T1OIHNwW7aT7RLY8J6PMXOqniKnVUxYT0mrMcJbA52036iXRoT1uMpdlbFU+ysignrMWE9TmBzsJv2E+3SmLAeT7GzKp5iZ1VMWI8J63ECm4PdtJ9ol8aE9XiKnVXxFDurYsJ6TFiPE9gc7Kb9RLs0nmJnVXwTdr+KCesrJqzHt9B+E3ssnmJnVXwTdr+KCesrJqzHt9B+E3ssnmJnVXwTdr+KCesrJqzHt9B+E3ssnmJnVXwTdr+KCesrJqzHt9B+E3ssnmJnVXwTdr+KCesrJqzHt9B+E3ssnmJnVXwTdr+KCesrJqzHt9B+E3ssnmJnVXwTdr+KCesrJqzHt9B+E3ssvgm7X8UJbE7F29gd8Ca7tP/oBDan4m3sDniTXdp/dAKbU/E2dge8yS7tPzqBzal4G7sD3mSX9h+dwOZUvI3dAW+yS/uPTmBzKt7G7oA32aX9RyewORVvY3fAm7xrk5alwC7t8jl2aZfPsUu7fI5d2uVz7NIun2OXdvkcu7TL59ilXT7HLu3yOXZpl8+xS7t8jl3a5XPs0i6fY5d2+Ry7tMvn2KVdPscu7fI5dmmXz7FLu3yM//77H+JY77gkOjOBAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Otras firmas Qrcode admitidas para Java"
    content: |
        "También puede firmar Potm con otros tipos de firma. Consulte la lista a continuación."
    format: 
        
       
back_to_top:
    enable: true
---