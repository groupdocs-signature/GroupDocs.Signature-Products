---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Digital
fileformat: Odt
productName: .NET
lang: id
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Odt for C#

############################# Head ############################
head_title: "Verifikasi tanda tangan Digital untuk file Odt melalui C#"
head_description: "Gunakan hanya beberapa baris kode .NET untuk memverifikasi dokumen Odt dan tanda tangan Digital mereka."

############################# Header ############################
title: "Digital verifikasi tanda tangan untuk file Odt"
description: "API untuk .NET memberikan kesempatan untuk memverifikasi tanda tangan Digital pada dokumen Odt. Verifikasi tanda tangan elektronik di dalam dokumen Odt Anda dapat dilakukan dengan cepat dan mudah."
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
    title: "Temukan fitur API GroupDocs.Signature for .NET baru"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API menyediakan berbagai cara untuk memproses berbagai format dokumen dengan menggunakan tanda tangan elektronik. Banyak jenis tanda tangan digital seperti teks, gambar, sertifikat digital, kode batang, kode QR, perangko, atau metadata yang didukung. Pelanggan dapat menambah, menghapus, mengedit, memvalidasi atau mencari tanda tangan digital di PDF, dokumen MS Word, buku kerja MS Excel, presentasi MS PowerPoint, file Adobe Photoshop dan berbagai format gambar. Sejumlah fitur dan pengaturan tambahan yang menakjubkan tersedia.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Cara memvalidasi tanda tangan Digital di dokumen Odt Anda"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) menyertakan fitur berguna seperti verifikasi tanda tangan Digital yang ditempatkan di dokumen Odt. Gunakan kesempatan ini tanpa menerapkan kode tambahan.
        
        * Pertama, instantiate kelas Signature yang menyediakan jalur parameter konstruktor ke dokumen yang seharusnya diverifikasi.
        * Kedua, buat objek VerifyOptions baru dan atur semua properti yang diperlukan.
        * Terakhir, aktifkan metode Verify objek Signature dengan melewati instance VerifyOptions.
        * Kemudian proses hasil verifikasi.

    title_right: "Persyaratan sistem"
    content_right: |
        GroupDocs.Signature for .NET didukung di semua platform dan sistem operasi utama. Sebelum menjalankan kode di bawah ini, pastikan Anda telah menginstal prasyarat berikut di sistem Anda.

        * Sistem operasi: Microsoft Windows, Linux, MacOS
        * Lingkungan pengembangan: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Unduh versi terbaru GroupDocs.Signature for .NET dari [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Odt file
        string filePath = "input.odt";

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
    title: "Menandatangani dengan Digital tanda tangan Demo Langsung"
    content: |
       Tambahkan berbagai tanda tangan elektronik ke file Odt sekarang juga dengan mengunjungi situs web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Verifikasi tanda tangan Digital lainnya menggunakan C#"
    content: |
        "Verifikasi tanda tangan elektronik yang ditempatkan di berbagai dokumen. Periksa kualitas tanda tangan dalam format file populer seperti yang diungkapkan di bawah ini."
    format: 
       
       
back_to_top:
    enable: true
---