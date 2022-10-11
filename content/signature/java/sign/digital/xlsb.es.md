---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Xlsb
productName: Java
lang: es
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Xlsb for Java

############################# Head ############################
head_title: "Adición de firmas electrónicas digitales al archivo Xlsb con Java"
head_description: "Coloque la firma digital en el archivo Xlsb para Java usando unas pocas líneas de código. Utilice la API de firma de documentos de GroupDocs para firmar docenas de formatos de archivo."

############################# Header ############################
title: "eSign Xlsb archivos con Digital firmas en Java"
description: "Cómo agregar la firma Digital con unas pocas líneas de código Java"
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
    title: "Acerca de GroupDocs.Signature for Java API de firmas digitales"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) es una API popular para firmar documentos con firmas electrónicas digitales, con certificados digitales. Para la API de firmas digitales, se utilizan archivos de certificados PFX para firmar documentos con claves privadas y públicas protegidas con contraseña. Las firmas digitales pueden usarse para certificar documentos comerciales con una página particular de eSign PDF, certificar documentos completos de Microsoft Office como Word, Excel, archivos de Powerpoint y documentos de Open Office. Los clientes pueden manipular fácilmente las firmas, como editarlas, eliminarlas o ajustarlas. La API proporciona una forma de buscar y verificar firmas. Además, se proporcionan muchas capacidades para la personalización de firmas.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Pasos para firmar Xlsb con Digital en Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) proporciona la capacidad de firmar documentos Xlsb con Digital firmas de forma rápida y sencilla.
        
        * Cree una instancia de la clase Signature que proporcione el archivo Xlsb que se supone que debe firmar como ruta o flujo de memoria
        * Cree una instancia de la clase SignOptions y configure todos los datos solicitados.
        * Invoque el método Signature.Sign() pasando la salida Xlsb archivo o flujo de memoria

    title_right: " Requisitos del sistema"
    content_right: |
        GroupDocs.Signature for Java son compatibles con todas las principales plataformas y sistemas operativos. Antes de ejecutar el código a continuación, asegúrese de tener instalados los siguientes requisitos previos en su sistema.

        * Sistemas operativos: Microsoft Windows, Linux, Mac OS
        * Entornos de desarrollo: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Obtén el último GroupDocs.Signature for Java de [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Xlsb file
        String filePath = "input.xlsb";
        // Set up output file
        String outputFilePath = "output.xlsb";
        // Provide digital certificate
        String certificateFilePath = "certificate.pfx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        DigitalSignOptions options = new DigitalSignOptions(certificateFilePath);

        // set certificate password
        options.setPassword("1234567890");

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Xlsb document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Firma de Xlsb documentos con Digital Live Demo"
    content: |
       Firme el archivo Xlsb con varias firmas ahora mismo visitando el sitio web de [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demostración en línea gratuita esperándote.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Otras firmas Digital admitidas para Java"
    content: |
        "También puede firmar Xlsb con otros tipos de firma. Consulte la lista a continuación."
    format: 
       
       
back_to_top:
    enable: true
---