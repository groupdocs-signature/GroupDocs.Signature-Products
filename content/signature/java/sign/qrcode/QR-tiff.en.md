---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Qrcode
codetype: QR
fileformat: Tiff
productName: Java
lang: en
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Qrcode signature on Tiff for Java

############################# Head ############################
head_title: "eSign Tiff document with QR QR Code in Java"
head_description: "Create QR QR Code Signature on Tiff file for Java using a few lines of code. Use the GroupDocs Document Signature API to e-sign your business documents and files with QR Code."

############################# Header ############################
title: "Generate QR QR Code signature for Tiff document in Java"
description: "eSign your Tiff documents and contracts with QR QR Code. Generate QR Code signature quick, easy and simple with few lines of code to set up options.!"
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
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) is a advanced .NET API to e-sign documents with digital signatures using QR Code. Users can generate QR code to download it, share over the social media as image. The signed document can be scanned with API or simply over the mobile camera! Sign electronically your business contracts and official documents with adding QR Code signature and manipulate it. Any QR Code signature will contains unique custom information to identifies the signer or authorizes the document. Also the QR Code content can be encrypted and decrypted with personal keys programitically. That allows many posibilities to share sensetive data inside the public documents. After the signing user can update, verify, remove, preview and search for the Barcodes within PDF, Microsoft Word, Excel worksheets, PowerPoint presentations, Adobe Photoshop, metafiles and image file formats, with additional support for customizing signature properties as needed.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Steps to sign Tiff with Qrcode in Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) provides ability to sign Tiff documents with Qrcode signatures quick and easily.
        
        * Create an instance of Signature class providing Tiff file supposed to signing as path or memory stream
        * Instantiate SignOptions class and set all demanded data.
        * Invoke the Signature.Sign passing output Tiff file or memory stream

    title_right: "System Requirements"
    content_right: |
        Documents signing with GroupDocs.Signature for Java can be performed in just a few simple steps. Our APIs are supported on all major platforms and operating systems. Before executing the code below, make sure you have the following prerequisites installed on your system.

        * Operating systems: Microsoft Windows, Linux, MacOS
        * Development environments: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Get the latest GroupDocs.Signature for Java from [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Tiff file
        string filePath = "input.tiff";
        // Set up output file
        string outputFilePath = "output.tiff";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(QrCodeTypes.QR);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Tiff document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signing Tiff documents with Qrcode Live Demo"
    content: |
       Sign Tiff file with various signatures right now by visiting the [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) website. Free online demo waiting for you.

              
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About QR QrCode"
          content: |
            QR Code (abbreviated from Quick Response Code) is the trademark for a type of matrix barcode (or two-dimensional barcode). It is most popular and widely used type of two-dimensional code. In practice, QR codes often contain data for a locator, identifier, or tracker that points to a website or application.
          characterset: |
             All 256 ASCII characters + Kanji
          textcapacity: |
             Up to 7089 numeric characters, 4296 alphanumeric characters, 2953 bytes (binary data) or 1817 Kanji characters.
          image: |
             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

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Signing Other Document Formats with QR Qrcode using Java"
    content: |
        Java QR Qrcode signatures management API for documents and images. Add QR Qrcode signatures to some of the popular file formats as stated below.
    format: 
        
       
back_to_top:
    enable: true
---