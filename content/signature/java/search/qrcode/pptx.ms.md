---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Qrcode
fileformat: Pptx
productName: Java
lang: ms
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Qrcode signatures at Pptx with Java

############################# Head ############################
head_title: "Cari tandatangan Qrcode dalam fail Pptx dalam Java"
head_description: "Gunakan Java untuk mencari tandatangan Qrcode dalam fail Pptx menggunakan beberapa baris kod."

############################# Header ############################
title: "Cari tandatangan Qrcode dalam fail Pptx."
description: "API asli Java membenarkan untuk mencari tandatangan Qrcode dalam fail Pptx yang telah ditandatangani. Lakukan carian e-tandatangan lanjutan dalam dokumen Pptx anda menggunakan beberapa baris kod."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "Mengenai API GroupDocs.Signature for Java."
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) menyediakan API Java untuk memproses dokumen menggunakan pelbagai jenis tandatangan seperti teks, imej, sijil digital, kod bar, kod QR, setem atau metadata. Pengguna boleh menambah, memadam, mengemas kini, mengesahkan atau mencari tandatangan elektronik dalam PDF, dokumen MS Word, buku kerja MS Excel, persembahan MS PowerPoint, fail Adobe Photoshop dan pelbagai format imej, dengan sokongan tambahan untuk menyesuaikan sifat tandatangan mengikut keperluan.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Bagaimana untuk mencari tandatangan Qrcode dalam Pptx"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) memudahkan pembangun Java mencari tandatangan Qrcode dalam fail Pptx daripada aplikasi mereka dengan melaksanakan beberapa langkah mudah.
        
        * Buat contoh baharu kelas Tandatangan dan lulus laluan dokumen sumber sebagai parameter pembina.
        * Segerakan objek SearchOptions mengikut keperluan anda dan tentukan pilihan carian.
        * Panggil kaedah Carian contoh kelas Tandatangan dan berikan SearchOptions kepadanya.
        * Proses hasil carian mengikut permintaan anda.

    title_right: "Keperluan Sistem"
    content_right: |
        GroupDocs.Signature for Java disokong pada semua platform dan sistem pengendalian utama. Sebelum melaksanakan kod di bawah, sila pastikan anda mempunyai prasyarat berikut dipasang pada sistem anda.

        * Sistem pengendalian: Microsoft Windows, Linux, MacOS
        * Persekitaran pembangunan: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Muat turun versi terkini GroupDocs.Signature for Java daripada [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Pptx file
        String filePath = "input.pptx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Create search options
        QrCodeSearchOptions options = new QrCodeSearchOptions();

        // specify special pages to search on 
        options.setAllPages(false);
        // single page number
        options.setPageNumber(1);
        // specify text match type
        options.setMatchType(TextMatchType.Contains);
        // specify text pattern to search
        options.setText("Text signature");
        // return  Qrcode images for processing
        options.setReturnContent(true);
        // set up type of returned  Qrcode images
        options.setReturnContentType(FileType.PNG);
                            
        // search for Qrcode signatures in Pptx document
        List<QrCodeSignature> signatures = signature.search(QrCodeSignature.class, options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Cari Qrcode tandatangan elektronik Demo Langsung"
    content: |
       Cari dokumen untuk pelbagai tandatangan elektronik pada fail Pptx sekarang dengan melawati tapak web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Cari tandatangan Qrcode lain menggunakan Java"
    content: |
        "Carian tandatangan elektronik dalam pelbagai dokumen. Cari tandatangan daripada salah satu format fail yang popular seperti yang ditunjukkan di bawah."
    format: 
           
       
back_to_top:
    enable: true
---