
---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Text
fileformat: Pdf
productName: .NET
lang: en
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpeg bmp gif tiff svg webp wmf
breadcrumb: Put Text signature on Pdf for C#

############################# Head ############################
head_title: "Adding Text signatures in a Pdf file with C#"
head_description: "Put Text Signature on Pdf file for .NET using a few lines of code. Use the GroupDocs Document Signature API to sign dozens file formats."

############################# Header ############################
title: "Sign .Pdf files with Text signatures in C#"
description: "How to add Text Signature with a few lines of .NET code"
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
        Sign your Pdf files with Text signatures using .NET easily. You can use just a couple of C# code lines in any platform of your choice like - Windows, Linux, macOS.
        You can put Text on Pdf file in a very convenient way and for free. Besides that it is possible to sign Pdf files using advanced Text options. 
        
        There are a lot of options features to sign Pdf which you may use for your purposes:

        * Text position on the page can be set up as absolutely as relatively;;
        * One Text signature may be placed on specified pages of multi-page documents;;
        * A lot of additional signature features like color, size, border etc. are available..
        
        There are also saving options for signed Pdf file:

        * after signing file might be saved with other supported format;
        * furthermore file can be encrypted with password or saved to memory stream.

        Signing Pdf files with Text provides vast amount opportunities for users. Moreover there is no need for any additional software installed - like MS Office, Open Office, Adobe Acrobat Reader etc.


############################# Steps ############################
steps:
    enable: true
    title_left: "Steps to sign Pdf with Text in C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) provides ability to sign Pdf documents with Text signatures quick and easily.
        
        * Create an instance of Signature class providing Pdf file supposed to signing as path or memory stream
        * Instantiate SignOptions class and set all demanded data.
        * Invoke the Signature.Sign passing output Pdf file or memory stream

    title_right: "System Requirements"
    content_right: |
        Documents signing with GroupDocs.Signature for .NET can be performed in just a few simple steps. Our APIs are supported on all major platforms and operating systems. Before executing the code below, make sure you have the following prerequisites installed on your system.

        * Operating systems: Microsoft Windows, Linux, MacOS
        * Development environments: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Get the latest GroupDocs.Signature for .NET from [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Pdf file
        string filePath = "input.pdf";
        // Set up output file
        string outputFilePath = "output.pdf";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide sign options
                TextSignOptions options = new TextSignOptions("John Smith")
                {
                    // set signature position
                    Left = 50,
                    Top = 200,
                };

                // sign Pdf document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signing Pdf documents with Text Live Demo"
    content: |
       Sign Pdf file with Text signature right now by visiting the [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) website. Free online demo waiting for you.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Signing Other Document Formats with Text using C#"
    content: |
        .NET Text signatures management API for documents and images. Add Text signatures to some of the popular file formats as stated below.
    format: 
       
       
back_to_top:
    enable: true
---