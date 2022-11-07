---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Barcode
fileformat: Ods
productName: .NET
lang: ms
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Barcode signature on Ods for C#

############################# Head ############################
head_title: "Pengesahan tandatangan Barcode untuk fail Ods melalui C#"
head_description: "Gunakan hanya beberapa baris kod .NET untuk mengesahkan dokumen Ods dan tandatangan Barcode mereka."

############################# Header ############################
title: "Barcode pengesahan tandatangan untuk fail Ods."
description: "API untuk .NET memberi peluang untuk mengesahkan tandatangan Barcode pada dokumen Ods. Pengesahan e-tandatangan di dalam dokumen Ods anda mungkin dilakukan dengan cepat dan mudah."
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
    title: "Temui ciri API GroupDocs.Signature for .NET baharu"
    content: |
        API [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) menyediakan pelbagai cara untuk memproses pelbagai format dokumen dengan menggunakan tandatangan elektronik. Banyak jenis tandatangan digital seperti teks, imej, sijil digital, kod bar, kod QR, setem atau metadata disokong. Pelanggan boleh menambah, mengalih keluar, mengedit, mengesahkan atau mencari tandatangan digital pada PDF, dokumen MS Word, buku kerja MS Excel, persembahan MS PowerPoint, fail Adobe Photoshop dan pelbagai format imej. Terdapat banyak ciri dan tetapan tambahan yang menakjubkan.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Bagaimana untuk mengesahkan tandatangan Barcode dalam dokumen Ods anda"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) termasuk ciri berguna seperti pengesahan tandatangan Barcode yang diletakkan pada dokumen Ods. Gunakan peluang ini tanpa melaksanakan kod tambahan.
        
        * Pertama, nyatakan kelas Tandatangan yang menyediakan sebagai laluan parameter pembina kepada dokumen yang sepatutnya disahkan.
        * Kedua, cipta objek VerifyOptions baharu dan sediakan semua sifat yang diperlukan.
        * Akhir sekali, gunakan kaedah Verify objek Tandatangan yang lulus contoh VerifyOptions.
        * Kemudian proses hasil pengesahan.

    title_right: "Keperluan Sistem"
    content_right: |
        GroupDocs.Signature for .NET disokong pada semua platform dan sistem pengendalian utama. Sebelum melaksanakan kod di bawah, sila pastikan anda mempunyai prasyarat berikut dipasang pada sistem anda.

        * Sistem pengendalian: Microsoft Windows, Linux, MacOS
        * Persekitaran pembangunan: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Muat turun versi terkini GroupDocs.Signature for .NET daripada [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Ods file
        string filePath = "input.ods";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide verification options
                BarcodeVerifyOptions options = new BarcodeVerifyOptions()
                {
                    // process only specified page
                    PageNumber = 3,
                    AllPages = false,
                    // set up text match type
                    MatchType = TextMatchType.Contains,
                    // specify text pattern to search
                    Text = "Special signature",
                };

                // Verify document signatures
                VerificationResult result = signature.Verify(options);

                //process result
                if (result.IsValid)
                {
                    //..
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Menandatangani dengan Barcode tandatangan Demo Langsung"
    content: |
       Tambahkan pelbagai tandatangan elektronik pada fail Ods sekarang dengan melawati tapak web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Sahkan tandatangan Barcode lain menggunakan C#"
    content: |
        "Pengesahan tandatangan elektronik yang diletakkan dalam pelbagai dokumen. Semak kualiti tandatangan dalam format fail popular seperti yang didedahkan di bawah."
    format: 
       
       
back_to_top:
    enable: true
---