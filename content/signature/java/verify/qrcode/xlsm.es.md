---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Qrcode
fileformat: Xlsm
productName: Java
lang: es
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Qrcode signature on Xlsm for Java

############################# Head ############################
head_title: "Verificación de Qrcode firmas para Xlsm archivos a través de Java"
head_description: "Use solo unas pocas líneas de código Java para verificar los documentos Xlsm y sus firmas Qrcode."

############################# Header ############################
title: "Qrcode verificación de firmas para Xlsm archivos"
description: "La API para Java brinda la oportunidad de verificar Qrcode firmas en Xlsm documentos. La verificación de las firmas electrónicas dentro de sus documentos Xlsm se puede realizar rápida y fácilmente."
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
    title: "Descubra las nuevas funciones de la API de GroupDocs.Signature for Java"
    content: |
        La API de [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) proporciona una amplia gama de formas de procesar numerosos formatos de documentos mediante el uso de firmas electrónicas. Se admiten muchos tipos de firmas digitales como textos, imágenes, certificados digitales, códigos de barras, códigos QR, sellos o metadatos. Los clientes pueden agregar, eliminar, editar, validar o buscar firmas digitales en archivos PDF, documentos de MS Word, libros de trabajo de MS Excel, presentaciones de MS PowerPoint, archivos de Adobe Photoshop y varios formatos de imagen. Hay disponible un número asombroso de funciones y configuraciones adicionales.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Cómo validar Qrcode firmas en su documento Xlsm"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) incluye funciones útiles como la verificación de Qrcode firmas colocadas en Xlsm documentos. Aproveche esta oportunidad sin implementar código adicional.
        
        * En primer lugar, crea una instancia de la clase de firma que proporciona una ruta de parámetro de constructor a un documento que se supone que debe verificarse.
        * En segundo lugar, cree un nuevo objeto VerifyOptions y configure todas las propiedades requeridas.
        * Finalmente, invoque el método Verify del objeto de Signature pasando la instancia de VerifyOptions.
        * Luego procese los resultados de la verificación.

    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for Java son compatibles con todas las principales plataformas y sistemas operativos. Antes de ejecutar el código a continuación, asegúrese de tener los siguientes requisitos previos instalados en su sistema.

        * Sistemas operativos: Microsoft Windows, Linux, Mac OS
        * Entornos de desarrollo: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Descarga la última versión de GroupDocs.Signature for Java de [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Xlsm file
        String filePath = "input.xlsm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide verification options
        QrCodeVerifyOptions options = new QrCodeVerifyOptions();

        // process only first page
        options.setPagesSetup(new PagesSetup());
        options.setPageNumber(1);
        options.setAllPages(false);
        // specify text match type
        options.setMatchType(TextMatchType.StartsWith);
        // specify text pattern to search
        options.setText("QrCode text");
                            
        // Verify document signatures
        VerificationResult result = signature.verify(options);

        //process result
        if (result.isValid())
        {
            //..
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Firmar con Qrcode firmas Demostración en vivo"
    content: |
       Agregue varias firmas electrónicas al archivo Xlsm ahora mismo visitando el sitio web de [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Verificar otras firmas Qrcode usando Java"
    content: |
        "Verificación de firmas electrónicas colocadas en diversos documentos. Verifique la calidad de las firmas en los formatos de archivo populares como se revela a continuación."
    format: 
       
       
back_to_top:
    enable: true
---