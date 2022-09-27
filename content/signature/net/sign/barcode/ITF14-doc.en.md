---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: I T F14
fileformat: Doc
productName: .NET
lang: en
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Doc for C#

############################# Head ############################
head_title: "eSign Doc document with I T F14 Barcode in C#"
head_description: "Create I T F14 Barcode Signature and put it on Doc document with .NET using a couple lines of code. Use the GroupDocs Document Signature API for signing various file formats."

############################# Header ############################
title: "Generate I T F14 Barcode signature for Doc document in C#"
description: "eSign your Doc business documents with I T F14 Barcode. Generate Barcode signature quickly and easily with a few lines of code to set up signing options."
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
    title_left: "Steps to sign Doc with Barcode in C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) provides ability to sign Doc documents with Barcode signatures quickly and easily.
        
        * Create an instance of Signature class providing Doc file supposed to signing as path or memory stream
        * Instantiate SignOptions class and set all demanded data.
        * Invoke the Signature.Sign() method passing output Doc file or memory stream

    title_right: " System Requirements"
    content_right: |
        GroupDocs.Signature for .NET are supported on all major platforms and operating systems. Before executing the code below, please make sure that you have the following prerequisites installed on your system.

        * Operating systems: Microsoft Windows, Linux, MacOS
        * Development environments: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Get the latest GroupDocs.Signature for .NET from [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Doc file
        string filePath = "input.doc";
        // Set up output file
        string outputFilePath = "output.doc";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined barcode text
                var options = new BarcodeSignOptions("BC12345678")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.I T F14,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50                                        
                };
                
                // sign Doc document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signing Doc documents with Barcode Live Demo"
    content: |
       Sign Doc file with various signatures right now by visiting the [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) website. Free online demo waiting for you.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About I T F14 Barcode"
          content: |
            ITF-14 is the GS1 implementation of an Interleaved 2 of 5 (ITF) bar code to encode a Global Trade Item Number.
          characterset: |
             Numeric digits (0-9).
          textcapacity: |
             13 digits + 1 check digit.
          image: |
             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

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Other supported Barcode signatures for C#"
    content: |
        "You can also sign Doc with other signature types. Please see the list below."
    format: 
           
       
back_to_top:
    enable: true
---