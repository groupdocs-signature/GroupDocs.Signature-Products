---
############################# Static ############################
layout: "auto-gen"
date: 2022-03-01T15:12:22
draft: false
otherformats: 
breadcrumb: put IMAGE signature on DOTX for C#

############################# Head ############################
head_title: "Adding IMAGE signatures in a DOTX file with C#"
head_description: "Put IMAGE Signature on DOTX file for .NET using a few lines of code. Use the GroupDocs Document Signature API to sign dozens file formats."

############################# Header ############################
title: "Operating IMAGE Signatures in .DOTX files with C#"
description: "How to {{OPERATION}} IMAGE Signature with a few lines of .NET code"
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
    content: |
        Sign your DOTX files with IMAGE signatures using .NET easily. You can use just a couple of C# code lines in any platform of your choice like - Windows, Linux, macOS.
        You can put IMAGE on DOTX file in a very convenient way and for free. Besides that it is possible to sign DOTX files using advanced IMAGE options. 
        
        There are a lot of options features to sign DOTX which you may use for your purposes:

        * IMAGE position on the page can be set up as absolutely as relatively;;
        * One IMAGE signature may be placed on specified pages of multi-page documents;;
        * A lot of additional signature features like color, size, border etc. are available..
        
        There are also saving options for signed DOTX file:

        * after signing file might be saved with other supported format;
        * furthermore file can be encrypted with password or saved to memory stream.

        Signing DOTX files with IMAGE provides vast amount opportunities for users. Moreover there is no need for any additional software installed - like MS Office, Open Office, Adobe Acrobat Reader etc.


############################# Steps ############################
steps:
    enable: true
    title_left: "Steps to sign DOTX with IMAGE in C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) provides ability to sign DOTX documents with IMAGE signatures quick and easily.
        
        * Create an instance of Signature class providing DOTX file supposed to signing as path or memory stream
        * Instantiate SignOptions class and set all demanded data.
        * Invoke the Signature.Sign passing output DOTX file or memory stream

    title_right: "System Requirements"
    content_right: |
        Documents signing with GroupDocs.Signature for .NET can be performed in just a few simple steps. Our APIs are supported on all major platforms and operating systems. Before executing the code below, make sure you have the following prerequisites installed on your system.

        * Operating systems: Microsoft Windows, Linux, MacOS
        * Development environments: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Get the latest GroupDocs.Signature for .NET from [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                // Instantiate Signature for DOTX file
        string filePath = "input.dotx";
        // Set up output DOTX file
        string outputFilePath = "input.dotx";

        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide sign options
                TextSignOptions options = new TextSignOptions("John Smith")
                {
                    // set signature position
                    Left = 50,
                    Top = 200,
                };

                // sign DOTX document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

demos:
    enable: true
    title: "Signing DOTX documents with IMAGE Live Demo"
    content: |
       Sign DOTX file with IMAGE signature right now by visiting the [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) website. Free online demo waiting for you.
          

more_formats:
    enable: true
    title: "Other supported IMAGE signatures for C#"
    content: "You can also sign DOTX with other signature types. Please see the list below."
       
       
back_to_top:
    enable: true
---