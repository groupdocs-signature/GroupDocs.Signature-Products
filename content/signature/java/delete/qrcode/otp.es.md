---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Qrcode
fileformat: Otp
productName: Java
lang: es
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Qrcode signature on Otp for Java

############################# Head ############################
head_title: "Eliminar Qrcode firmas de Otp archivos a través de Java"
head_description: "La eliminación de firmas Qrcode específicas de documentos Otp firmados se puede realizar fácilmente con el código corto Java."

############################# Header ############################
title: "Eliminar Qrcode firmas que se colocan en archivos Otp"
description: "Elimine varias firmas Qrcode de los documentos Otp. Eliminar las firmas Qrcode requiere un código Java simple."
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
    title: "Obtener información sobre las características de la API de GroupDocs.Signature for Java"
    content: |
        La API de [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) proporciona muchas formas de procesar sus documentos mediante firmas electrónicas. Están disponibles firmas digitales como textos, imágenes, certificados digitales, códigos de barras, códigos QR, sellos o metadatos. Los clientes tienen la posibilidad de agregar, eliminar, actualizar, verificar o buscar firmas digitales en archivos PDF, documentos de MS Word, libros de trabajo de MS Excel, presentaciones de MS PowerPoint, archivos de Adobe Photoshop y varios formatos de imagen. Se proporciona una gran cantidad de funciones y configuraciones útiles.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Cómo eliminar las firmas Qrcode de su documento Otp"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) proporciona una característica útil para borrar documentos Otp de Qrcode firmas con unas pocas líneas de código.
        
        * En primer lugar, cree una instancia de la ruta de paso del objeto Signature a su documento como parámetro del constructor.
        * Luego, cree un objeto de firma apropiado y configure su identificador único.
        * Después de eso, invoque el método Eliminar pasando el objeto de firma que debe eliminarse.
        * Finalmente, los resultados de la operación del proceso.

    title_right: "Requisitos del sistema"
    content_right: |
        GroupDocs.Signature for Java son compatibles con todas las principales plataformas y sistemas operativos. Antes de ejecutar el código a continuación, asegúrese de tener instalados los siguientes requisitos previos en su sistema.

        * Sistemas operativos: Microsoft Windows, Linux, Mac OS
        * Entornos de desarrollo: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Descarga la última versión de GroupDocs.Signature for Java de [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Otp file
        String filePath = "input.otp";
        // Set up output file
        String outputFilePath = "output.otp";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be deleted
        // such Id may be obtained as result of search operation
        String id = "eff64a14-dad9-47b0-88e5-2ee4e3604e71";

        // provide signature features to delete
        QrCodeSignature signatureToDelete = new QrCodeSignature(id);

        // delete signature
        Boolean deleteResult = signature.delete(outputFilePath, signatureToDelete);

        // process deletion result
        if (deleteResult)
        {
                System.out.println("Signature was deleted successfully!");
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Firmar con Qrcode firmas Demostración en vivo"
    content: |
       Agregue varias firmas electrónicas al archivo Otp ahora mismo visitando el sitio web de [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Elimina tus Qrcode firmas con Java"
    content: |
        "Eliminación de firmas electrónicas que se agregaron a varios formatos de documentos. Elimine firmas rápidamente sin código adicional."
    format: 
       
       
back_to_top:
    enable: true
---