---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Interleaved2of5
fileformat: Svg
productName: Java
lang: id
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Svg for Java

############################# Head ############################
head_title: "eSign Svg dokumen dengan Interleaved2of5 Barcode di Java"
head_description: "Buat Interleaved2of5 Tanda Tangan Barcode dan letakkan di dokumen Svg dengan Java menggunakan beberapa baris kode. Gunakan API Tanda Tangan Dokumen GroupDocs untuk menandatangani berbagai format file."

############################# Header ############################
title: "Buat Interleaved2of5 Tanda tangan kode batang untuk dokumen Svg di Java"
description: "eSign dokumen bisnis Svg Anda dengan Interleaved2of5 Barcode. Hasilkan tanda tangan Barcode dengan cepat dan mudah dengan beberapa baris kode untuk menyiapkan opsi penandatanganan."
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
    title: "Tentang GroupDocs.Signature for Java API tanda tangan kode batang."
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) adalah API yang cepat dan mudah untuk mengelola dokumen digital penandatanganan elektronik menggunakan jenis Barcode seperti UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN , ITF14 dan banyak lainnya. Pelanggan dapat dengan mudah membuat Barcode yang menyediakan teks yang diperlukan dan meletakkannya di PDF, Dokumen Microsoft Office Words, buku kerja Microsoft Office Excel, presentasi MS PowerPoint, file Adobe Photoshop dan berbagai format gambar. Barcode yang ditempatkan dalam dokumen dapat diperbarui, dicari, diverifikasi, dihapus, atau dipratinjau. Selain itu, kustomisasi barcode didukung.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Langkah-langkah untuk menandatangani Svg dengan Barcode di Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) memberikan kemampuan untuk menandatangani dokumen Svg dengan Barcode tanda tangan dengan cepat dan mudah.
        
        * Buat instance kelas Signature yang menyediakan file Svg yang seharusnya ditandatangani sebagai jalur atau aliran memori
        * Buat instance kelas SignOptions dan atur semua data yang diminta.
        * Aktifkan metode Signature.Sign() dengan meneruskan file Svg atau aliran memori

    title_right: " Persyaratan sistem"
    content_right: |
        GroupDocs.Signature for Java didukung di semua platform dan sistem operasi utama. Sebelum menjalankan kode di bawah ini, pastikan Anda telah menginstal prasyarat berikut di sistem Anda.

        * Sistem operasi: Microsoft Windows, Linux, MacOS
        * Lingkungan pengembangan: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Dapatkan GroupDocs.Signature for Java terbaru dari [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Svg file
        String filePath = "input.svg";
        // Set up output file
        String outputFilePath = "output.svg";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(BarcodeTypes.Interleaved2of5);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Svg document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Menandatangani dokumen Svg dengan Barcode Demo Langsung"
    content: |
       Tanda tangani file Svg dengan berbagai tanda tangan sekarang juga dengan mengunjungi situs web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demo online gratis menunggu Anda.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Interleaved2of5 Barcode"
          content: |
            Interleaved 2 of 5 (ITF) adalah digit penyandian simbologi barcode dua lebar yang berkesinambungan. Ini digunakan secara komersial pada film 135, untuk barcode ITF-14, dan pada karton beberapa produk, sedangkan produk di dalamnya diberi label UPC atau EAN.
          characterset: |
             Digit numerik (0-9).
          textcapacity: |
             Panjang variabel.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAB8AAACGCAYAAAAlx1GyAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAFdSURBVHhe7Y0xCkJRAMPe/S/9BSFLqHaSN9hAhyzNeS6y+BUWv8LX+DnnPfjkHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3X+K9Z/Ar/Gn+eF5E2tt5Q4JATAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Tanda tangan Barcode lain yang didukung untuk Java"
    content: |
        "Anda juga dapat menandatangani Svg dengan jenis tanda tangan lainnya. Silakan lihat daftarnya di bawah ini."
    format: 
        
       
back_to_top:
    enable: true
---