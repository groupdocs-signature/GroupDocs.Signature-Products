---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Qrcode
fileformat: Dot
productName: .NET
lang: en
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Qrcode signature on Dot for C#

############################# Head ############################
head_title: "Delete Qrcode signatures from Dot files in C#"
head_description: "Deletion of specific Qrcode signatures from signed Dot documents might be performed easily with short .NET code."

############################# Header ############################
title: "Remove Qrcode signatures which are in Dot files"
description: "Delete various Qrcode signatures from Dot documents. Removing Qrcode signatures requires simple C# code."
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
    title: "Get information about GroupDocs.Signature for .NET API features"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API provides many ways to process your documents with electronic signatures. Digital signatures like text, image, barcode, QR-code, stamp, form-field and metadata are available. Customers have possibility to add, delete, edit, validate, or search digital signatures at PDF, Microsoft Word, Excel, PowerPoint and many other document formats. A vast number of useful features and settings are provided.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "How to remove Qrcode signatures from your Dot document"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) provides useful feature of clearing Dot documents of Qrcode signatures with a few lines of code.
        
        * Firstly, instantiate Signature object passing path to your document as a constructor parameter.
        * Then, create an approproate signature object and set up its unique identifier.
        * After that, invoke Delete method passing signature object which must be deleted.
        * Finally, process updation result.

    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for .NET are supported on all major platforms and operating systems. Before executing the code below, please make sure that you have the following prerequisites installed on your system.

        * Operating systems: Microsoft Windows, Linux, MacOS
        * Development environments: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Download the latest version of GroupDocs.Signature for .NET from [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Dot file
        string filePath = "input.dot";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be deleted
                // such Id may be obtained as result of search operation
                string id = "eff64a14-dad9-47b0-88e5-2ee4e3604e71";

                // provide signature features to delete
                QrCodeSignature signatureToDelete = new QrCodeSignature()
                {
                    // set up particular signature id
                    SignatureId = id
                };

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
    title: "Signing with Qrcode signatures Live Demo"
    content: |
       Add various electronic signatures to Dot file right now by visiting the [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) website.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Signing Other Document Formats with Qrcode using C#"
    content: |
        .NET Qrcode signatures management API for documents and images. Add Qrcode signatures to some of the popular file formats as stated below.
    format: 
       
       
back_to_top:
    enable: true
---