---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Image
fileformat: Ots
productName: .NET
lang: es
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Ots for C#

############################# Head ############################
head_title: "Eliminar Image firmas de Ots archivos a través de C#"
head_description: "La eliminación de firmas Image específicas de documentos Ots firmados se puede realizar fácilmente con el código corto .NET."

############################# Header ############################
title: "Eliminar Image firmas que se colocan en archivos Ots"
description: "Elimine varias firmas Image de los documentos Ots. Eliminar las firmas Image requiere un código C# simple."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "Obtenga información sobre las características de la API de GroupDocs.Signature for .NET"
    content: |
        La API de [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) proporciona muchas formas de procesar sus documentos mediante firmas electrónicas. Están disponibles firmas digitales como textos, imágenes, certificados digitales, códigos de barras, códigos QR, sellos o metadatos. Los clientes tienen la posibilidad de agregar, eliminar, actualizar, verificar o buscar firmas digitales en archivos PDF, documentos de MS Word, libros de trabajo de MS Excel, presentaciones de MS PowerPoint, archivos de Adobe Photoshop y varios formatos de imagen. Se proporciona una gran cantidad de funciones y configuraciones útiles.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Cómo eliminar las firmas Image de su documento Ots"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) proporciona una característica útil para borrar documentos Ots de Image firmas con unas pocas líneas de código.
        
        * En primer lugar, cree una instancia de la ruta de paso del objeto Signature a su documento como parámetro del constructor.
        * Luego, cree un objeto de firma apropiado y configure su identificador único.
        * Después de eso, invoque el método Eliminar pasando el objeto de firma que debe eliminarse.
        * Finalmente, los resultados de la operación del proceso.

    title_right: "Requisitos del sistema"
    content_right: |
        GroupDocs.Signature for .NET son compatibles con todas las principales plataformas y sistemas operativos. Antes de ejecutar el código a continuación, asegúrese de tener los siguientes requisitos previos instalados en su sistema.

        * Sistemas operativos: Microsoft Windows, Linux, Mac OS
        * Entornos de desarrollo: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Descarga la última versión de GroupDocs.Signature for .NET de [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Ots file
        string filePath = "input.ots";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be deleted
                // such Id may be obtained as result of search operation
                string id = "e3ad0ec7-9abf-426d-b9aa-b3328f3f1470";

                // provide signature features to delete
                // set up particular signature id
                ImageSignature signatureToDelete = new ImageSignature(id);

                // delete signature
                bool deleteResult = signature.Delete(signatureToDelete);

                // process deletion result
                if (deleteResult)
                {
                    Console.WriteLine("Signature was deleted successfully!");
                }
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Firmar con Image firmas Demostración en vivo"
    content: |
       Agregue varias firmas electrónicas al archivo Ots ahora mismo visitando el sitio web de [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Elimina tus Image firmas con C#"
    content: |
        "Eliminación de firmas electrónicas que se agregaron a varios formatos de documentos. Elimine firmas rápidamente sin código adicional."
    format: 
       
       
back_to_top:
    enable: true
---