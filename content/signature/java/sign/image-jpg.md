---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
otherformats: 
breadcrumb: put IMAGE signature on JPG for Java

############################# Head ############################
head_title: "Adding IMAGE signatures in a JPG file with Java"
head_description: "Put IMAGE Signature on JPG file for Java using a few lines of code. Use the GroupDocs Document Signature API to sign dozens file formats."

############################# Header ############################
title: "Operating IMAGE Signatures in .JPG files with Java"
description: "How to {{OPERATION}} IMAGE Signature with a few lines of Java code"
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
    content: |
        Sign your JPG files with IMAGE signatures using Java easily. You can use just a couple of Java code lines in any platform of your choice like - Windows, Linux, macOS.
        You can put IMAGE on JPG file in a very convenient way and for free. Besides that it is possible to sign JPG files using advanced IMAGE options. 
        
        There are a lot of options features to sign JPG which you may use for your purposes:

        * IMAGE position on the page can be set up as absolutely as relatively;;
        * One IMAGE signature may be placed on specified pages of multi-page documents;;
        * A lot of additional signature features like color, size, border etc. are available..
        
        There are also saving options for signed JPG file:

        * after signing file might be saved with other supported format;
        * furthermore file can be encrypted with password or saved to memory stream.

        Signing JPG files with IMAGE provides vast amount opportunities for users. Moreover there is no need for any additional software installed - like MS Office, Open Office, Adobe Acrobat Reader etc.


############################# Steps ############################
steps:
    enable: true
    title_left: "Steps to sign JPG with IMAGE in Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) provides ability to sign JPG documents with IMAGE signatures quick and easily.
        
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
                // Instantiate Signature for JPG file
        string filePath = "input.jpg";
        // Set up output JPG file
        string outputFilePath = "input.jpg";

        Signature signature = new Signature(filePath);

        //Provide sign options
        TextSignOptions options = new TextSignOptions("John Smith");

        // set signature position
        options.setLeft(50);
        options.setTop(50);

        // sign JPG document
        SignResult result = signature.sign(outputFilePath, options);

        ```

demos:
    enable: true
    title: "Signing JPG documents with IMAGE Live Demo"
    content: |
       Sign JPG file with IMAGE signature right now by visiting the [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) website. Free online demo waiting for you.
          

more_formats:
    enable: true
    title: "Other supported IMAGE signatures for Java"
    content: "You can also sign JPG with other signature types. Please see the list below."
       
       
back_to_top:
    enable: true
---