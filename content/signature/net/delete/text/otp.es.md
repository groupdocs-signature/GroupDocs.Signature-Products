---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Text
fileformat: Otp
productName: .NET
lang: es
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Text signature on Otp for C#

############################# Head ############################
head_title: "Eliminar Text firmas de Otp archivos a través de C#"
head_description: "La eliminación de firmas Text específicas de documentos Otp firmados se puede realizar fácilmente con el código corto .NET."

############################# Header ############################
title: "Eliminar Text firmas que se colocan en archivos Otp"
description: "Elimine varias firmas Text de los documentos Otp. Eliminar las firmas Text requiere un código C# simple."
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
    title: "Obtener información sobre las características de la API de GroupDocs.Signature for .NET"
    content: |
        La API de [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) proporciona muchas formas de procesar sus documentos mediante firmas electrónicas. Están disponibles firmas digitales como textos, imágenes, certificados digitales, códigos de barras, códigos QR, sellos o metadatos. Los clientes tienen la posibilidad de agregar, eliminar, actualizar, verificar o buscar firmas digitales en archivos PDF, documentos de MS Word, libros de trabajo de MS Excel, presentaciones de MS PowerPoint, archivos de Adobe Photoshop y varios formatos de imagen. Se proporciona una gran cantidad de funciones y configuraciones útiles.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Cómo eliminar las firmas Text de su documento Otp"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) proporciona una característica útil para borrar documentos Otp de Text firmas con unas pocas líneas de código.
        
        * En primer lugar, cree una instancia de la ruta de paso del objeto Signature a su documento como parámetro del constructor.
        * Luego, cree un objeto de firma apropiado y configure su identificador único.
        * Después de eso, invoque el método Eliminar pasando el objeto de firma que debe eliminarse.
        * Finalmente, los resultados de la operación del proceso.

    title_right: "Requisitos del sistema"
    content_right: |
        GroupDocs.Signature for .NET son compatibles con todas las principales plataformas y sistemas operativos. Antes de ejecutar el código a continuación, asegúrese de tener instalados los siguientes requisitos previos en su sistema.

        * Sistemas operativos: Microsoft Windows, Linux, Mac OS
        * Entornos de desarrollo: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Descarga la última versión de GroupDocs.Signature for .NET de [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Otp file
        string filePath = "input.otp";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be deleted
                // such Id may be obtained as result of search operation
                string id = "ff988ab1-7403-4c8d-8db7-f2a56b9f8530";

                // provide signature features to delete
                // set up particular signature id
                TextSignature signatureToDelete = new TextSignature(id);

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
    title: "Firmar con Text firmas Demostración en vivo"
    content: |
       Agregue varias firmas electrónicas al archivo Otp ahora mismo visitando el sitio web de [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Elimina tus Text firmas con C#"
    content: |
        "Eliminación de firmas electrónicas que se agregaron a varios formatos de documentos. Elimine firmas rápidamente sin código adicional."
    format: 
       
       
back_to_top:
    enable: true
---