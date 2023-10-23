---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Tar
productName: .NET
lang: es
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Tar for C#

############################# Head ############################
head_title: "Adición de firmas electrónicas digitales al archivo Tar con C#"
head_description: "Coloque la firma digital en el archivo Tar para .NET usando unas pocas líneas de código. Utilice la API de firma de documentos de GroupDocs para firmar docenas de formatos de archivo."

############################# Header ############################
title: "eSign Tar archivos con Digital firmas en C#"
description: "Cómo agregar la firma Digital con unas pocas líneas de código .NET"
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
    title: "Acerca de GroupDocs.Signature for .NET API de firmas digitales"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) es una API popular para firmar documentos con firmas electrónicas digitales, con certificados digitales. Para la API de firmas digitales, se utilizan archivos de certificados PFX para firmar documentos con claves privadas y públicas protegidas con contraseña. Las firmas digitales pueden usarse para certificar documentos comerciales con una página particular de eSign PDF, certificar documentos completos de Microsoft Office como Word, Excel, archivos de Powerpoint y documentos de Open Office. Los clientes pueden manipular fácilmente las firmas, como editarlas, eliminarlas o ajustarlas. La API proporciona una forma de buscar y verificar firmas. Además, se proporcionan muchas capacidades para la personalización de firmas.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Pasos para firmar Tar con Digital en C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) proporciona la capacidad de firmar documentos Tar con Digital firmas de forma rápida y sencilla.
        
        * Cree una instancia de la clase Signature que proporcione el archivo Tar que se supone que debe firmar como ruta o flujo de memoria
        * Cree una instancia de la clase SignOptions y configure todos los datos solicitados.
        * Invoque el método Signature.Sign() pasando la salida Tar archivo o flujo de memoria

    title_right: " Requisitos del sistema"
    content_right: |
        GroupDocs.Signature for .NET son compatibles con todas las principales plataformas y sistemas operativos. Antes de ejecutar el código a continuación, asegúrese de tener instalados los siguientes requisitos previos en su sistema.

        * Sistemas operativos: Microsoft Windows, Linux, Mac OS
        * Entornos de desarrollo: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Obtén el último GroupDocs.Signature for .NET de [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Tar file
        string filePath = "input.tar";
        // Set up output file
        string outputFilePath = "output.tar";
        // Provide digital certificate
        string certificateFilePath = "certificate.pfx";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide sign options
                DigitalSignOptions options = new DigitalSignOptions(certificateFilePath)
                {
                    // set certificate password
                    Password = "1234567890",
                    // set signature position
                    Left = 50,
                    Top = 200,
                };

                // sign Tar document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Firma de Tar documentos con Digital Live Demo"
    content: |
       Firme el archivo Tar con varias firmas ahora mismo visitando el sitio web de [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demostración en línea gratuita esperándote.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Otras firmas Digital admitidas para C#"
    content: |
        "También puede firmar Tar con otros tipos de firma. Consulte la lista a continuación."
    format: 
       
       
back_to_top:
    enable: true
---