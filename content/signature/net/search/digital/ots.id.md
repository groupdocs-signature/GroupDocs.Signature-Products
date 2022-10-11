---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Digital
fileformat: Ots
productName: .NET
lang: id
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Search Digital signatures at Ots with C#

############################# Head ############################
head_title: "Cari tanda tangan Digital dalam file Ots di C#"
head_description: "Gunakan .NET untuk mencari tanda tangan Digital di file Ots menggunakan beberapa baris kode."

############################# Header ############################
title: "Cari tanda tangan Digital di file Ots"
description: ".NET API asli memungkinkan untuk mencari Digital tanda tangan di file Ots yang sudah ditandatangani. Lakukan pencarian tanda tangan elektronik lanjutan dalam dokumen Ots Anda menggunakan beberapa baris kode."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "Tentang GroupDocs.Signature for .NET API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) menyediakan .NET API untuk memproses dokumen menggunakan berbagai jenis tanda tangan seperti teks, gambar, sertifikat digital, kode batang, kode QR, stempel, atau metadata. Pengguna dapat menambah, menghapus, memperbarui, memverifikasi atau mencari tanda tangan elektronik dalam PDF, dokumen MS Word, buku kerja MS Excel, presentasi MS PowerPoint, file Adobe Photoshop dan berbagai format gambar, dengan dukungan tambahan untuk menyesuaikan properti tanda tangan sesuai kebutuhan.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Cara mencari tanda tangan Digital di Ots"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) memudahkan pengembang .NET untuk mencari tanda tangan Digital dalam file Ots dari aplikasi mereka dengan menerapkan beberapa langkah mudah.
        
        * Buat instance baru kelas Signature dan teruskan jalur dokumen sumber sebagai parameter konstruktor.
        * Buat instance objek SearchOptions sesuai dengan kebutuhan Anda dan tentukan opsi pencarian.
        * Panggil metode Pencarian dari instance kelas Signature dan berikan SearchOptions ke sana.
        * Proses pencarian hasil sesuai dengan permintaan Anda.

    title_right: "Persyaratan sistem"
    content_right: |
        GroupDocs.Signature for .NET didukung di semua platform dan sistem operasi utama. Sebelum menjalankan kode di bawah ini, pastikan Anda telah menginstal prasyarat berikut di sistem Anda.

        * Sistem operasi: Microsoft Windows, Linux, MacOS
        * Lingkungan pengembangan: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Unduh versi terbaru GroupDocs.Signature for .NET dari [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Ots file
        string filePath = "input.ots";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Create search options
                DigitalSearchOptions options = new DigitalSearchOptions()
                {
                    // specify special search criteria
                    Comments = "Approved",
                    // specify date range period of signature
                    SignDateTimeFrom = new DateTime(year: 2020, month: 01, day: 01),
                    SignDateTimeTo = new DateTime(year: 2020, month: 12, day: 31)
                };

                // search for Digital signatures in Ots document
                List<DigitalSignature> signatures = signature.Search<DigitalSignature>(options);

                // process signatures which were found                
                foreach (DigitalSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Telusuri Digital tanda tangan elektronik Demo Langsung"
    content: |
       Cari dokumen untuk berbagai tanda tangan elektronik ke file Ots sekarang juga dengan mengunjungi situs web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Cari tanda tangan Digital lainnya menggunakan C#"
    content: |
        "Pencarian tanda tangan elektronik di berbagai dokumen. Temukan tanda tangan dari salah satu format file populer seperti yang ditunjukkan di bawah ini."
    format: 
           
       
back_to_top:
    enable: true
---