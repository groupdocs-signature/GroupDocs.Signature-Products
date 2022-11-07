---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Barcode
fileformat: Jpg
productName: .NET
lang: ms
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Barcode signatures at Jpg with C#

############################# Head ############################
head_title: "Cari tandatangan Barcode dalam fail Jpg dalam C#"
head_description: "Gunakan .NET untuk mencari tandatangan Barcode dalam fail Jpg menggunakan beberapa baris kod."

############################# Header ############################
title: "Cari tandatangan Barcode dalam fail Jpg."
description: "API asli .NET membenarkan untuk mencari tandatangan Barcode dalam fail Jpg yang telah ditandatangani. Lakukan carian e-tandatangan lanjutan dalam dokumen Jpg anda menggunakan beberapa baris kod."
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
    title: "Mengenai API GroupDocs.Signature for .NET."
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) menyediakan API .NET untuk memproses dokumen menggunakan pelbagai jenis tandatangan seperti teks, imej, sijil digital, kod bar, kod QR, setem atau metadata. Pengguna boleh menambah, memadam, mengemas kini, mengesahkan atau mencari tandatangan elektronik dalam PDF, dokumen MS Word, buku kerja MS Excel, persembahan MS PowerPoint, fail Adobe Photoshop dan pelbagai format imej, dengan sokongan tambahan untuk menyesuaikan sifat tandatangan mengikut keperluan.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Bagaimana untuk mencari tandatangan Barcode dalam Jpg"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) memudahkan pembangun .NET mencari tandatangan Barcode dalam fail Jpg daripada aplikasi mereka dengan melaksanakan beberapa langkah mudah.
        
        * Buat contoh baharu kelas Tandatangan dan lulus laluan dokumen sumber sebagai parameter pembina.
        * Segerakan objek SearchOptions mengikut keperluan anda dan tentukan pilihan carian.
        * Panggil kaedah Carian contoh kelas Tandatangan dan berikan SearchOptions kepadanya.
        * Proses hasil carian mengikut permintaan anda.

    title_right: "Keperluan Sistem"
    content_right: |
        GroupDocs.Signature for .NET disokong pada semua platform dan sistem pengendalian utama. Sebelum melaksanakan kod di bawah, sila pastikan anda mempunyai prasyarat berikut dipasang pada sistem anda.

        * Sistem pengendalian: Microsoft Windows, Linux, MacOS
        * Persekitaran pembangunan: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Muat turun versi terkini GroupDocs.Signature for .NET daripada [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Jpg file
        string filePath = "input.jpg";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Create search options
                BarcodeSearchOptions options = new BarcodeSearchOptions()
                {
                    // specify special pages to search on 
                    AllPages = false,
                    // single page number
                    PageNumber = 1,
                    // set up text match type
                    MatchType = TextMatchType.Contains,
                    // specify text pattern to search
                    Text = "Text signature",
                    // return  Barcode images for processing
                    ReturnContent = true,
                    // set up type of returned  Barcode images
                    ReturnContentType = FileType.PNG
                };

                // search for Barcode signatures in Jpg document
                List<BarcodeSignature> signatures = signature.Search<BarcodeSignature>(options);

                // process signatures which were found                
                foreach (BarcodeSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Cari Barcode tandatangan elektronik Demo Langsung"
    content: |
       Cari dokumen untuk pelbagai tandatangan elektronik pada fail Jpg sekarang dengan melawati tapak web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Cari tandatangan Barcode lain menggunakan C#"
    content: |
        "Carian tandatangan elektronik dalam pelbagai dokumen. Cari tandatangan daripada salah satu format fail yang popular seperti yang ditunjukkan di bawah."
    format: 
           
       
back_to_top:
    enable: true
---