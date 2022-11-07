---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: UPCA
fileformat: Docm
productName: Java
lang: ms
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Docm for Java

############################# Head ############################
head_title: "eSign Docm dokumen dengan UPCA Barcode dalam Java"
head_description: "Cipta UPCA Tandatangan Kod Bar dan letakkan pada Docm dokumen dengan Java menggunakan beberapa baris kod. Gunakan API Tandatangan Dokumen GroupDocs untuk menandatangani pelbagai format fail."

############################# Header ############################
title: "Hasilkan UPCA Tandatangan Kod Bar untuk Docm dokumen dalam Java"
description: "eTandatangani dokumen perniagaan Docm anda dengan UPCA Barcode. Hasilkan tandatangan Kod Bar dengan cepat dan mudah dengan beberapa baris kod untuk menyediakan pilihan tandatangan."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "Perihal GroupDocs.Signature for Java API tandatangan kod bar."
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) ialah API yang cepat dan mudah untuk mengurus tandatangan elektronik dokumen digital menggunakan jenis Kod Bar seperti UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN , ITF14 dan banyak lagi. Pelanggan boleh membuat Kod Bar dengan mudah dengan menyediakan teks yang diperlukan dan meletakkannya pada PDF, Dokumen Microsoft Office Words, buku kerja Microsoft Office Excel, persembahan MS PowerPoint, fail Adobe Photoshop dan pelbagai format imej. Kod bar yang diletakkan dalam dokumen boleh dikemas kini, dicari, disahkan, dipadam atau dipratonton sama ada. Selain itu, penyesuaian kod bar disokong.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Langkah-langkah untuk menandatangani Docm dengan Barcode dalam Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) menyediakan keupayaan untuk menandatangani dokumen Docm dengan tandatangan Barcode dengan cepat dan mudah.
        
        * Buat contoh kelas Tandatangan yang menyediakan fail Docm yang sepatutnya ditandatangani sebagai laluan atau aliran memori
        * Segerakan kelas SignOptions dan tetapkan semua data yang diminta.
        * Guna kaedah Signature.Sign() yang menghantar fail keluaran Docm atau aliran memori

    title_right: " Keperluan Sistem"
    content_right: |
        GroupDocs.Signature for Java disokong pada semua platform dan sistem pengendalian utama. Sebelum melaksanakan kod di bawah, sila pastikan anda mempunyai prasyarat berikut dipasang pada sistem anda.

        * Sistem pengendalian: Microsoft Windows, Linux, MacOS
        * Persekitaran pembangunan: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Dapatkan GroupDocs.Signature for Java terkini daripada [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Docm file
        String filePath = "input.docm";
        // Set up output file
        String outputFilePath = "output.docm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(BarcodeTypes.UPCA);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Docm document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Menandatangani dokumen Docm dengan Barcode Demo Langsung"
    content: |
       Tandatangani fail Docm dengan pelbagai tandatangan sekarang dengan melawati tapak web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demo dalam talian percuma menanti anda.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About UPCA Barcode"
          content: |
            Kod Produk Universal ialah simbol kod bar yang digunakan secara meluas di seluruh dunia untuk menjejaki barang dagangan di kedai.
          characterset: |
             Digit berangka (0-9).
          textcapacity: |
             Tepat 11 digit + 1 digit semak.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAGwAAABjCAYAAAB+MOUYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAARpSURBVHhe7ZFBimBRCMT6/pfuUYaAi6pe58MLSJCAG39+H5/iPexjvId9jPewj/Ee9jHewz7Ge9jH+PNhPz//M4bdzS2ZAWu7TvQytAO7m1syA9Z2nehlaAd2N7dkBqztOtHL0A7sbm7JDFjbdaKXoR3Y3dySGbC260QvQzuwu7klM2Bt14lehnZgd3NLZsDarhO9DO3A7uaWzIC1XSd6GdqB3c0tmQFru070MrQDu5tbMgPWdp3oZWgHdje3ZAas7TrRy9AO7G5uyQxY23Wil6Ed2N3ckhmwtutEL0M7sLu5JTNgbdeJXoZ2YHdzS2bA2q4TvQztwO7mlsyAtV0nehnagd3NLZkBa7tO9DK0A7ubWzID1nad6GVoB3Y3t2QGrO060cvQDuxubskMWNt1opehHdjd3JIZsLbrRC9DO7C7uSUzYG3XiV6GdmB3c0tmwNquE70M7cDu5pbMgLVdJ3oZ2oHdzS2ZAWu7TvQytAO7m1syA9Z2nehlaAd2N7dkBqztOtHL0A7sbm7JDFjbdaKXoR3Y3dySGbC260QvQzuwu7klM2Bt14lehnZgd3NLZsDarhO9DO3A7uaWzIC1XSd6GdqB3c0tmQFru070MrQDu5tbMgPWdp3oZWgHdje3ZAas7TrRy9AO7G5uyQxY23Wil6Ed2N3ckhmwtutEL0M7sLu5JTNgbdeJXoZ2YHdzS2bA2q4TvQztwO7mlsyAtV0nehnagd3NLZkBa7tO9DK0A7ubWzID1nad6GVoB3Y3t2QGrO060cvQDuxubskMWNt1opehHdjd3JIZsLbrRC9DO7C7uSUzYG3XiV6GdmB3c0tmwNquE70M7cDu5pbMgLVdJ3oZ2oHdzS2ZAWu7TvQytAO7m1syA9Z2nehlaAd2N7dkBqztOtHL0A7sbm7JDFjbdaKXoR3Y3dySGbC260QvQzuwu7klM2Bt14lehnZgd3NLZsDarhO9DO3A7uaWzIC1XSd6GdqB3c0tmQFru070MrQDu5tbMgPWdp3oZWgHdje3ZAas7TrRy9AO7G5uyQxY23Wil6Ed2N3ckhmwtutEL0M7sLu5JTNgbdeJXoZ2YHdzS2bA2q4TvQztwO7mlsyAtV0nehnagd3NLZkBa7tO9DK0A7ubWzID1nad6GVoB3Y3t2QGrO060cvQDuxubskMWNt1opehHdjd3JIZsLbrRC9DO7C7uSUzYG3XiV6GdmB3c0tmwNquE70M7cDu5pbMgLVdJ3oZ2oHdzS2ZAWu7TvQytAO7m1syA9Z2nehlaAd2N7dkBqztOtHL0A7sbm7JDFjbdaKXoR3Y3dySGbC260QvQzuwu7klM2Bt14lehnZgd3NLZsDarhO9DO3A7uaWzIC1XSd6GdqB3c0tmQFru070MrQDu5tbMgPWdp3oZWgHdje3ZAas7TrRy9AO7G5uyQxY23Wil6Ed2N3ckhmwtutEL0M7sLu5JTNgbdeJXh5K3sM+xnvYx3gP+xjvYR/jPexT/P7+A4FOQDtpBhIBAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Tandatangan Barcode lain yang disokong untuk Java"
    content: |
        "Anda juga boleh menandatangani Docm dengan jenis tandatangan lain. Sila lihat senarai di bawah."
    format: 
        
       
back_to_top:
    enable: true
---