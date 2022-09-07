---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Image
fileformat: Ppsm
productName: .NET
lang: es
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Search Image signatures at Ppsm with C#

############################# Head ############################
head_title: "Busque Image firmas en Ppsm archivo en C#"
head_description: "Use .NET para buscar firmas Image en archivos Ppsm usando unas pocas líneas de código."

############################# Header ############################
title: "Buscar firmas Image en el archivo Ppsm"
description: ".NET API nativa permite buscar Image firmas en archivos Ppsm ya firmados. Realice una búsqueda avanzada de firmas electrónicas dentro de sus documentos Ppsm utilizando unas pocas líneas de código."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "Acerca de la API de GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) proporciona la API de .NET para procesar documentos utilizando varios tipos de firma, como textos, imágenes, certificados digitales, códigos de barras, códigos QR, sellos o metadatos. Los usuarios pueden agregar, eliminar, actualizar, verificar o buscar firmas electrónicas en archivos PDF, documentos de MS Word, libros de trabajo de MS Excel, presentaciones de MS PowerPoint, archivos de Adobe Photoshop y varios formatos de imagen, con soporte adicional para personalizar las propiedades de las firmas según sea necesario.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Cómo buscar firmas Image en Ppsm"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) facilita a los desarrolladores de .NET la búsqueda de firmas Image en archivos Ppsm desde sus aplicaciones mediante la implementación de unos sencillos pasos.
        
        * Cree una nueva instancia de la clase Signature y pase la ruta del documento de origen como parámetro del constructor.
        * Cree una instancia del objeto SearchOptions de acuerdo con sus requisitos y especifique las opciones de búsqueda.
        * Llame al método de búsqueda de la instancia de la clase Signature y pásele SearchOptions.
        * Procese los resultados de la búsqueda de acuerdo con sus demandas.

    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for .NET son compatibles con todas las principales plataformas y sistemas operativos. Antes de ejecutar el código a continuación, asegúrese de tener los siguientes requisitos previos instalados en su sistema.

        * Sistemas operativos: Microsoft Windows, Linux, Mac OS
        * Entornos de desarrollo: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Descarga la última versión de GroupDocs.Signature for .NET de [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Ppsm file
        string filePath = "input.ppsm";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Create search options
                ImageSearchOptions options = new ImageSearchOptions()
                {
                    // set minimum size if needed
                    MinContentSize = 100,
                    // set maximum image size if needed
                    MaxContentSize = 2000,                    
                    // return  Image images for processing
                    ReturnContent = true,
                    // set up type of returned  Image images
                    ReturnContentType = FileType.PNG                                 
                };

                // search for Image signatures in Ppsm document
                List<ImageSignature> signatures = signature.Search<ImageSignature>(options);

                // process signatures which were found                
                foreach (ImageSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Firmar con Image firmas Demostración en vivo"
    content: |
       Agregue varias firmas electrónicas a los archivos Ppsm ahora mismo visitando el sitio web de [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Busque otras firmas Image usando C#"
    content: |
        "Búsqueda de firmas electrónicas en diversos documentos. Encuentre firmas de uno de los formatos de archivo populares como se muestra a continuación."
    format: 
           
       
back_to_top:
    enable: true
---