---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Qrcode
fileformat: Tiff
productName: .NET
lang: en
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Qrcode signatures at Tiff with C#

############################# Head ############################
head_title: "Search Qrcode signatures in Tiff file in C#"
head_description: "Use .NET for searching Qrcode signatures in Tiff files using a few lines of code."

############################# Header ############################
title: "Search Qrcode signatures in Tiff file"
description: ".NET native API to search Qrcode signatures in already signed Tiff file. Perform advanced e-signature operations within your Tiff documents using a few lines of code."
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
    title: "About GroupDocs.Signature for .NET API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) provides .NET API for processing documents using various signature types such as text, image, barcode, QR-code, stamp, form-field and metadata. Users can load, edit, validate, save, remove, preview and search digital signatures within PDF, Microsoft Word, Excel worksheets, PowerPoint presentations, Adobe Photoshop, metafiles and image file formats, with additional support for customizing signature properties as needed.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "How to search Qrcode signatures in Tiff"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) makes it easy for .NET developers to search Qrcode signatures in Tiff files from within their applications by implementing a few easy steps.
        
        * Create new instance of Signature class and pass source document path as a constructor parameter.
        * Instantiate the SearchOptions object according to your requirements and specify search options.
        * Call Search method of Signature class instance and pass SearchOptions to it.

    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for .NET are supported on all major platforms and operating systems. Before executing the code below, please make sure that you have the following prerequisites installed on your system.

        * Operating systems: Microsoft Windows, Linux, MacOS
        * Development environments: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Download the latest version of GroupDocs.Signature for .NET from [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Tiff file
        string filePath = "input.tiff";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Create search options
                QrCodeSearchOptions options = new QrCodeSearchOptions()
                {
                    // specify special pages to search on 
                    AllPages = false,
                    // single page number
                    PageNumber = 1,
                    // set up text match type
                    MatchType = TextMatchType.Contains,
                    // specify text pattern to search
                    Text = "Text signature",
                    // return  Qrcode images for processing
                    ReturnContent = true,
                    // set up type of returned  Qrcode images
                    ReturnContentType = FileType.PNG
                };

                // search for Qrcode signatures in Tiff document
                List<QrCodeSignature> signatures = signature.Search<QrCodeSignature>(options);

                // process signatures which were found                
                foreach (QrCodeSignature signature in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signing with Qrcode signatures Live Demo"
    content: |
       Add various electronic signatures to Tiff file right now by visiting the [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) website.

        
############################# More Formats ############################
more_formats:
    enable: true
    title: Search other Qrcode signatures using C#
    content: |
        Electronic signatures search in various documents. Find signatures from some of the popular file formats as stated below.
    format: 
           
       
back_to_top:
    enable: true
---