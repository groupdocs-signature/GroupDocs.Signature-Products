---
############################# Static ############################
layout: "auto-gen"
date: 2021-05-13T13:39:52+03:00
draft: false

############################# Head ############################
head_title: "How to Add Digital Signatures to ODT Files in Java"
head_description: "Learn how to add digital signatures to a ODT file in Java using GroupDocs.Siganture API - add customized electronic signatures to popular business documents and image file formats."

############################# Header ############################
title: "Add Digital Signatures to ODT in Java"
description: "Secure your ODT files by adding popular digital signature types using Java library. Manipulate electronic signatures properties and set up advance signing options within documents as you may need."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Download Free Trial"
    link: "https://downloads.groupdocs.com/signature/java"

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"

    middle:
        button:

            # button loop
            - link: "https://apireference.groupdocs.com/signature/java"
              text: "API Reference"

            # button loop
            - link: "https://github.com/groupdocs-signature"
              text: "Code Examples"

            # button loop
            - link: "https://products.groupdocs.app/signature/family"
              text: "Live Demos"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/signature/java"
              text: "Pricing"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/java"
        link_buy: "https://purchase.groupdocs.com"

############################# About ############################
about:
    enable: true
    title: "About GroupDocs.Signature for Java API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java) is an advanced Java library to digitally sign documents using various signature types such as text, image, barcode, stamp, form-field, QR-code and metadata. By adding just a few lines of code, empower your Java applications with features to add, edit, verify, delete and search digital signatures within PDF, Microsoft Word, Excel worksheets, PowerPoint presentations, Adobe Photoshop, metafiles and image file formats. The e-signature API also supports additional features to customize signature properties as per requirements.

############################# Steps ############################
steps:
    enable: true
    title_left: "How to Add Digital Signatures in a ODT File"
    content_left: |
        The below code example clearly demonstrates the steps about **how to add digital signatures to a ODT file using [GroupDocs.Signature](https://products.groupdocs.com/signature/java) library in Java** by adding just a few lines of code.

        *   Create new instance of [Signature](https://apireference.groupdocs.com/java/signature/com.groupdocs.signature/Signature) class and pass source document path as a constructor parameter.
        *   Instantiate the [DigitalSignOptions](https://apireference.groupdocs.com/java/signature/com.groupdocs.signature.options.sign/DigitalSignOptions) object with required certificate & password.
        *   Call [Sign](https://apireference.groupdocs.com/java/signature/com.groupdocs.signature/Signature#sign(java.io.OutputStream,%20com.groupdocs.signature.options.sign.SignOptions)) method of [Signature](https://apireference.groupdocs.com/java/signature/com.groupdocs.signature/Signature) class instance; pass DigitalSignOptions to it.
        *   Analyze [SignResult](https://apireference.groupdocs.com/java/signature/com.groupdocs.signature.domain/SignResult) result to check newly created signatures if needed.
        
    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for Java APIs are supported on all major platforms and operating systems. Before executing the code below, please make sure that you have the following prerequisites installled on your system.

        *   Operating Systems: Microsoft Windows, Linux, MacOS
        *   Development Environments: Visual Studio, Xamarin, MonoDevelop
        *   Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        *   Download the latest version of GroupDocs.Signature for Java from [Nuget](https://www.nuget.org/packages/groupdocs.signature)
        
    code: |
        ```java
        Signature signature = new Signature("sample.pdf"); 
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");
         
        // certifiate password
        options.setPassword("1234567890");
        // digital certificate details
        options.setReason("Sign");
        options.setContact("JohnSmith");
        options.setLocation("Office1");
         
        // image as digital certificate appearance on document pages
        options.setImageFilePath("sample.jpg");
        //
        options.setAllPages(true);
        options.setWidth(80);
        options.setHeight(60);
        options.setVerticalAlignment(VerticalAlignment.Bottom);
        options.setHorizontalAlignment(HorizontalAlignment.Right);
        Padding padding = new Padding();
        padding.setBottom(10);
        padding.setRight(10);
        options.setMargin(padding);
         
        SignResult signResult = signature.sign("signed.odt", options);
        // analyzing result
        System.out.print("List of newly created signatures:");
        int number = 1;
        for(BaseSignature temp : signResult.getSucceeded())
        {
            System.out.print("Signature #"+ number++ +": Type: "+temp.getSignatureType()+" Id:"+temp.getSignatureId()+
                    ",Location: "+temp.getLeft()+"x"+temp.getTop()+". Size: "+temp.getWidth()+"x"+temp.getHeight());
        }
        ```
        
############################# Demos ############################
demos:
    enable: true
    title: "Add ODT Signature Live Demos"
    content: |
        Add ODT file electronic signatures right now by visiting [GroupDocs.Signature Live Demos](https://products.groupdocs.app/signature/family) website.
        The live demo has the following benefits
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-odt"
          title: "What is ODT File Format"
          content: |
            ODT files are type of documents created with word processing applications that are based on OpenDocument Text File format. These are created with word processor applications such as free OpenOffice Writer and can hold content such as text, images, objects and styles. The ODT file is to Writer word processor what the DOCX is to Microsoft Word. Several applications including Google Docs and Google's web-based word processor included with Google Drive can open the ODT files for editing. Microsoft Word can also open ODT files and save it in to other formats such as DOC and DOCX. Learn more about ODT file format

          link: "https://docs.fileformat.com/word-processing/odt/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Other Available Options"
    content: |
        Multi-format digital signatures API for documents and images. Add signatures to some of the popular file formats as stated below.
    format: 
        # format loop
        - name: "Add e-Signatures to PDF"
          link: "https://products.groupdocs.com/signature/java/add/pdf/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Add e-Signatures to DOC"
          link: "https://products.groupdocs.com/signature/java/add/doc/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Add e-Signatures to DOCM"
          link: "https://products.groupdocs.com/signature/java/add/docm/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Add e-Signatures to DOCX"
          link: "https://products.groupdocs.com/signature/java/add/docx/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Add e-Signatures to DOT"
          link: "https://products.groupdocs.com/signature/java/add/dot/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Add e-Signatures to DOTX"
          link: "https://products.groupdocs.com/signature/java/add/dotx/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Add e-Signatures to DOTM"
          link: "https://products.groupdocs.com/signature/java/add/dotm/"
          description: "Microsoft Word Macro-Enabled Template"

        # format loop
        - name: "Add e-Signatures to RTF"
          link: "https://products.groupdocs.com/signature/java/add/rtf/"
          description: "Rich Text Document"

        # format loop
        - name: "Add e-Signatures to ODT"
          link: "https://products.groupdocs.com/signature/java/add/odt/"
          description: "Open Document Text"

        # format loop
        - name: "Add e-Signatures to OTT"
          link: "https://products.groupdocs.com/signature/java/add/ott/"
          description: "OpenDocument Text Template"

        # format loop
        - name: "Add e-Signatures to XLS"
          link: "https://products.groupdocs.com/signature/java/add/xls/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Add e-Signatures to XLSX"
          link: "https://products.groupdocs.com/signature/java/add/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Add e-Signatures to XLSM"
          link: "https://products.groupdocs.com/signature/java/add/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Add e-Signatures to XLSM"
          link: "https://products.groupdocs.com/signature/java/add/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Add e-Signatures to XLSB"
          link: "https://products.groupdocs.com/signature/java/add/xlsb/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Add e-Signatures to XLTX"
          link: "https://products.groupdocs.com/signature/java/add/xltx/"
          description: "Microsoft Excel template"

        # format loop
        - name: "Add e-Signatures to XLTM"
          link: "https://products.groupdocs.com/signature/java/add/xltm/"
          description: "Microsoft Excel macro-enabled template"

        # format loop
        - name: "Add e-Signatures to ODS"
          link: "https://products.groupdocs.com/signature/java/add/ods/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Add e-Signatures to OTS"
          link: "https://products.groupdocs.com/signature/java/add/ots/"
          description: "OpenDocument Spreadsheet Template"

        # format loop
        - name: "Add e-Signatures to PPT"
          link: "https://products.groupdocs.com/signature/java/add/ppt/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Add e-Signatures to PPTX"
          link: "https://products.groupdocs.com/signature/java/add/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Add e-Signatures to PPS"
          link: "https://products.groupdocs.com/signature/java/add/pps/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Add e-Signatures to PPSX"
          link: "https://products.groupdocs.com/signature/java/add/ppsx/"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Add e-Signatures to POTM"
          link: "https://products.groupdocs.com/signature/java/add/potm/"
          description: "Microsoft PowerPoint Macro-Enabled Template"

        # format loop
        - name: "Add e-Signatures to POTX"
          link: "https://products.groupdocs.com/signature/java/add/potx/"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Add e-Signatures to PPTM"
          link: "https://products.groupdocs.com/signature/java/add/pptm/"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Add e-Signatures to ODP"
          link: "https://products.groupdocs.com/signature/java/add/odp/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Add e-Signatures to OTP"
          link: "https://products.groupdocs.com/signature/java/add/otp/"
          description: "OpenDocument Presentation Template"

        # format loop
        - name: "Add e-Signatures to WEBP"
          link: "https://products.groupdocs.com/signature/java/add/webp/"
          description: "WebP Image"

        # format loop
        - name: "Add e-Signatures to TIFF"
          link: "https://products.groupdocs.com/signature/java/add/tiff/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Add e-Signatures to JPEG"
          link: "https://products.groupdocs.com/signature/java/add/jpeg/"
          description: "JPEG Image"

        # format loop
        - name: "Add e-Signatures to GIF"
          link: "https://products.groupdocs.com/signature/java/add/gif/"
          description: "Graphics Interchange Format"

        # format loop
        - name: "Add e-Signatures to PNG"
          link: "https://products.groupdocs.com/signature/java/add/png/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Add e-Signatures to BMP"
          link: "https://products.groupdocs.com/signature/java/add/bmp/"
          description: "Bitmap File Format"

        # format loop
        - name: "Add e-Signatures to CDR"
          link: "https://products.groupdocs.com/signature/java/add/cdr/"
          description: "CorelDraw Vector Graphic Drawing"

        # format loop
        - name: "Add e-Signatures to SVG"
          link: "https://products.groupdocs.com/signature/java/add/svg/"
          description: "Scalable Vector Graphics"

        # format loop
        - name: "Add e-Signatures to PSD"
          link: "https://products.groupdocs.com/signature/java/add/psd/"
          description: "Adobe Photoshop Document"

        # format loop
        - name: "Add e-Signatures to WMF"
          link: "https://products.groupdocs.com/signature/java/add/wmf/"
          description: "Windows Metafile"

        # format loop
        - name: "Add e-Signatures to EMF"
          link: "https://products.groupdocs.com/signature/java/add/emf/"
          description: "Enhanced Metafile Format"

        # format loop
        - name: "Add e-Signatures to CMX"
          link: "https://products.groupdocs.com/signature/java/add/cmx/"
          description: "Corel Metafile eXchange Image"

        # format loop
        - name: "Add e-Signatures to DJVU"
          link: "https://products.groupdocs.com/signature/java/add/djvu/"
          description: "Deja Vu"

        # format loop
        - name: "Add e-Signatures to PPSM"
          link: "https://products.groupdocs.com/signature/java/add/ppsm/"
          description: "Microsoft PowerPoint Macro-Enabled Slide Show"

        # format loop
        - name: "Add e-Signatures to DCM"
          link: "https://products.groupdocs.com/signature/java/add/dcm/"
          description: "Digital Imaging and Communications in Medicine"


############################# Back to top ###############################
back_to_top:
    enable: true
---
