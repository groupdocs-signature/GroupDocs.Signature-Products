---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Qrcode
codetype: QR
fileformat: 7z
productName: .NET
lang: ms
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Qrcode signature on 7z for C#

############################# Head ############################
head_title: "eSign 7z dokumen dengan QR QR Code dalam C#"
head_description: "Cipta QR Kod QR dan letakkan pada fail 7z menggunakan .NET dengan sekeping pendek kod C#. Gunakan API Tandatangan Dokumen GroupDocs untuk menandatangani dokumen dan fail perniagaan anda dengan Kod QR."

############################# Header ############################
title: "Hasilkan QR tandatangan Kod QR untuk 7z dokumen dalam C#"
description: "eTandatangani dokumen dan kontrak 7z anda dengan Kod QR QR. Hasilkan tandatangan Kod QR dengan cepat dan mudah."
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
    title: "Mengenai GroupDocs.Signature for .NET API tandatangan Kod QR"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) ialah API matang untuk mencipta dan menjana tandatangan Kod QR untuk dokumen. Pengguna boleh menjana tandatangan Kod QR yang menyediakan teks untuk memuat turunnya atau berkongsi melalui media sosial sebagai imej. Dokumen yang ditandatangani boleh diimbas dengan API atau hanya melalui kamera mudah alih! Tandatangani kontrak perniagaan dan dokumen rasmi anda secara elektronik dengan menambahkan tandatangan Kod QR dan memanipulasinya. Mana-mana tandatangan Kod QR akan mengandungi maklumat tersuai yang unik untuk mengenal pasti penandatangan atau membenarkan dokumen. Tambahan pula, kandungan Kod QR boleh disulitkan dan dinyahsulit dengan kunci peribadi secara pengaturcaraan. Itu membuka banyak kebolehan untuk berkongsi data sensitif di dalam dokumen awam. Selepas pengguna yang menandatangani boleh mengemas kini, mengesahkan, memadam, pratonton atau mencari Kod QR dalam PDF, dokumen MS Word, buku kerja MS Excel, persembahan MS PowerPoint, fail Adobe Photoshop dan pelbagai format imej. Kod QR boleh disesuaikan tambahan.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Langkah-langkah untuk menandatangani 7z dengan Qrcode dalam C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) menyediakan keupayaan untuk menandatangani dokumen 7z dengan tandatangan Qrcode dengan cepat dan mudah.
        
        * Buat contoh kelas Tandatangan yang menyediakan fail 7z yang sepatutnya ditandatangani sebagai laluan atau aliran memori
        * Segerakan kelas SignOptions dan tetapkan semua data yang diminta.
        * Guna kaedah Signature.Sign() yang menghantar fail keluaran 7z atau aliran memori

    title_right: " Keperluan Sistem"
    content_right: |
        GroupDocs.Signature for .NET disokong pada semua platform dan sistem pengendalian utama. Sebelum melaksanakan kod di bawah, sila pastikan anda mempunyai prasyarat berikut dipasang pada sistem anda.

        * Sistem pengendalian: Microsoft Windows, Linux, MacOS
        * Persekitaran pembangunan: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Dapatkan GroupDocs.Signature for .NET terkini daripada [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input 7z file
        string filePath = "input.7z";
        // Set up output file
        string outputFilePath = "output.7z";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined QrCode text
                QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith")
                {
                    // setup QrCode encoding type
                    EncodeType = QrCodeTypes.QR,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50
                };

                // sign 7z document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Menandatangani dokumen 7z dengan Qrcode Demo Langsung"
    content: |
       Tandatangani fail 7z dengan pelbagai tandatangan sekarang dengan melawati tapak web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demo dalam talian percuma menanti anda.

              
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About QR QrCode"
          content: |
            Kod QR (disingkatkan daripada Kod Respons Pantas) ialah tanda dagangan untuk jenis kod bar matriks (atau kod bar dua dimensi). Ia adalah jenis kod dua dimensi yang paling popular dan digunakan secara meluas. Dalam amalan, kod QR selalunya mengandungi data untuk pencari, pengecam atau penjejak yang menghala ke tapak web atau aplikasi.
          characterset: |
             Semua 256 aksara ASCII + Kanji
          textcapacity: |
             Sehingga 7089 aksara angka, 4296 aksara abjad angka, 2953 bait (data binari) atau 1817 aksara Kanji.
          image: |
             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

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Tandatangan Qrcode lain yang disokong untuk C#"
    content: |
        "Anda juga boleh menandatangani 7z dengan jenis tandatangan lain. Sila lihat senarai di bawah."
    format: 
        
       
back_to_top:
    enable: true
---