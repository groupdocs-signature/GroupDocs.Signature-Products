---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Postnet
fileformat: Ppsx
productName: .NET
lang: en
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Ppsx for C#

############################# Head ############################
head_title: "eSign Ppsx document with Postnet Barcode in C#"
head_description: "Create Postnet Barcode Signature and put it on Ppsx document with .NET using a couple lines of code. Use the GroupDocs Document Signature API for signing various file formats."

############################# Header ############################
title: "Generate Postnet Barcode signature for Ppsx document in C#"
description: "eSign your Ppsx business documents with Postnet Barcode. Generate Barcode signature quickly and easily with a few lines of code to set up signing options."
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
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) is a popular API for digital documents e-signing using many Barcode types like UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN, ITF14 and many others. Customers can create easily Barcodes providing just demanded text and put them on PDFs, MS Word documents, MS Excel workbooks, MS PowerPoint presentations, Adobe Photoshop files and various image formats. Barcodes placed in documents can be updated, searched, verified, deleted or previewed either. Moreover, barcodes customization is supported.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Steps to sign Ppsx with Barcode in C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) provides ability to sign Ppsx documents with Barcode signatures quickly and easily.
        
        * Create an instance of Signature class providing Ppsx file supposed to signing as path or memory stream
        * Instantiate SignOptions class and set all demanded data.
        * Invoke the Signature.Sign() method passing output Ppsx file or memory stream

    title_right: " System Requirements"
    content_right: |
        GroupDocs.Signature for .NET are supported on all major platforms and operating systems. Before executing the code below, please make sure that you have the following prerequisites installed on your system.

        * Operating systems: Microsoft Windows, Linux, MacOS
        * Development environments: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Get the latest GroupDocs.Signature for .NET from [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Ppsx file
        string filePath = "input.ppsx";
        // Set up output file
        string outputFilePath = "output.ppsx";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined barcode text
                var options = new BarcodeSignOptions("BC12345678")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.Postnet,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50                                        
                };
                
                // sign Ppsx document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signing Ppsx documents with Barcode Live Demo"
    content: |
       Sign Ppsx file with various signatures right now by visiting the [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) website. Free online demo waiting for you.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Postnet Barcode"
          content: |
            POSTNET (Postal Numeric Encoding Technique) is a barcode symbology used by the United States Postal Service to assist in directing mail.
          characterset: |
             Numeric digits (0-9).
          textcapacity: |
             Up to 11 characters.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAACcAAAAjCAYAAAAXMhMjAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAACeSURBVFhH7c7BCkMxEELR/P9Pp1LoRrCXpi4Cbw5kIRKZtS82x52a407Ncae+HrfWer8Pyr+i/3NcQv/nuIT+z3EJ/X/Ocf9mlxuhsXZ2uREaa2eXG6Gxdna5ERprZ5cbobF2drkRGmtnlxuhsXZ2uREaa2eXG6Gxdna5ERprZ5cbobF2drkRGmtnlxuhsXZ2ubnAHHdqjjt18XF7vwDevzbHqsQWPwAAAABJRU5ErkJggg==

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Other supported Barcode signatures for C#"
    content: |
        "You can also sign Ppsx with other signature types. Please see the list below."
    format: 
        
       
back_to_top:
    enable: true
---