---
############################# Static ############################
layout: "auto-gen"
date: 2022-03-01T15:12:22
draft: false
otherformats: pdf doc docx docm dot dotm dotx odt rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tif tiff svg webp wmf
breadcrumb: Create  BARCODE signature on OTT for C#

############################# Head ############################
head_title: "Adding BARCODE signatures in a OTT file with C#"
head_description: "Put BARCODE Signature on OTT file for .NET using a few lines of code. Use the GroupDocs Document Signature API to sign dozens file formats."

############################# Header ############################
title: "Sign .OTT files with BARCODE signatures in C#"
description: "How to add BARCODE Signature with a few lines of .NET code"
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
        Sign your OTT files with BARCODE signatures using .NET easily. You can use just a couple of C# code lines in any platform of your choice like - Windows, Linux, macOS.
        You can put BARCODE on OTT file in a very convenient way and for free. Besides that it is possible to sign OTT files using advanced BARCODE options. 
        
        There are a lot of options features to sign OTT which you may use for your purposes:

        * BARCODE position on the page can be set up as absolutely as relatively;;
        * One BARCODE signature may be placed on specified pages of multi-page documents;;
        * A lot of additional signature features like color, size, border etc. are available..
        
        There are also saving options for signed OTT file:

        * after signing file might be saved with other supported format;
        * furthermore file can be encrypted with password or saved to memory stream.

        Signing OTT files with BARCODE provides vast amount opportunities for users. Moreover there is no need for any additional software installed - like MS Office, Open Office, Adobe Acrobat Reader etc.


############################# Steps ############################
steps:
    enable: true
    title_left: "Steps to sign OTT with BARCODE in C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) provides ability to sign OTT documents with BARCODE signatures quick and easily.
        
        * Create an instance of Signature class providing OTT file supposed to signing as path or memory stream
        * Instantiate SignOptions class and set all demanded data.
        * Invoke the Signature.Sign passing output OTT file or memory stream

    title_right: "System Requirements"
    content_right: |
        Documents signing with GroupDocs.Signature for .NET can be performed in just a few simple steps. Our APIs are supported on all major platforms and operating systems. Before executing the code below, make sure you have the following prerequisites installed on your system.

        * Operating systems: Microsoft Windows, Linux, MacOS
        * Development environments: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Get the latest GroupDocs.Signature for .NET from [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input OTT file
        string filePath = "input.ott";
        // Set up output file
        string outputFilePath = "output.ott";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined barcode text
                BarcodeSignOptions options = new BarcodeSignOptions("JohnSmith")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.DEUTSCHEPOSTLEITCODE,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50
                };

                // sign OTT document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

demos:
    enable: true
    title: "Signing OTT documents with BARCODE Live Demo"
    content: |
       Sign OTT file with BARCODE signature right now by visiting the [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) website. Free online demo waiting for you.

############################# More Formats ############################
more_formats:
    enable: true
    title: "Signing Other Document Formats with DEUTSCHEPOSTLEITCODE BARCODE using C#"
    content: |
        .NET DEUTSCHEPOSTLEITCODE BARCODE signatures management API for documents and images. Add DEUTSCHEPOSTLEITCODE BARCODE signatures to some of the popular file formats as stated below.
    format: 
        # format loop
        - name: "Add e-Signatures to PDF"
          link: "/signature/net/SIGN/BARCODE/DEUTSCHEPOSTLEITCODE-pdf/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Add e-Signatures to DOC"
          link: "/signature/net/SIGN/BARCODE/DEUTSCHEPOSTLEITCODE-doc/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Add e-Signatures to DOCX"
          link: "/signature/net/SIGN/BARCODE/DEUTSCHEPOSTLEITCODE-docx/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Add e-Signatures to DOCM"
          link: "/signature/net/SIGN/BARCODE/DEUTSCHEPOSTLEITCODE-docm/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Add e-Signatures to DOT"
          link: "/signature/net/SIGN/BARCODE/DEUTSCHEPOSTLEITCODE-dot/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Add e-Signatures to DOTM"
          link: "/signature/net/SIGN/BARCODE/DEUTSCHEPOSTLEITCODE-dotm/"
          description: "Microsoft Word Macro-Enabled Template"

        # format loop
        - name: "Add e-Signatures to DOTX"
          link: "/signature/net/SIGN/BARCODE/DEUTSCHEPOSTLEITCODE-dotx/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Add e-Signatures to ODT"
          link: "/signature/net/SIGN/BARCODE/DEUTSCHEPOSTLEITCODE-odt/"
          description: "Open Document Text"

        # format loop
        - name: "Add e-Signatures to OTT"
          link: "/signature/net/SIGN/BARCODE/DEUTSCHEPOSTLEITCODE-ott/"
          description: "OpenDocument Text Template"

        # format loop
        - name: "Add e-Signatures to RTF"
          link: "/signature/net/SIGN/BARCODE/DEUTSCHEPOSTLEITCODE-rtf/"
          description: "Rich text format"

        # format loop
        - name: "Add e-Signatures to XLS"
          link: "/signature/net/SIGN/BARCODE/DEUTSCHEPOSTLEITCODE-xls/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Add e-Signatures to XLSX"
          link: "/signature/net/SIGN/BARCODE/DEUTSCHEPOSTLEITCODE-xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Add e-Signatures to XLSM"
          link: "/signature/net/SIGN/BARCODE/DEUTSCHEPOSTLEITCODE-xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Add e-Signatures to XLSB"
          link: "/signature/net/SIGN/BARCODE/DEUTSCHEPOSTLEITCODE-xlsb/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Add e-Signatures to CSV"
          link: "/signature/net/SIGN/BARCODE/DEUTSCHEPOSTLEITCODE-csv/"
          description: "Comma-separated values Worksheet"

        # format loop
        - name: "Add e-Signatures to ODS"
          link: "/signature/net/SIGN/BARCODE/DEUTSCHEPOSTLEITCODE-ods/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Add e-Signatures to OTS"
          link: "/signature/net/SIGN/BARCODE/DEUTSCHEPOSTLEITCODE-ots/"
          description: "OpenDocument Spreadsheet Template"

        # format loop
        - name: "Add e-Signatures to XLTX"
          link: "/signature/net/SIGN/BARCODE/DEUTSCHEPOSTLEITCODE-xltx/"
          description: "Microsoft Excel template"

        # format loop
        - name: "Add e-Signatures to XLTM"
          link: "/signature/net/SIGN/BARCODE/DEUTSCHEPOSTLEITCODE-xltm/"
          description: "Microsoft Excel macro-enabled template"

        # format loop
        - name: "Add e-Signatures to PPT"
          link: "/signature/net/SIGN/BARCODE/DEUTSCHEPOSTLEITCODE-ppt/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Add e-Signatures to PPTX"
          link: "/signature/net/SIGN/BARCODE/DEUTSCHEPOSTLEITCODE-pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Add e-Signatures to PPS"
          link: "/signature/net/SIGN/BARCODE/DEUTSCHEPOSTLEITCODE-pps/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Add e-Signatures to PPSX"
          link: "/signature/net/SIGN/BARCODE/DEUTSCHEPOSTLEITCODE-ppsx/"
          description: "PowerPoint Open XML Slide Show"                              

        # format loop
        - name: "Add e-Signatures to ODP"
          link: "/signature/net/SIGN/BARCODE/DEUTSCHEPOSTLEITCODE-odp/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Add e-Signatures to OTP"
          link: "/signature/net/SIGN/BARCODE/DEUTSCHEPOSTLEITCODE-otp/"
          description: "OpenDocument Presentation Template"

        # format loop
        - name: "Add e-Signatures to POTX"
          link: "/signature/net/SIGN/BARCODE/DEUTSCHEPOSTLEITCODE-potx/"
          description: "PowerPoint template presentation" 

        # format loop
        - name: "Add e-Signatures to POTM"
          link: "/signature/net/SIGN/BARCODE/DEUTSCHEPOSTLEITCODE-potm/"
          description: "PowerPoint template with support for Macros" 
          
        # format loop
        - name: "Add e-Signatures to PPTM"
          link: "/signature/net/SIGN/BARCODE/DEUTSCHEPOSTLEITCODE-pptm/"
          description: "PowerPoint macro-enabled Presentation" 

        # format loop
        - name: "Add e-Signatures to PPSM"
          link: "/signature/net/SIGN/BARCODE/DEUTSCHEPOSTLEITCODE-ppsm/"
          description: "PowerPoint Macro-enabled Slide Show" 

        # format loop
        - name: "Add e-Signatures to PNG"
          link: "/signature/net/SIGN/BARCODE/DEUTSCHEPOSTLEITCODE-png/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Add e-Signatures to JPG"
          link: "/signature/net/SIGN/BARCODE/DEUTSCHEPOSTLEITCODE-jpg/"
          description: "JPEG Image"

        # format loop
        - name: "Add e-Signatures to BMP"
          link: "/signature/net/SIGN/BARCODE/DEUTSCHEPOSTLEITCODE-bmp/"
          description: "Bitmap File Format"

        # format loop
        - name: "Add e-Signatures to GIF"
          link: "/signature/net/SIGN/BARCODE/DEUTSCHEPOSTLEITCODE-gif/"
          description: "Graphics Interchange Format"

        # format loop
        - name: "Add e-Signatures to TIFF"
          link: "/signature/net/SIGN/BARCODE/DEUTSCHEPOSTLEITCODE-tif/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Add e-Signatures to SVG"
          link: "/signature/net/SIGN/BARCODE/DEUTSCHEPOSTLEITCODE-svg/"
          description: "Scalable Vector Graphics"

        # format loop
        - name: "Add e-Signatures to WEBP"
          link: "/signature/net/SIGN/BARCODE/DEUTSCHEPOSTLEITCODE-webp/"
          description: "WebP Image"

        # format loop
        - name: "Add e-Signatures to WMF"
          link: "/signature/net/SIGN/BARCODE/DEUTSCHEPOSTLEITCODE-wmf/"
          description: "Windows Metafile"       
       
back_to_top:
    enable: true
---