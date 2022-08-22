---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Docx
productName: .NET
lang: en
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpeg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Docx for C#

############################# Head ############################
head_title: "Create Metadata electronic signatures in the Docx documents with C#"
head_description: "Make Metadata as hidden electronic signatures withint the Docx documents for .NET using a few lines of code. Use the GroupDocs Document Signature API to e-sign your business documents and files with Metadata information."

############################# Header ############################
title: "Metadata electronic signatures for Docx document in C# is simple and easy!"
description: "eSign your Docx documents and contracts with the hidden Metadata. Generate Metadata for image, Words, PDF, Excel and Presentation quick, easy and simple with few lines of code to set up options.!"
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
    

overview:
    enable: true
    title: "Overview API"
    content: |
        Sign your Docx files with Metadata signatures using .NET easily. You can use just a couple of C# code lines in any platform of your choice like - Windows, Linux, macOS.
        You can put Metadata on Docx file in a very convenient way and for free. Besides that it is possible to sign Docx files using advanced Metadata options. 
        
        There are a lot of options features to sign Docx which you may use for your purposes:

        * Metadata position on the page can be set up as absolutely as relatively;;
        * One Metadata signature may be placed on specified pages of multi-page documents;;
        * A lot of additional signature features like color, size, border etc. are available..
        
        There are also saving options for signed Docx file:

        * after signing file might be saved with other supported format;
        * furthermore file can be encrypted with password or saved to memory stream.

        Signing Docx files with Metadata provides vast amount opportunities for users. Moreover there is no need for any additional software installed - like MS Office, Open Office, Adobe Acrobat Reader etc.


############################# Steps ############################
steps:
    enable: true
    title_left: "Steps to sign Docx with Metadata in C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) provides ability to sign Docx documents with Metadata signatures quick and easily.
        
        * Create an instance of Signature class providing Docx file supposed to signing as path or memory stream
        * Instantiate SignOptions class and set all demanded data.
        * Invoke the Signature.Sign passing output Docx file or memory stream

    title_right: "System Requirements"
    content_right: |
        Documents signing with GroupDocs.Signature for .NET can be performed in just a few simple steps. Our APIs are supported on all major platforms and operating systems. Before executing the code below, make sure you have the following prerequisites installed on your system.

        * Operating systems: Microsoft Windows, Linux, MacOS
        * Development environments: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Get the latest GroupDocs.Signature for .NET from [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Docx file
        string filePath = "input.docx";
        // Set up output file
        string outputFilePath = "output.docx";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create metadata signature with predefined barcode text
                var options = new MetadataSignOptions();

                // add various metadata signature items to the document
                //  no encryption
                options
                    .Add(new PdfMetadataSignature("Author", "Mr.Scherlock Holmes")) // String value
                    .Add(new PdfMetadataSignature("CreatedOn", DateTime.Now))       // Datetime value
                    .Add(new PdfMetadataSignature("DocumentId", 123456))            // Integer value
                    .Add(new PdfMetadataSignature("SignatureId", 123.456D))         // Double value
                    .Add(new PdfMetadataSignature("Amount", 123.456M))              // Decimal value
                    .Add(new PdfMetadataSignature("Total", 123.456F));              // Float value
                
                // sign Docx document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signing Docx documents with Metadata Live Demo"
    content: |
       Sign Docx file with Metadata signature right now by visiting the [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) website. Free online demo waiting for you.          

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