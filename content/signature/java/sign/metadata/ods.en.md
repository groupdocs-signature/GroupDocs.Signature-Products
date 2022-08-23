---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Ods
productName: Java
lang: en
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpeg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Ods for Java

############################# Head ############################
head_title: "Create Metadata electronic signatures in the Ods documents with Java"
head_description: "Make Metadata as hidden electronic signatures withint the Ods documents for Java using a few lines of code. Use the GroupDocs Document Signature API to e-sign your business documents and files with Metadata information."

############################# Header ############################
title: "Metadata electronic signatures for Ods document in Java is simple and easy!"
description: "eSign your Ods documents and contracts with the hidden Metadata. Generate Metadata for image, Words, PDF, Excel and Presentation quick, easy and simple with few lines of code to set up options.!"
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
    

overview:
    enable: true
    title: "Overview API"
    content: |
        Sign your Ods files with Metadata signatures using Java easily. You can use just a couple of Java code lines in any platform of your choice like - Windows, Linux, macOS.
        You can put Metadata on Ods file in a very convenient way and for free. Besides that it is possible to sign Ods files using advanced Metadata options. 
        
        There are a lot of options features to sign Ods which you may use for your purposes:

        * Metadata position on the page can be set up as absolutely as relatively;;
        * One Metadata signature may be placed on specified pages of multi-page documents;;
        * A lot of additional signature features like color, size, border etc. are available..
        
        There are also saving options for signed Ods file:

        * after signing file might be saved with other supported format;
        * furthermore file can be encrypted with password or saved to memory stream.

        Signing Ods files with Metadata provides vast amount opportunities for users. Moreover there is no need for any additional software installed - like MS Office, Open Office, Adobe Acrobat Reader etc.


############################# Steps ############################
steps:
    enable: true
    title_left: "Steps to sign Ods with Metadata in Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) provides ability to sign Ods documents with Metadata signatures quick and easily.
        
        * Create an instance of Signature class providing Ods file supposed to signing as path or memory stream
        * Instantiate SignOptions class and set all demanded data.
        * Invoke the Signature.Sign passing output Ods file or memory stream

    title_right: "System Requirements"
    content_right: |
        Documents signing with GroupDocs.Signature for Java can be performed in just a few simple steps. Our APIs are supported on all major platforms and operating systems. Before executing the code below, make sure you have the following prerequisites installed on your system.

        * Operating systems: Microsoft Windows, Linux, MacOS
        * Development environments: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Get the latest GroupDocs.Signature for Java from [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
        
        // Set up input Ods file
        string filePath = "input.ods";
        // Set up output file
        string outputFilePath = "output.ods";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // instantiate metadata signing options
        MetadataSignOptions options = new MetadataSignOptions();

        // setup Author property
        SpreadsheetMetadataSignature mdSign_Author = new SpreadsheetMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
        options.Signatures.Add(mdSign_Author);
        // setup document data
        SpreadsheetMetadataSignature mdSign_DocData = new SpreadsheetMetadataSignature("CreatedOn", DateTime.Now);// Datetime value
        options.Signatures.Add(mdSign_DocData);
        // setup document id
        SpreadsheetMetadataSignature mdSign_DocId = new SpreadsheetMetadataSignature("DocumentId", 123456);// Integer value
        options.Signatures.Add(mdSign_DocId);

        // sign Ods document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signing Ods documents with Metadata Live Demo"
    content: |
       Sign Ods file with Metadata signature right now by visiting the [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) website. Free online demo waiting for you.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Signing Other Document Formats with Metadata using Java"
    content: |
        Java Metadata signatures management API for documents and images. Add Metadata signatures to some of the popular file formats as stated below.
    format: 
       
       
back_to_top:
    enable: true
---