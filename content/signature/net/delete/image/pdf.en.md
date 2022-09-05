---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Image
fileformat: Pdf
productName: .NET
lang: en
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Pdf for C#

############################# Head ############################
head_title: "Delete Image signatures from Pdf files via C#"
head_description: "Deletion of specific Image signatures from signed Pdf documents might be performed easily with short .NET code."

############################# Header ############################
title: "Remove Image signatures which are placed in Pdf files"
description: "Delete various Image signatures from Pdf documents. Removing Image signatures requires simple C# code."
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
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API provides many ways to process your documents using electronic signatures. Digital signatures like texts, images, digital certificates, barcodes, QR-codes, stamps or metadata are available. Customers have possibility to add, delete, update, verify or search digital signatures at PDFs, MS Word documents, MS Excel workbooks, MS PowerPoint presentations, Adobe Photoshop files and various image formats. A vast number of useful features and settings are provided.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "How to remove Image signatures from your Pdf document"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) provides useful feature for clearing Pdf documents of Image signatures with a few lines of code.
        
        * Firstly, instantiate Signature object passing path to your document as a constructor parameter.
        * Then, create an appropriate signature object and set up its unique identifier.
        * After that, invoke Delete method passing signature object which must be deleted.
        * Finally, process operation results.

    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for .NET are supported on all major platforms and operating systems. Before executing the code below, please make sure that you have the following prerequisites installed on your system.

        * Operating systems: Microsoft Windows, Linux, MacOS
        * Development environments: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Download the latest version of GroupDocs.Signature for .NET from [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Pdf file
        string filePath = "input.pdf";

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
    title: "Signing with Image signatures Live Demo"
    content: |
       Add various electronic signatures to Pdf file right now by visiting the [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) website.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Delete your Image signatures with C#"
    content: |
        "Deletion of e-signatures which were added to various document formats. Remove signatures quickly without extra code."
    format: 
       
       
back_to_top:
    enable: true
---