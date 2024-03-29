---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Digital
fileformat: Xls
productName: .NET
lang: en
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Xls for C#

############################# Head ############################
head_title: "Delete Digital signatures from Xls files via C#"
head_description: "Deletion of specific Digital signatures from signed Xls documents might be performed easily with short .NET code."

############################# Header ############################
title: "Remove Digital signatures which are placed in Xls files"
description: "Delete various Digital signatures from Xls documents. Removing Digital signatures requires simple C# code."
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
    title_left: "How to remove Digital signatures from your Xls document"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) provides useful feature for clearing Xls documents of Digital signatures with a few lines of code.
        
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
                
        // Set up input Xls file
        string filePath = "input.xls";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be deleted
                // such Id may be obtained as result of search operation
                string id = "a01e1940-997a-444b-89af-9309a2d559a5";

                // provide signature features to delete
                // set up particular signature id
                DigitalSignature signatureToDelete = new DigitalSignature(id);

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
    title: "Signing with Digital signatures Live Demo"
    content: |
       Add various electronic signatures to Xls file right now by visiting the [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) website.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Delete your Digital signatures with C#"
    content: |
        "Deletion of e-signatures which were added to various document formats. Remove signatures quickly without extra code."
    format: 
       
       
back_to_top:
    enable: true
---