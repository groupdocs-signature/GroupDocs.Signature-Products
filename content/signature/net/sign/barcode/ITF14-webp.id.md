---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: I T F14
fileformat: Webp
productName: .NET
lang: id
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Webp for C#

############################# Head ############################
head_title: "eSign Webp dokumen dengan I T F14 Barcode di C#"
head_description: "Buat I T F14 Tanda Tangan Barcode dan letakkan di dokumen Webp dengan .NET menggunakan beberapa baris kode. Gunakan API Tanda Tangan Dokumen GroupDocs untuk menandatangani berbagai format file."

############################# Header ############################
title: "Buat I T F14 Tanda tangan kode batang untuk dokumen Webp di C#"
description: "eSign dokumen bisnis Webp Anda dengan I T F14 Barcode. Hasilkan tanda tangan Barcode dengan cepat dan mudah dengan beberapa baris kode untuk menyiapkan opsi penandatanganan."
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
    title: "Tentang GroupDocs.Signature for .NET API tanda tangan kode batang."
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) adalah API yang cepat dan mudah untuk mengelola dokumen digital penandatanganan elektronik menggunakan jenis Barcode seperti UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN , ITF14 dan banyak lainnya. Pelanggan dapat dengan mudah membuat Barcode yang menyediakan teks yang diperlukan dan meletakkannya di PDF, Dokumen Microsoft Office Words, buku kerja Microsoft Office Excel, presentasi MS PowerPoint, file Adobe Photoshop dan berbagai format gambar. Barcode yang ditempatkan dalam dokumen dapat diperbarui, dicari, diverifikasi, dihapus, atau dipratinjau. Selain itu, kustomisasi barcode didukung.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Langkah-langkah untuk menandatangani Webp dengan Barcode di C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) memberikan kemampuan untuk menandatangani dokumen Webp dengan Barcode tanda tangan dengan cepat dan mudah.
        
        * Buat instance kelas Signature yang menyediakan file Webp yang seharusnya ditandatangani sebagai jalur atau aliran memori
        * Buat instance kelas SignOptions dan atur semua data yang diminta.
        * Aktifkan metode Signature.Sign() dengan meneruskan file Webp atau aliran memori

    title_right: " Persyaratan sistem"
    content_right: |
        GroupDocs.Signature for .NET didukung di semua platform dan sistem operasi utama. Sebelum menjalankan kode di bawah ini, pastikan Anda telah menginstal prasyarat berikut di sistem Anda.

        * Sistem operasi: Microsoft Windows, Linux, MacOS
        * Lingkungan pengembangan: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Dapatkan GroupDocs.Signature for .NET terbaru dari [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Webp file
        string filePath = "input.webp";
        // Set up output file
        string outputFilePath = "output.webp";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined barcode text
                var options = new BarcodeSignOptions("BC12345678")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.I T F14,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50                                        
                };
                
                // sign Webp document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Menandatangani dokumen Webp dengan Barcode Demo Langsung"
    content: |
       Tanda tangani file Webp dengan berbagai tanda tangan sekarang juga dengan mengunjungi situs web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demo online gratis menunggu Anda.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About I T F14 Barcode"
          content: |
            ITF-14 adalah implementasi GS1 dari kode batang Interleaved 2 of 5 (ITF) untuk mengkodekan Nomor Item Perdagangan Global.
          characterset: |
             Digit numerik (0-9).
          textcapacity: |
             13 digit + 1 digit cek.
          image: |
             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

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Tanda tangan Barcode lain yang didukung untuk C#"
    content: |
        "Anda juga dapat menandatangani Webp dengan jenis tanda tangan lainnya. Silakan lihat daftarnya di bawah ini."
    format: 
        
       
back_to_top:
    enable: true
---