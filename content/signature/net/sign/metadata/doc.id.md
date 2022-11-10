---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Doc
productName: .NET
lang: id
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Doc for C#

############################# Head ############################
head_title: "Tambahkan tanda tangan elektronik Metadata ke dokumen Doc melalui C#"
head_description: "Gunakan Metadata sebagai tanda tangan elektronik tersembunyi di dalam dokumen Doc Anda menggunakan beberapa baris kode C#. Gunakan API Tanda Tangan Dokumen GroupDocs untuk menandatangani dokumen dan file bisnis Anda secara elektronik dengan informasi Metadata."

############################# Header ############################
title: "Tanda tangan elektronik metadata untuk dokumen Doc melalui .NET sederhana dan mudah digunakan!"
description: "eSign dokumen dan kontrak Doc Anda dengan entri Metadata tersembunyi. Hasilkan Metadata untuk PDF, dokumen MS Word, buku kerja MS Excel, presentasi MS PowerPoint dan berbagai format gambar tanpa masalah dan pengkodean tambahan."
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
    title: "Tentang GroupDocs.Signature for .NET Metadata signatures API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) adalah API populer untuk penandatanganan elektronik dokumen digital. Tanda tangan seperti teks, gambar, sertifikat digital, kode batang, kode QR, perangko, atau metadata tersedia. Tanda tangan dapat ditempatkan pada PDF, dokumen MS Word, buku kerja MS Excel, presentasi MS PowerPoint, file Adobe Photoshop dan berbagai format gambar. Pelanggan dapat menandatangani dokumen mereka dan memperbarui, mencari, memverifikasi, menghapus, atau melihat pratinjau tanda tangan elektronik yang diletakkan pada dokumen tersebut. Selain itu, banyak kemampuan untuk kustomisasi tanda tangan disediakan.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Langkah-langkah untuk menandatangani Doc dengan Metadata di C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) memberikan kemampuan untuk menandatangani dokumen Doc dengan Metadata tanda tangan dengan cepat dan mudah.
        
        * Buat instance kelas Signature yang menyediakan file Doc yang seharusnya ditandatangani sebagai jalur atau aliran memori
        * Buat instance kelas SignOptions dan atur semua data yang diminta.
        * Aktifkan metode Signature.Sign() dengan meneruskan file Doc atau aliran memori

    title_right: " Persyaratan sistem"
    content_right: |
        GroupDocs.Signature for .NET didukung di semua platform dan sistem operasi utama. Sebelum menjalankan kode di bawah ini, pastikan Anda telah menginstal prasyarat berikut di sistem Anda.

        * Sistem operasi: Microsoft Windows, Linux, MacOS
        * Lingkungan pengembangan: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Dapatkan GroupDocs.Signature for .NET terbaru dari [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Doc file
        string filePath = "input.doc";
        // Set up output file
        string outputFilePath = "output.doc";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // instantiate metadata signing options
                var options = new MetadataSignOptions();

                // setup Author property
                WordProcessingMetadataSignature mdSign_Author = new WordProcessingMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
                options.Signatures.Add(mdSign_Author);
                // setup document data
                WordProcessingMetadataSignature mdSign_DocData = new WordProcessingMetadataSignature("CreatedOn", DateTime.Now);// Datetime value
                options.Signatures.Add(mdSign_DocData);
                // setup document id
                WordProcessingMetadataSignature mdSign_DocId = new WordProcessingMetadataSignature("DocumentId", 123456);// Integer value
                options.Signatures.Add(mdSign_DocId);
                
                // sign Doc document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Menandatangani dokumen Doc dengan Metadata Demo Langsung"
    content: |
       Tanda tangani file Doc dengan berbagai tanda tangan sekarang juga dengan mengunjungi situs web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demo online gratis menunggu Anda.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Tanda tangan Metadata lain yang didukung untuk C#"
    content: |
        "Anda juga dapat menandatangani Doc dengan jenis tanda tangan lainnya. Silakan lihat daftarnya di bawah ini."
    format: 
       
       
back_to_top:
    enable: true
---