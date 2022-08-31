---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Image
fileformat: Xlsb
productName: .NET
lang: en
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Xlsb for C#

############################# Head ############################
head_title: "Update Image signatures placed at Xlsb files in C#"
head_description: "Use simple and easy to understand .NET code for Image signatures updation in signed Xlsb documents."

############################# Header ############################
title: "Edit and update Image signatures placed at Xlsb files"
description: "API for .NET provides functionality to edit and update Image signatures at Xlsb documents. Update e-signatures inside your Xlsb documents with a couple lines of code quickly and easily."
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
    title: "Learn about GroupDocs.Signature for .NET API features"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API functionality contains vast selection of means to process in demand documents formats by using electronic signatures. Wide spectrum of e-signatures like text, image, barcode, QR-code, stamp, form-field and metadata are supported. Customers can add, remove, edit, validate, or search digital signatures at PDF, Microsoft Word, Excel, PowerPoint and many image documents. A large number of useful features and settings are available.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "How to change Image signatures in your Xlsb document"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) includes useful features like updation of Image signatures placed at Xlsb documents. It is makes possible to change signatures features without excess code.
        
        * To start with, create Signature object passing as a constructor parameter path to a document which must to be updated.
        * Then, instantiate an approproate particular signature object and set up its identifier and properties which needs to be changed.
        * In addition, call Signature's Update method passing particular signature object.
        * Lastly, process updation result.

    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for .NET are supported on all major platforms and operating systems. Before executing the code below, please make sure that you have the following prerequisites installed on your system.

        * Operating systems: Microsoft Windows, Linux, MacOS
        * Development environments: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Download the latest version of GroupDocs.Signature for .NET from [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Xlsb file
        string filePath = "input.xlsb";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be updated
                // such Id might be get as result of search operation
                string id = "ff988ab1-7403-4c8d-8db7-f2a56b9f8530";

                // provide signature features to update
                ImageSignature signatureToUpdate = new ImageSignature()
                {
                    // set up particular signature id
                    SignatureId = id,
                    // specify signature width
                    Width = 170,
                    // specify signature height
                    Height = 250,
                    // set left position
                    Left = 10,
                    // set top position
                    Top = 10
                };

                // update signature
                bool updateResult = signature.Update(signatureToUpdate);

                // process updation result
                if (updateResult)
                {
                    Console.WriteLine("Signature was updated successfully!");
                }
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signing with Image signatures Live Demo"
    content: |
       Add various electronic signatures to Xlsb file right now by visiting the [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) website.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Signing Other Document Formats with Image using C#"
    content: |
        .NET Image signatures management API for documents and images. Add Image signatures to some of the popular file formats as stated below.
    format: 
       
       
back_to_top:
    enable: true
---