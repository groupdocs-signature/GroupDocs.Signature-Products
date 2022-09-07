---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Image
fileformat: Dotx
productName: Java
lang: es
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Search Image signatures at Dotx with Java

############################# Head ############################
head_title: "Busque Image firmas en Dotx archivo en Java"
head_description: "Use Java para buscar firmas Image en archivos Dotx usando unas pocas líneas de código."

############################# Header ############################
title: "Buscar firmas Image en el archivo Dotx"
description: "Java API nativa permite buscar Image firmas en archivos Dotx ya firmados. Realice una búsqueda avanzada de firmas electrónicas dentro de sus documentos Dotx utilizando unas pocas líneas de código."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "Acerca de la API de GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) proporciona la API de Java para procesar documentos utilizando varios tipos de firma, como textos, imágenes, certificados digitales, códigos de barras, códigos QR, sellos o metadatos. Los usuarios pueden agregar, eliminar, actualizar, verificar o buscar firmas electrónicas en archivos PDF, documentos de MS Word, libros de trabajo de MS Excel, presentaciones de MS PowerPoint, archivos de Adobe Photoshop y varios formatos de imagen, con soporte adicional para personalizar las propiedades de las firmas según sea necesario.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Cómo buscar firmas Image en Dotx"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) facilita a los desarrolladores de Java la búsqueda de firmas Image en archivos Dotx desde sus aplicaciones mediante la implementación de unos sencillos pasos.
        
        * Cree una nueva instancia de la clase Signature y pase la ruta del documento de origen como parámetro del constructor.
        * Cree una instancia del objeto SearchOptions de acuerdo con sus requisitos y especifique las opciones de búsqueda.
        * Llame al método de búsqueda de la instancia de la clase Signature y pásele SearchOptions.
        * Procese los resultados de la búsqueda de acuerdo con sus demandas.

    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for Java son compatibles con todas las principales plataformas y sistemas operativos. Antes de ejecutar el código a continuación, asegúrese de tener los siguientes requisitos previos instalados en su sistema.

        * Sistemas operativos: Microsoft Windows, Linux, Mac OS
        * Entornos de desarrollo: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Descarga la última versión de GroupDocs.Signature for Java de [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Dotx file
        String filePath = "input.dotx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Create search options
        ImageSearchOptions options = new ImageSearchOptions();

        // set minimum size if needed 
        options.setMinContentSize(100);
        // set maximum image size if needed
        options.setMaxContentSize(2000);
        // return images for processing
        options.setReturnContent(true);
        // set up type of returned images
        options.setReturnContentType(FileType.PNG);

        // search for Image signatures in Dotx document
        List<ImageSignature> signatures = signature.search(ImageSignature.class, options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Firmar con Image firmas Demostración en vivo"
    content: |
       Agregue varias firmas electrónicas a los archivos Dotx ahora mismo visitando el sitio web de [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Busque otras firmas Image usando Java"
    content: |
        "Búsqueda de firmas electrónicas en diversos documentos. Encuentre firmas de uno de los formatos de archivo populares como se muestra a continuación."
    format: 
           
       
back_to_top:
    enable: true
---