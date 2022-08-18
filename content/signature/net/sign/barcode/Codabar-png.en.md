---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Codabar
fileformat: Png
productName: .NET
lang: en
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpeg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Png for C#

############################# Head ############################
head_title: "Adding Barcode signatures in a Png file with C#"
head_description: "Put Barcode Signature on Png file for .NET using a few lines of code. Use the GroupDocs Document Signature API to sign dozens file formats."

############################# Header ############################
title: "Sign .Png files with Barcode signatures in C#"
description: "How to add Barcode Signature with a few lines of .NET code"
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
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) is a advanced .NET API to electronically sign digital documents using various signature types such as text, image, barcode, QR-code, stamp, form-field and metadata. Users can load, edit, validate, save, remove, preview and search digital signatures within PDF, Microsoft Word, Excel worksheets, PowerPoint presentations, Adobe Photoshop, metafiles and image file formats, with additional support for customizing signature properties as needed.
    

overview:
    enable: true
    title: "Overview API"
    content: |
        Sign your Png files with Barcode signatures using .NET easily. You can use just a couple of C# code lines in any platform of your choice like - Windows, Linux, macOS.
        You can put Barcode on Png file in a very convenient way and for free. Besides that it is possible to sign Png files using advanced Barcode options. 
        
        There are a lot of options features to sign Png which you may use for your purposes:

        * Barcode position on the page can be set up as absolutely as relatively;;
        * One Barcode signature may be placed on specified pages of multi-page documents;;
        * A lot of additional signature features like color, size, border etc. are available..
        
        There are also saving options for signed Png file:

        * after signing file might be saved with other supported format;
        * furthermore file can be encrypted with password or saved to memory stream.

        Signing Png files with Barcode provides vast amount opportunities for users. Moreover there is no need for any additional software installed - like MS Office, Open Office, Adobe Acrobat Reader etc.


############################# Steps ############################
steps:
    enable: true
    title_left: "Steps to sign Png with Barcode in C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) provides ability to sign Png documents with Barcode signatures quick and easily.
        
        * Create an instance of Signature class providing Png file supposed to signing as path or memory stream
        * Instantiate SignOptions class and set all demanded data.
        * Invoke the Signature.Sign passing output Png file or memory stream

    title_right: "System Requirements"
    content_right: |
        Documents signing with GroupDocs.Signature for .NET can be performed in just a few simple steps. Our APIs are supported on all major platforms and operating systems. Before executing the code below, make sure you have the following prerequisites installed on your system.

        * Operating systems: Microsoft Windows, Linux, MacOS
        * Development environments: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Get the latest GroupDocs.Signature for .NET from [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Png file
        string filePath = "input.png";
        // Set up output file
        string outputFilePath = "output.png";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined barcode text
                BarcodeSignOptions options = new BarcodeSignOptions("JohnSmith")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.Codabar,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50
                };

                // sign Png document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signing Png documents with Barcode Live Demo"
    content: |
       Sign Png file with Barcode signature right now by visiting the [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) website. Free online demo waiting for you.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Codabar Barcode"
          content: |
            Codabar is a linear barcode symbology that was designed to be accurately read even when printed on dot-matrix printers for multi-part forms such as FedEx airbills and blood bank form.
          characterset: |
             Numeric digits (0-9) and special characters $/-:+.
          textcapacity: |
             No specific restrictions.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAD0AAABGCAYAAAB/h5zrAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAK2SURBVHhe7c9BagQBDAPB/f+nNxDQpUCOfc1MQx8khMGf7wN5n34K79NP4X36KYxPfz6fX0OyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2svfi3/I+/RTeJ9+Cg98+vv9AViQgD/8yuhqAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Signing Other Document Formats with Codabar Barcode using C#"
    content: |
        .NET Codabar Barcode signatures management API for documents and images. Add Codabar Barcode signatures to some of the popular file formats as stated below.
    format: 
           
       
back_to_top:
    enable: true
---