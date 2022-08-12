---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png bmp gif tif tiff svg webp wmf
breadcrumb: Create  BARCODE signature on JPG for Java

############################# Head ############################
head_title: "Adding BARCODE signatures in a JPG file with Java"
head_description: "Put BARCODE Signature on JPG file for Java using a few lines of code. Use the GroupDocs Document Signature API to sign dozens file formats."

############################# Header ############################
title: "Sign .JPG files with BARCODE signatures in Java"
description: "How to add BARCODE Signature with a few lines of Java code"
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "About GroupDocs.Signature for Java API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) is a advanced .NET API to electronically sign digital documents using various signature types such as text, image, barcode, QR-code, stamp, form-field and metadata. Users can load, edit, validate, save, remove, preview and search digital signatures within PDF, Microsoft Word, Excel worksheets, PowerPoint presentations, Adobe Photoshop, metafiles and image file formats, with additional support for customizing signature properties as needed.
    

overview:
    enable: true
    title: "Overview API"
    content: |
        Sign your JPG files with BARCODE signatures using Java easily. You can use just a couple of Java code lines in any platform of your choice like - Windows, Linux, macOS.
        You can put BARCODE on JPG file in a very convenient way and for free. Besides that it is possible to sign JPG files using advanced BARCODE options. 
        
        There are a lot of options features to sign JPG which you may use for your purposes:

        * BARCODE position on the page can be set up as absolutely as relatively;;
        * One BARCODE signature may be placed on specified pages of multi-page documents;;
        * A lot of additional signature features like color, size, border etc. are available..
        
        There are also saving options for signed JPG file:

        * after signing file might be saved with other supported format;
        * furthermore file can be encrypted with password or saved to memory stream.

        Signing JPG files with BARCODE provides vast amount opportunities for users. Moreover there is no need for any additional software installed - like MS Office, Open Office, Adobe Acrobat Reader etc.


############################# Steps ############################
steps:
    enable: true
    title_left: "Steps to sign JPG with BARCODE in Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) provides ability to sign JPG documents with BARCODE signatures quick and easily.
        
        * Create an instance of Signature class providing JPG file supposed to signing as path or memory stream
        * Instantiate SignOptions class and set all demanded data.
        * Invoke the Signature.Sign passing output JPG file or memory stream

    title_right: "System Requirements"
    content_right: |
        Documents signing with GroupDocs.Signature for Java can be performed in just a few simple steps. Our APIs are supported on all major platforms and operating systems. Before executing the code below, make sure you have the following prerequisites installed on your system.

        * Operating systems: Microsoft Windows, Linux, MacOS
        * Development environments: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Get the latest GroupDocs.Signature for Java from [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
        
        // Set up input JPG file
        string filePath = "input.jpg";
        // Set up output file
        string outputFilePath = "output.jpg";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(BarcodeTypes.SWISSPOSTPARCEL);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign JPG document
        SignResult result = signature.sign(outputFilePath, options);

        ```

demos:
    enable: true
    title: "Signing JPG documents with BARCODE Live Demo"
    content: |
       Sign JPG file with BARCODE signature right now by visiting the [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) website. Free online demo waiting for you.

############################# More Formats ############################
more_formats:
    enable: true
    title: "Signing Other Document Formats with SWISSPOSTPARCEL BARCODE using Java"
    content: |
        Java SWISSPOSTPARCEL BARCODE signatures management API for documents and images. Add SWISSPOSTPARCEL BARCODE signatures to some of the popular file formats as stated below.
    format: 
        # format loop
        - name: "Add e-Signatures to PDF"
          link: "/signature/net/SIGN/BARCODE/SWISSPOSTPARCEL-pdf/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Add e-Signatures to DOC"
          link: "/signature/net/SIGN/BARCODE/SWISSPOSTPARCEL-doc/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Add e-Signatures to DOCX"
          link: "/signature/net/SIGN/BARCODE/SWISSPOSTPARCEL-docx/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Add e-Signatures to DOCM"
          link: "/signature/net/SIGN/BARCODE/SWISSPOSTPARCEL-docm/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Add e-Signatures to DOT"
          link: "/signature/net/SIGN/BARCODE/SWISSPOSTPARCEL-dot/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Add e-Signatures to DOTM"
          link: "/signature/net/SIGN/BARCODE/SWISSPOSTPARCEL-dotm/"
          description: "Microsoft Word Macro-Enabled Template"

        # format loop
        - name: "Add e-Signatures to DOTX"
          link: "/signature/net/SIGN/BARCODE/SWISSPOSTPARCEL-dotx/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Add e-Signatures to ODT"
          link: "/signature/net/SIGN/BARCODE/SWISSPOSTPARCEL-odt/"
          description: "Open Document Text"

        # format loop
        - name: "Add e-Signatures to OTT"
          link: "/signature/net/SIGN/BARCODE/SWISSPOSTPARCEL-ott/"
          description: "OpenDocument Text Template"

        # format loop
        - name: "Add e-Signatures to RTF"
          link: "/signature/net/SIGN/BARCODE/SWISSPOSTPARCEL-rtf/"
          description: "Rich text format"

        # format loop
        - name: "Add e-Signatures to XLS"
          link: "/signature/net/SIGN/BARCODE/SWISSPOSTPARCEL-xls/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Add e-Signatures to XLSX"
          link: "/signature/net/SIGN/BARCODE/SWISSPOSTPARCEL-xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Add e-Signatures to XLSM"
          link: "/signature/net/SIGN/BARCODE/SWISSPOSTPARCEL-xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Add e-Signatures to XLSB"
          link: "/signature/net/SIGN/BARCODE/SWISSPOSTPARCEL-xlsb/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Add e-Signatures to CSV"
          link: "/signature/net/SIGN/BARCODE/SWISSPOSTPARCEL-csv/"
          description: "Comma-separated values Worksheet"

        # format loop
        - name: "Add e-Signatures to ODS"
          link: "/signature/net/SIGN/BARCODE/SWISSPOSTPARCEL-ods/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Add e-Signatures to OTS"
          link: "/signature/net/SIGN/BARCODE/SWISSPOSTPARCEL-ots/"
          description: "OpenDocument Spreadsheet Template"

        # format loop
        - name: "Add e-Signatures to XLTX"
          link: "/signature/net/SIGN/BARCODE/SWISSPOSTPARCEL-xltx/"
          description: "Microsoft Excel template"

        # format loop
        - name: "Add e-Signatures to XLTM"
          link: "/signature/net/SIGN/BARCODE/SWISSPOSTPARCEL-xltm/"
          description: "Microsoft Excel macro-enabled template"

        # format loop
        - name: "Add e-Signatures to PPT"
          link: "/signature/net/SIGN/BARCODE/SWISSPOSTPARCEL-ppt/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Add e-Signatures to PPTX"
          link: "/signature/net/SIGN/BARCODE/SWISSPOSTPARCEL-pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Add e-Signatures to PPS"
          link: "/signature/net/SIGN/BARCODE/SWISSPOSTPARCEL-pps/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Add e-Signatures to PPSX"
          link: "/signature/net/SIGN/BARCODE/SWISSPOSTPARCEL-ppsx/"
          description: "PowerPoint Open XML Slide Show"                              

        # format loop
        - name: "Add e-Signatures to ODP"
          link: "/signature/net/SIGN/BARCODE/SWISSPOSTPARCEL-odp/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Add e-Signatures to OTP"
          link: "/signature/net/SIGN/BARCODE/SWISSPOSTPARCEL-otp/"
          description: "OpenDocument Presentation Template"

        # format loop
        - name: "Add e-Signatures to POTX"
          link: "/signature/net/SIGN/BARCODE/SWISSPOSTPARCEL-potx/"
          description: "PowerPoint template presentation" 

        # format loop
        - name: "Add e-Signatures to POTM"
          link: "/signature/net/SIGN/BARCODE/SWISSPOSTPARCEL-potm/"
          description: "PowerPoint template with support for Macros" 
          
        # format loop
        - name: "Add e-Signatures to PPTM"
          link: "/signature/net/SIGN/BARCODE/SWISSPOSTPARCEL-pptm/"
          description: "PowerPoint macro-enabled Presentation" 

        # format loop
        - name: "Add e-Signatures to PPSM"
          link: "/signature/net/SIGN/BARCODE/SWISSPOSTPARCEL-ppsm/"
          description: "PowerPoint Macro-enabled Slide Show" 

        # format loop
        - name: "Add e-Signatures to PNG"
          link: "/signature/net/SIGN/BARCODE/SWISSPOSTPARCEL-png/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Add e-Signatures to JPG"
          link: "/signature/net/SIGN/BARCODE/SWISSPOSTPARCEL-jpg/"
          description: "JPEG Image"

        # format loop
        - name: "Add e-Signatures to BMP"
          link: "/signature/net/SIGN/BARCODE/SWISSPOSTPARCEL-bmp/"
          description: "Bitmap File Format"

        # format loop
        - name: "Add e-Signatures to GIF"
          link: "/signature/net/SIGN/BARCODE/SWISSPOSTPARCEL-gif/"
          description: "Graphics Interchange Format"

        # format loop
        - name: "Add e-Signatures to TIFF"
          link: "/signature/net/SIGN/BARCODE/SWISSPOSTPARCEL-tif/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Add e-Signatures to SVG"
          link: "/signature/net/SIGN/BARCODE/SWISSPOSTPARCEL-svg/"
          description: "Scalable Vector Graphics"

        # format loop
        - name: "Add e-Signatures to WEBP"
          link: "/signature/net/SIGN/BARCODE/SWISSPOSTPARCEL-webp/"
          description: "WebP Image"

        # format loop
        - name: "Add e-Signatures to WMF"
          link: "/signature/net/SIGN/BARCODE/SWISSPOSTPARCEL-wmf/"
          description: "Windows Metafile"       
       
back_to_top:
    enable: true
---