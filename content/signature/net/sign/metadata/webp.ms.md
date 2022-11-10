---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Webp
productName: .NET
lang: ms
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Webp for C#

############################# Head ############################
head_title: "Tambahkan tandatangan elektronik Metadata pada dokumen Webp melalui C#"
head_description: "Gunakan Metadata sebagai tandatangan elektronik tersembunyi di dalam dokumen Webp anda menggunakan beberapa baris kod C#. Gunakan API Tandatangan Dokumen GroupDocs untuk menandatangani dokumen dan fail perniagaan anda dengan maklumat Metadata."

############################# Header ############################
title: "Tandatangan elektronik metadata untuk dokumen Webp melalui .NET adalah mudah dan mudah untuk digunakan!"
description: "eTandatangani dokumen dan kontrak Webp anda dengan entri Metadata tersembunyi. Jana Metadata untuk PDF, dokumen MS Word, buku kerja MS Excel, persembahan MS PowerPoint dan pelbagai format imej tanpa masalah dan pengekodan tambahan."
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
    title: "Perihal GroupDocs.Signature for .NET API tandatangan metadata"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) ialah API popular untuk tandatangan elektronik dokumen digital. Tandatangan seperti teks, imej, sijil digital, kod bar, kod QR, setem atau metadata tersedia. Tandatangan mungkin diletakkan pada PDF, dokumen MS Word, buku kerja MS Excel, persembahan MS PowerPoint, fail Adobe Photoshop dan pelbagai format imej. Pelanggan boleh menandatangani dokumen mereka dan mengemas kini, mencari, mengesahkan, memadam atau pratonton e-tandatangan yang diletakkan pada dokumen tersebut. Selain itu, banyak kebolehan untuk penyesuaian tandatangan disediakan.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Langkah-langkah untuk menandatangani Webp dengan Metadata dalam C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) menyediakan keupayaan untuk menandatangani dokumen Webp dengan tandatangan Metadata dengan cepat dan mudah.
        
        * Buat contoh kelas Tandatangan yang menyediakan fail Webp yang sepatutnya ditandatangani sebagai laluan atau aliran memori
        * Segerakan kelas SignOptions dan tetapkan semua data yang diminta.
        * Guna kaedah Signature.Sign() yang menghantar fail keluaran Webp atau aliran memori

    title_right: " Keperluan Sistem"
    content_right: |
        GroupDocs.Signature for .NET disokong pada semua platform dan sistem pengendalian utama. Sebelum melaksanakan kod di bawah, sila pastikan anda mempunyai prasyarat berikut dipasang pada sistem anda.

        * Sistem pengendalian: Microsoft Windows, Linux, MacOS
        * Persekitaran pembangunan: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Dapatkan GroupDocs.Signature for .NET terkini daripada [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Webp file
        string filePath = "input.webp";
        // Set up output file
        string outputFilePath = "output.webp";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // instantiate metadata signing options
                MetadataSignOptions options = new MetadataSignOptions();

                // Specify different Metadata Signatures and add them to options signature collection
                // set start id
                ushort imgsMetadataId = 41996;
                // setup int value
                ImageMetadataSignature mdSign_DocId = new ImageMetadataSignature(imgsMetadataId++, 123456); // int
                options.Signatures.Add(mdSign_DocId);
                // setup Author property
                ImageMetadataSignature mdSign_Author = new ImageMetadataSignature(imgsMetadataId++, "Mr.Scherlock Holmes"); // string
                options.Signatures.Add(mdSign_Author);
                // setup data of sign date
                ImageMetadataSignature mdSign_Date = new ImageMetadataSignature(imgsMetadataId++, DateTime.Now); // DateTime
                options.Signatures.Add(mdSign_Date);
                // setup double
                ImageMetadataSignature mdSign_Amnt = new ImageMetadataSignature(imgsMetadataId++, 123.456M); //decimal value
                options.Signatures.Add(mdSign_Amnt);

                // sign Webp document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Menandatangani dokumen Webp dengan Metadata Demo Langsung"
    content: |
       Tandatangani fail Webp dengan pelbagai tandatangan sekarang dengan melawati tapak web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demo dalam talian percuma menanti anda.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Tandatangan Metadata lain yang disokong untuk C#"
    content: |
        "Anda juga boleh menandatangani Webp dengan jenis tandatangan lain. Sila lihat senarai di bawah."
    format: 
       
       
back_to_top:
    enable: true
---