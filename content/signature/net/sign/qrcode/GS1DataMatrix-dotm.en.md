---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Qrcode
codetype: G S1 Data Matrix
fileformat: Dotm
productName: .NET
lang: en
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpeg bmp gif tiff svg webp wmf
breadcrumb: Put  Qrcode signature on Dotm for C#

############################# Head ############################
head_title: "eSign Dotm document with G S1 Data Matrix QR Code in C#"
head_description: "Create G S1 Data Matrix QR Code Signature on Dotm file for .NET using a few lines of code. Use the GroupDocs Document Signature API to e-sign your business documents and files with QR Code."

############################# Header ############################
title: "Generate G S1 Data Matrix QR Code signature for Dotm document in C#"
description: "eSign your Dotm documents and contracts with G S1 Data Matrix QR Code. Generate QR Code signature quick, easy and simple with few lines of code to set up options.!"
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
        Sign your Dotm files with Qrcode signatures using .NET easily. You can use just a couple of C# code lines in any platform of your choice like - Windows, Linux, macOS.
        You can put Qrcode on Dotm file in a very convenient way and for free. Besides that it is possible to sign Dotm files using advanced Qrcode options. 
        
        There are a lot of options features to sign Dotm which you may use for your purposes:

        * Qrcode position on the page can be set up as absolutely as relatively;;
        * One Qrcode signature may be placed on specified pages of multi-page documents;;
        * A lot of additional signature features like color, size, border etc. are available..
        
        There are also saving options for signed Dotm file:

        * after signing file might be saved with other supported format;
        * furthermore file can be encrypted with password or saved to memory stream.

        Signing Dotm files with Qrcode provides vast amount opportunities for users. Moreover there is no need for any additional software installed - like MS Office, Open Office, Adobe Acrobat Reader etc.


############################# Steps ############################
steps:
    enable: true
    title_left: "Steps to sign Dotm with Qrcode in C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) provides ability to sign Dotm documents with Qrcode signatures quick and easily.
        
        * Create an instance of Signature class providing Dotm file supposed to signing as path or memory stream
        * Instantiate SignOptions class and set all demanded data.
        * Invoke the Signature.Sign passing output Dotm file or memory stream

    title_right: "System Requirements"
    content_right: |
        Documents signing with GroupDocs.Signature for .NET can be performed in just a few simple steps. Our APIs are supported on all major platforms and operating systems. Before executing the code below, make sure you have the following prerequisites installed on your system.

        * Operating systems: Microsoft Windows, Linux, MacOS
        * Development environments: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Get the latest GroupDocs.Signature for .NET from [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Dotm file
        string filePath = "input.dotm";
        // Set up output file
        string outputFilePath = "output.dotm";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined QrCode text
                QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith")
                {
                    // setup QrCode encoding type
                    EncodeType = QrCodeTypes.G S1 Data Matrix,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50
                };

                // sign Dotm document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signing Dotm documents with Qrcode Live Demo"
    content: |
       Sign Dotm file with Qrcode signature right now by visiting the [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) website. Free online demo waiting for you.

              
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About G S1 Data Matrix QrCode"
          content: |
            GS1 Data Matrix is a variant of Data Matrix that conforms to GS1 specifications. Use GS1 DataMatrix to encode the information such as, but not limited to, the following: AI(01) Global Trade Item Number (GTIN), AI(17) Expiration Date, AI(10) Batch Number, AI(21) Serial Number.
          characterset: |
             Character set: upper and lower case letters and special characters $@%*+-./:=<>;&*_,'! all with correct Application Identifiers.
          textcapacity: |
             Codetext capacity: up to 3116 numeric digits, or 2335 alpha numeric characters.
          image: |
             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

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Signing Other Document Formats with G S1 Data Matrix Qrcode using C#"
    content: |
        .NET G S1 Data Matrix Qrcode signatures management API for documents and images. Add G S1 Data Matrix Qrcode signatures to some of the popular file formats as stated below.
    format: 
        
       
back_to_top:
    enable: true
---