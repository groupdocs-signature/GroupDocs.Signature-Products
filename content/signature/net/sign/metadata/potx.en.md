---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Potx
productName: .NET
lang: en
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Potx for C#

############################# Head ############################
head_title: "Create Metadata electronic signatures in the Potx documents with C#"
head_description: "Make Metadata as hidden electronic signatures withint the Potx documents for .NET using a few lines of code. Use the GroupDocs Document Signature API to e-sign your business documents and files with Metadata information."

############################# Header ############################
title: "Metadata electronic signatures for Potx document in C# is simple and easy!"
description: "eSign your Potx documents and contracts with the hidden Metadata. Generate Metadata for image, Words, PDF, Excel and Presentation quick, easy and simple with few lines of code to set up options."
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
    title: "About GroupDocs.Signature for .NET API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) is a advanced .NET API to e-sign documents with digital signatures using QR Code. Users can generate QR code to download it, share over the social media as image. The signed document can be scanned with API or simply over the mobile camera! Sign electronically your business contracts and official documents with adding QR Code signature and manipulate it. Any QR Code signature will contains unique custom information to identifies the signer or authorizes the document. Also the QR Code content can be encrypted and decrypted with personal keys programitically. That allows many posibilities to share sensetive data inside the public documents. After the signing user can update, verify, remove, preview and search for the Barcodes within PDF, Microsoft Word, Excel worksheets, PowerPoint presentations, Adobe Photoshop, metafiles and image file formats, with additional support for customizing signature properties as needed.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Steps to sign Potx with Metadata in C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) provides ability to sign Potx documents with Metadata signatures quickly and easily.
        
        * Create an instance of Signature class providing Potx file supposed to signing as path or memory stream
        * Instantiate SignOptions class and set all demanded data.
        * Invoke the Signature.Sign passing output Potx file or memory stream

    title_right: "System Requirements"
    content_right: |
        Documents signing with GroupDocs.Signature for .NET can be performed in just a few simple steps. Our APIs are supported on all major platforms and operating systems. Before executing the code below, make sure you have the following prerequisites installed on your system.

        * Operating systems: Microsoft Windows, Linux, MacOS
        * Development environments: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Get the latest GroupDocs.Signature for .NET from [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Potx file
        string filePath = "input.potx";
        // Set up output file
        string outputFilePath = "output.potx";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // instantiate metadata signing options
                var options = new MetadataSignOptions();

                // setup Author property
                PresentationMetadataSignature mdSign_Author = new PresentationMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
                options.Signatures.Add(mdSign_Author);
                // setup document data
                PresentationMetadataSignature mdSign_DocData = new PresentationMetadataSignature("CreatedOn", DateTime.Now);// Datetime value
                options.Signatures.Add(mdSign_DocData);
                // setup document id
                PresentationMetadataSignature mdSign_DocId = new PresentationMetadataSignature("DocumentId", 123456);// Integer value
                options.Signatures.Add(mdSign_DocId);
                
                // sign Potx document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signing Potx documents with Metadata Live Demo"
    content: |
       Sign Potx file with various signatures right now by visiting the [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) website. Free online demo waiting for you.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Signing Other Document Formats with Metadata using C#"
    content: |
        .NET Metadata signatures management API for documents and images. Add Metadata signatures to some of the popular file formats as stated below.
    format: 
       
       
back_to_top:
    enable: true
---