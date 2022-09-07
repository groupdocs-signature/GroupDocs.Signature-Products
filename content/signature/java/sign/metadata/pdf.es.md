---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Pdf
productName: Java
lang: es
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Pdf for Java

############################# Head ############################
head_title: "Agregue firmas electrónicas de metadatos a documentos Pdf a través de Java"
head_description: "Use metadatos como firmas electrónicas ocultas dentro de sus documentos Pdf usando un par de líneas de código Java. Utilice la API de firma de documentos de GroupDocs para firmar electrónicamente sus documentos y archivos comerciales con información de metadatos."

############################# Header ############################
title: "¡Las firmas electrónicas de metadatos para el documento Pdf a través de Java son simples y fáciles de usar!"
description: "Firme electrónicamente sus documentos y contratos de Pdf con entradas de metadatos ocultas. Genere metadatos para archivos PDF, documentos de MS Word, libros de trabajo de MS Excel, presentaciones de MS PowerPoint y varios formatos de imagen sin problemas y con codificación adicional."
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
    title_left: "Pasos para firmar Pdf con Metadata en Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) proporciona la capacidad de firmar documentos Pdf con Metadata firmas de forma rápida y sencilla.
        
        * Cree una instancia de la clase Signature que proporcione el archivo Pdf que se supone que debe firmar como ruta o flujo de memoria
        * Cree una instancia de la clase SignOptions y configure todos los datos solicitados.
        * Invoque el método Signature.Sign() pasando la salida Pdf archivo o flujo de memoria

    title_right: "System Requirements"
    content_right: |
        La firma de documentos con GroupDocs.Signature for Java se puede realizar en unos pocos pasos simples. Nuestras API son compatibles con todas las principales plataformas y sistemas operativos. Antes de ejecutar el código a continuación, asegúrese de tener instalados los siguientes requisitos previos en su sistema.

        * Sistemas operativos: Microsoft Windows, Linux, Mac OS
        * Entornos de desarrollo: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Obtén el último GroupDocs.Signature for Java de [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Pdf file
        String filePath = "input.pdf";
        // Set up output file
        String outputFilePath = "output.pdf";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // instantiate metadata signing options
        MetadataSignOptions options = new MetadataSignOptions();

        // setup Author property
        PdfMetadataSignature mdSign_Author = new PdfMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
        options.getSignatures().add(mdSign_Author);
        // setup document data
        PdfMetadataSignature mdSign_DocData = new PdfMetadataSignature("CreatedOn", new Date());// Datetime value
        options.getSignatures().add(mdSign_DocData);
        // setup document id
        PdfMetadataSignature mdSign_DocId = new PdfMetadataSignature("DocumentId", 123456);// Integer value
        options.getSignatures().add(mdSign_DocId);

        // sign Pdf document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Firma de Pdf documentos con Metadata Live Demo"
    content: |
       Firme el archivo Pdf con varias firmas ahora mismo visitando el sitio web de [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demostración en línea gratuita esperándote.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Otras firmas Metadata admitidas para Java"
    content: |
        "También puede firmar Pdf con otros tipos de firma. Consulte la lista a continuación."
    format: 
       
       
back_to_top:
    enable: true
---