---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Qrcode
fileformat: Xlsb
productName: .NET
lang: en
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Qrcode signature on Xlsb for C#

############################# Head ############################
head_title: "Verification of Qrcode signatures for Xlsb files via C#"
head_description: "Use only a few lines of .NET code to verify Xlsb documents and their Qrcode signatures."

############################# Header ############################
title: "Qrcode signatures verification for Xlsb files"
description: "API for .NET provides opportunity to verify Qrcode signatures at Xlsb documents. Verification of e-signatures inside your Xlsb documents might be performed quickly and easily."
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
    title: "Discover new GroupDocs.Signature for .NET API features"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API provides wide range of ways to process numerous documents formats by using electronic signatures. Many types of digital signatures as texts, images, digital certificates, barcodes, QR-codes, stamps or metadata are supported. Customers can add, remove, edit, validate or search digital signatures at PDFs, MS Word documents, MS Excel workbooks, MS PowerPoint presentations, Adobe Photoshop files and various image formats. Astonishing number of additional features and settings are available.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "How to validate Qrcode signatures in your Xlsb document"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) includes useful features like verification of Qrcode signatures placed at Xlsb documents. Use this opportunity without implementing extra code.
        
        * Firstly, instantiate Signature class providing as a constructor parameter path to a document which is supposed to be verified.
        * Secondly, create a new VerifyOptions object and set up all required properties.
        * Finally, invoke Signature's object Verify method passing VerifyOptions instance.
        * Then process verification results.

    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for .NET are supported on all major platforms and operating systems. Before executing the code below, please make sure that you have the following prerequisites installed on your system.

        * Operating systems: Microsoft Windows, Linux, MacOS
        * Development environments: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Download the latest version of GroupDocs.Signature for .NET from [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
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
    title: "Signing with Qrcode signatures Live Demo"
    content: |
       Add various electronic signatures to Xlsb file right now by visiting the [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) website.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Verify other Qrcode signatures using C#"
    content: |
        "Verification of electronic signatures placed in various documents. Check quality of signatures in the popular file formats as revealed below."
    format: 
       
       
back_to_top:
    enable: true
---