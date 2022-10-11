---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Image
fileformat: Xltx
productName: .NET
lang: es
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Xltx for C#

############################# Head ############################
head_title: "Actualice Image firmas colocadas en Xltx archivos con C#"
head_description: "Use código simple y fácil de entender .NET para la actualización de firmas Image en documentos Xltx firmados."

############################# Header ############################
title: "Edite y actualice Image firmas colocadas en Xltx archivos"
description: "La API para .NET proporciona funcionalidad para la actualización de firmas Image en documentos Xltx. Actualice las firmas electrónicas dentro de sus documentos Xltx con un par de líneas de código C# rápida y fácilmente."
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
    title: "Más información sobre las funciones de la API de GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) La funcionalidad de la API contiene una amplia selección de medios para procesar formatos de documentos en demanda mediante el uso de firmas electrónicas. Se admite un amplio espectro de firmas electrónicas como textos, imágenes, certificados digitales, códigos de barras, códigos QR, sellos o metadatos. Los clientes pueden agregar, eliminar, editar, validar o buscar firmas digitales en archivos PDF, documentos de MS Word, libros de trabajo de MS Excel, presentaciones de MS PowerPoint, archivos de Adobe Photoshop y varios formatos de imagen. Numerosas funciones y configuraciones útiles están disponibles.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Cómo cambiar las firmas Image en su documento Xltx"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) incluye funciones útiles como la actualización de Image firmas colocadas en Xltx documentos. Hace posible cambiar las características de las firmas sin código adicional.
        
        * Para empezar, cree un objeto de firma que pase como una ruta de parámetro de constructor a un documento que se supone que debe actualizarse.
        * Luego, cree una instancia de un objeto de firma particular apropiado y configure su identificador y propiedades que deben cambiarse.
        * Por último, llame al método de actualización de la firma pasando un objeto de firma particular.
        * Proceso de actualización de resultados a su aviso.

    title_right: "Requisitos del sistema"
    content_right: |
        GroupDocs.Signature for .NET son compatibles con todas las principales plataformas y sistemas operativos. Antes de ejecutar el código a continuación, asegúrese de tener instalados los siguientes requisitos previos en su sistema.

        * Sistemas operativos: Microsoft Windows, Linux, Mac OS
        * Entornos de desarrollo: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Descarga la última versión de GroupDocs.Signature for .NET de [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Xltx file
        string filePath = "input.xltx";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be updated
                // such Id might be got as a result of search operation
                string id = "ff988ab1-7403-4c8d-8db7-f2a56b9f8530";

                // provide signature features to update
                // set up particular signature id
                ImageSignature signatureToUpdate = new ImageSignature(id)
                {
                    // specify signature width
                    Width = 170,
                    // specify signature height
                    Height = 250,
                    // set left position
                    Left = 10,
                    // set top position
                    Top = 10
                };

                // update signature
                bool updateResult = signature.Update(signatureToUpdate);

                // process updation result
                if (updateResult)
                {
                    Console.WriteLine("Signature was updated successfully!");
                }
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Actualización de las firmas Image en las páginas del documento: demostración en vivo"
    content: |
       Edite varias firmas electrónicas del documento Xltx ahora mismo visitando el sitio web de [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Actualice varias firmas Image a través de C#"
    content: |
        "Edición de firmas digitales que se colocan en varios formatos de documentos. Actualizar datos de firmas sin código extra."
    format: 
       
       
back_to_top:
    enable: true
---