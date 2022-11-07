---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Digital
fileformat: Pptx
productName: .NET
lang: ms
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Pptx for C#

############################# Head ############################
head_title: "Pengesahan tandatangan Digital untuk fail Pptx melalui C#"
head_description: "Gunakan hanya beberapa baris kod .NET untuk mengesahkan dokumen Pptx dan tandatangan Digital mereka."

############################# Header ############################
title: "Digital pengesahan tandatangan untuk fail Pptx."
description: "API untuk .NET memberi peluang untuk mengesahkan tandatangan Digital pada dokumen Pptx. Pengesahan e-tandatangan di dalam dokumen Pptx anda mungkin dilakukan dengan cepat dan mudah."
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
    title_left: "Bagaimana untuk mengesahkan tandatangan Digital dalam dokumen Pptx anda"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) termasuk ciri berguna seperti pengesahan tandatangan Digital yang diletakkan pada dokumen Pptx. Gunakan peluang ini tanpa melaksanakan kod tambahan.
        
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
                
        // Set up input Pptx file
        string filePath = "input.pptx";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide verification options
                DigitalVerifyOptions options = new DigitalVerifyOptions()
                {
                    // Digital signature comment
                    Comments = "Approved by co-owner",
                    // specify period of signatures
                    SignDateTimeFrom = new DateTime(year: 2021, month: 01, day: 01),
                    SignDateTimeTo = new DateTime(year: 2022, month: 12, day: 31)
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
    title: "Menandatangani dengan Digital tandatangan Demo Langsung"
    content: |
       Tambahkan pelbagai tandatangan elektronik pada fail Pptx sekarang dengan melawati tapak web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Sahkan tandatangan Digital lain menggunakan C#"
    content: |
        "Pengesahan tandatangan elektronik yang diletakkan dalam pelbagai dokumen. Semak kualiti tandatangan dalam format fail popular seperti yang didedahkan di bawah."
    format: 
       
       
back_to_top:
    enable: true
---