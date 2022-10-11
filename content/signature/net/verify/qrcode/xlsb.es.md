---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Qrcode
fileformat: Xlsb
productName: .NET
lang: es
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Qrcode signature on Xlsb for C#

############################# Head ############################
head_title: "Verificación de Qrcode firmas para Xlsb archivos a través de C#"
head_description: "Use solo unas pocas líneas de código .NET para verificar los documentos Xlsb y sus firmas Qrcode."

############################# Header ############################
title: "Qrcode verificación de firmas para Xlsb archivos"
description: "La API para .NET brinda la oportunidad de verificar Qrcode firmas en Xlsb documentos. La verificación de las firmas electrónicas dentro de sus documentos Xlsb se puede realizar rápida y fácilmente."
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
    title: "Descubra las nuevas funciones de la API de GroupDocs.Signature for .NET"
    content: |
        La API de [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) proporciona una amplia gama de formas de procesar numerosos formatos de documentos mediante el uso de firmas electrónicas. Se admiten muchos tipos de firmas digitales como textos, imágenes, certificados digitales, códigos de barras, códigos QR, sellos o metadatos. Los clientes pueden agregar, eliminar, editar, validar o buscar firmas digitales en archivos PDF, documentos de MS Word, libros de trabajo de MS Excel, presentaciones de MS PowerPoint, archivos de Adobe Photoshop y varios formatos de imagen. Hay disponible un número asombroso de funciones y configuraciones adicionales.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Cómo validar Qrcode firmas en su documento Xlsb"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) incluye funciones útiles como la verificación de Qrcode firmas colocadas en Xlsb documentos. Aproveche esta oportunidad sin implementar código adicional.
        
        * En primer lugar, crea una instancia de la clase de firma que proporciona una ruta de parámetro de constructor a un documento que se supone que debe verificarse.
        * En segundo lugar, cree un nuevo objeto VerifyOptions y configure todas las propiedades requeridas.
        * Finalmente, invoque el método Verify del objeto de Signature pasando la instancia de VerifyOptions.
        * Luego procese los resultados de la verificación.

    title_right: "Requisitos del sistema"
    content_right: |
        GroupDocs.Signature for .NET son compatibles con todas las principales plataformas y sistemas operativos. Antes de ejecutar el código a continuación, asegúrese de tener instalados los siguientes requisitos previos en su sistema.

        * Sistemas operativos: Microsoft Windows, Linux, Mac OS
        * Entornos de desarrollo: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Descarga la última versión de GroupDocs.Signature for .NET de [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Xlsb file
        string filePath = "input.xlsb";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide verification options
                QrCodeVerifyOptions options = new QrCodeVerifyOptions()
                {
                    // process only first page
                    PagesSetup = new PagesSetup() { FirstPage = true },
                    AllPages = false,
                    // set up text match type
                    MatchType = TextMatchType.StartsWith,
                    // specify text pattern to search
                    Text = "QrCode text",
                };

                // Verify document signatures
                VerificationResult result = signature.Verify(options);

                //process result
                if (result.IsValid)
                {
                    //..
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Firmar con Qrcode firmas Demostración en vivo"
    content: |
       Agregue varias firmas electrónicas al archivo Xlsb ahora mismo visitando el sitio web de [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Verificar otras firmas Qrcode usando C#"
    content: |
        "Verificación de firmas electrónicas colocadas en diversos documentos. Verifique la calidad de las firmas en los formatos de archivo populares como se revela a continuación."
    format: 
       
       
back_to_top:
    enable: true
---