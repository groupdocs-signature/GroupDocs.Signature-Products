---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Pptx
productName: Java
lang: es
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Pptx for Java

############################# Head ############################
head_title: "Agregando Digital firmas al archivo Pptx con Java"
head_description: "Coloque la firma Digital en el archivo Pptx para Java usando unas pocas líneas de código. Utilice la API de firma de documentos de GroupDocs para firmar docenas de formatos de archivo."

############################# Header ############################
title: "Firme Pptx archivos con Digital firmas en Java"
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
    title: "Acerca de la API de GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) es una API popular para la firma electrónica de documentos digitales. Están disponibles firmas como textos, imágenes, certificados digitales, códigos de barras, códigos QR, sellos o metadatos. Las firmas se pueden colocar en archivos PDF, documentos de MS Word, libros de trabajo de MS Excel, presentaciones de MS PowerPoint, archivos de Adobe Photoshop y varios formatos de imagen. Los clientes pueden firmar su documento y actualizar, buscar, verificar, eliminar o obtener una vista previa de las firmas electrónicas que se colocaron en esos documentos. Además, se proporcionan muchas capacidades para la personalización de firmas.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Pasos para firmar Pptx con Digital en Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) proporciona la capacidad de firmar documentos Pptx con Digital firmas de forma rápida y sencilla.
        
        * Cree una instancia de la clase Signature que proporcione el archivo Pptx que se supone que debe firmar como ruta o flujo de memoria
        * Cree una instancia de la clase SignOptions y configure todos los datos solicitados.
        * Invoque el método Signature.Sign() pasando la salida Pptx archivo o flujo de memoria

    title_right: "System Requirements"
    content_right: |
        La firma de documentos con GroupDocs.Signature for Java se puede realizar en unos pocos pasos simples. Nuestras API son compatibles con todas las principales plataformas y sistemas operativos. Antes de ejecutar el código a continuación, asegúrese de tener instalados los siguientes requisitos previos en su sistema.

        * Sistemas operativos: Microsoft Windows, Linux, Mac OS
        * Entornos de desarrollo: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Obtén el último GroupDocs.Signature for Java de [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Pptx file
        String filePath = "input.pptx";
        // Set up output file
        String outputFilePath = "output.pptx";
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

        // sign Pptx document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Firma de Pptx documentos con Digital Live Demo"
    content: |
       Firme el archivo Pptx con varias firmas ahora mismo visitando el sitio web de [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demostración en línea gratuita esperándote.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Otras firmas Digital admitidas para Java"
    content: |
        "También puede firmar Pptx con otros tipos de firma. Consulte la lista a continuación."
    format: 
       
       
back_to_top:
    enable: true
---