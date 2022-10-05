---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: E A N14
fileformat: Ott
productName: .NET
lang: en
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Ott for C#

############################# Head ############################
head_title: "eSign Ott document with E A N14 Barcode in C#"
head_description: "Create E A N14 Barcode Signature and put it on Ott document with .NET using a couple lines of code. Use the GroupDocs Document Signature API for signing various file formats."

############################# Header ############################
title: "Generate E A N14 Barcode signature for Ott document in C#"
description: "eSign your Ott business documents with E A N14 Barcode. Generate Barcode signature quickly and easily with a few lines of code to set up signing options."
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
    title_left: "Steps to sign Ott with Barcode in C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) provides ability to sign Ott documents with Barcode signatures quickly and easily.
        
        * Create an instance of Signature class providing Ott file supposed to signing as path or memory stream
        * Instantiate SignOptions class and set all demanded data.
        * Invoke the Signature.Sign() method passing output Ott file or memory stream

    title_right: " System Requirements"
    content_right: |
        GroupDocs.Signature for .NET are supported on all major platforms and operating systems. Before executing the code below, please make sure that you have the following prerequisites installed on your system.

        * Operating systems: Microsoft Windows, Linux, MacOS
        * Development environments: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Get the latest GroupDocs.Signature for .NET from [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Ott file
        string filePath = "input.ott";
        // Set up output file
        string outputFilePath = "output.ott";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined barcode text
                var options = new BarcodeSignOptions("BC12345678")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.E A N14,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50                                        
                };
                
                // sign Ott document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signing Ott documents with Barcode Live Demo"
    content: |
       Sign Ott file with various signatures right now by visiting the [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) website. Free online demo waiting for you.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About E A N14 Barcode"
          content: |
            European Article Number or EAN is a standard describing a barcode symbology and numbering system used in global trade to identify a specific retail product type, in a specific packaging configuration, from a specific manufacturer.
          characterset: |
             Numeric digits (0-9) and special characters.
          textcapacity: |
             Exactly 14 numeric digits.
          image: |
             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

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Other supported Barcode signatures for C#"
    content: |
        "You can also sign Ott with other signature types. Please see the list below."
    format: 
        
       
back_to_top:
    enable: true
---