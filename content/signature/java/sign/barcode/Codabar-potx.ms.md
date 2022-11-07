---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Codabar
fileformat: Potx
productName: Java
lang: ms
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Potx for Java

############################# Head ############################
head_title: "eSign Potx dokumen dengan Codabar Barcode dalam Java"
head_description: "Cipta Codabar Tandatangan Kod Bar dan letakkan pada Potx dokumen dengan Java menggunakan beberapa baris kod. Gunakan API Tandatangan Dokumen GroupDocs untuk menandatangani pelbagai format fail."

############################# Header ############################
title: "Hasilkan Codabar Tandatangan Kod Bar untuk Potx dokumen dalam Java"
description: "eTandatangani dokumen perniagaan Potx anda dengan Codabar Barcode. Hasilkan tandatangan Kod Bar dengan cepat dan mudah dengan beberapa baris kod untuk menyediakan pilihan tandatangan."
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
    title_left: "Langkah-langkah untuk menandatangani Potx dengan Barcode dalam Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) menyediakan keupayaan untuk menandatangani dokumen Potx dengan tandatangan Barcode dengan cepat dan mudah.
        
        * Buat contoh kelas Tandatangan yang menyediakan fail Potx yang sepatutnya ditandatangani sebagai laluan atau aliran memori
        * Segerakan kelas SignOptions dan tetapkan semua data yang diminta.
        * Guna kaedah Signature.Sign() yang menghantar fail keluaran Potx atau aliran memori

    title_right: " Keperluan Sistem"
    content_right: |
        GroupDocs.Signature for Java disokong pada semua platform dan sistem pengendalian utama. Sebelum melaksanakan kod di bawah, sila pastikan anda mempunyai prasyarat berikut dipasang pada sistem anda.

        * Sistem pengendalian: Microsoft Windows, Linux, MacOS
        * Persekitaran pembangunan: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Dapatkan GroupDocs.Signature for Java terkini daripada [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Potx file
        String filePath = "input.potx";
        // Set up output file
        String outputFilePath = "output.potx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(BarcodeTypes.Codabar);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Potx document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Menandatangani dokumen Potx dengan Barcode Demo Langsung"
    content: |
       Tandatangani fail Potx dengan pelbagai tandatangan sekarang dengan melawati tapak web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demo dalam talian percuma menanti anda.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Codabar Barcode"
          content: |
            Codabar ialah simbol kod bar linear yang direka bentuk untuk dibaca dengan tepat walaupun dicetak pada pencetak dot-matriks untuk borang berbilang bahagian seperti bil udara FedEx dan borang bank darah.
          characterset: |
             Digit berangka (0-9) dan aksara khas $/-:+.
          textcapacity: |
             Tiada sekatan khusus.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAD0AAABGCAYAAAB/h5zrAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAK2SURBVHhe7c9BagQBDAPB/f+nNxDQpUCOfc1MQx8khMGf7wN5n34K79NP4X36KYxPfz6fX0OyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2svfi3/I+/RTeJ9+Cg98+vv9AViQgD/8yuhqAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Tandatangan Barcode lain yang disokong untuk Java"
    content: |
        "Anda juga boleh menandatangani Potx dengan jenis tandatangan lain. Sila lihat senarai di bawah."
    format: 
        
       
back_to_top:
    enable: true
---