---
############################# Static ############################
layout: "landing"
date: 2024-03-05T15:50:57
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: id
#productCode: java
#otherformats: 
#breadcrumb: Put  signature on  for Java
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: ".NET, Java, Cloud API & Aplikasi Tanda Tangan Dokumen Online"
head_description: "Dapatkan solusi e-signature dokumen all-in-one untuk .NET, Java, dan aplikasi berbasis cloud. Tandatangani format dokumen umum secara online menggunakan fitur drag and drop sederhana"

############################# Header ############################
title: "Menandatangani dokumen<br>melalui API Java"
description: "Menandatangani dokumen dan gambar digital di platform apa pun menggunakan API fleksibel dan solusi berbasis aplikasi kami untuk pemrogram dan pengguna akhir."
words:
  for: "untuk"

actions:
  main: "Unduhan Maven Gratis"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-signature/"
  alt: "Perizinan"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java"
  title: "Siap untuk memulai?"
  description: "Coba fitur GroupDocs.Signature secara gratis atau minta lisensi"

release:
  title: "Versi {0} dirilis"
  notes: "Lihat apa yang baru"
  downloads: "Unduhan"

code:
  title: "Tanda tangani file PDF di Java"
  more: "Lebih banyak contoh"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-signature</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Pilih dokumen PDF
    Signature signature = new Signature("sample.pdf");
    
    // Berikan teks
    TextSignOptions options = 
        new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // Tanda tangani dokumen dan simpan ke file
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Ikhtisar Tanda Tangan"
  description: "API untuk melakukan penandatanganan dokumen dan operasi terkait dalam aplikasi Java"
  features:
    # feature loop
    - title: "Peningkatan dokumen bisnis dengan tanda tangan digital di Java"
      content: "Penandatanganan yang cepat dan dapat disesuaikan: GroupDocs.Signature untuk Java menawarkan beragam opsi tanda tangan digital untuk PDF, gambar, dan dokumen Office. Anda dapat menggunakan teks, kode batang, kode QR, sertifikat digital, gambar, atau metadata tersembunyi. Pemrosesan dokumen cepat dan efisien."

    # feature loop
    - title: "Memanipulasi dokumen yang ditandatangani"
      content: "Pemrosesan dokumen tingkat lanjut melibatkan operasi yang kuat pada dokumen yang ditandatangani menggunakan GroupDocs.Signature untuk Java. Anda dapat mencari dan memvalidasi tanda tangan yang telah ditambahkan ke dokumen bisnis menggunakan berbagai kriteria yang berguna. Selain itu, Anda dapat mengakses informasi rinci tentang dokumen atau mendapatkan gambar pratinjau halamannya."

    # feature loop
    - title: "Berbagai pilihan keluaran"
      content: "Opsi penandatanganan yang kuat memungkinkan Anda menyesuaikan output untuk dokumen yang ditandatangani dengan GroupDocs.Signature untuk Java. Anda dapat secara tepat memposisikan tanda tangan apa pun di halaman dokumen mana pun dan mengonfigurasi tampilannya dengan berbagai cara. Java API mendukung penyimpanan dokumen bisnis yang ditandatangani dalam berbagai format yang didukung dan menyediakan opsi untuk mengamankannya dengan kata sandi."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independensi platform"
  description: "GroupDocs.Signature untuk Java mendukung sistem operasi, kerangka kerja, dan manajer paket berikut"
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "Format file yang didukung"
  description: |
    GroupDocs.Signature untuk Java mendukung operasi dengan [format file](https://docs.groupdocs.com/signature/java/supported-document-formats/) berikut.
  groups:
    # group loop
    - color: "green"
      content: |
        ### format Microsoft Office
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Gambar & Format Lainnya
        * **Portabel:** PDF
        * **Gambar-gambar:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Format kantor lainnya:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Format lainnya
        * **jaring:** HTML, MHTML
        * **Arsip:** ZIP, TAR, 7Z
        * **Sertifikat:** PFX

############################# Features ############################
features:
  enable: true
  title: "Fitur GroupDocs.Signature"
  description: "Menandatangani PDF, Dokumen Office, dan gambar dengan tanda tangan digital"

  items:
    # feature loop
    - icon: "sign"
      title: "Menambahkan Tanda Tangan"
      content: "Tanda tangani dokumen menggunakan berbagai jenis tanda tangan yang didukung dengan menempatkan tanda tangan digital secara tepat di posisi mana pun di halaman mana pun."

    # feature loop
    - icon: "custom"
      title: "Menyesuaikan hasil"
      content: "Sesuaikan tampilan tanda tangan dengan menyesuaikan warna, font, batas, rotasi, dan fitur lainnya untuk mencapai hasil yang diinginkan."

    # feature loop
    - icon: "password"
      title: "Mengamankan dokumen dengan kata sandi"
      content: "Untuk banyak tipe dokumen yang didukung, Anda dapat melindungi dokumen yang ditandatangani dengan kata sandi."

    # feature loop
    - icon: "protect"
      title: "Mencegah perubahan yang tidak sah"
      content: "Lindungi dokumen bisnis penting yang ditandatangani dengan sertifikat digital dari modifikasi yang tidak sah."

    # feature loop
    - icon: "convert"
      title: "Memperoleh hasil dalam format yang diinginkan"
      content: "Dapatkan file hasil yang ditandatangani dengan mudah dalam format apa pun yang didukung. Anda juga dapat mengonversi dokumen MS Word ke PDF dengan mudah."

    # feature loop
    - icon: "preview"
      title: "Pratinjau dokumen"
      content: "Simpan halaman mana pun dari dokumen sebagai gambar untuk diproses di masa mendatang."

    # feature loop
    - icon: "search"
      title: "Mencari tanda tangan"
      content: "Dimungkinkan untuk mendapatkan informasi tentang tanda tangan yang ditambahkan sebelumnya dalam dokumen tertentu."

    # feature loop
    - icon: "validate"
      title: "Memvalidasi dokumen"
      content: "Validasi kebenaran tanda tangan pada setiap dokumen yang ditandatangani."

    # feature loop
    - icon: "update"
      title: "Mengelola tanda tangan"
      content: "Setelah tanda tangan ditempatkan pada halaman dokumen, tanda tangan tersebut dapat dihapus, dipindahkan, atau diperbarui sesuai kebutuhan."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Contoh kode"
  description: "Beberapa kasus penggunaan GroupDocs.Signature khas untuk operasi Java"
  items:
    # code sample loop
    - title: "Tingkatkan dokumen PDF dengan kode QR"
      content: |
        Meningkatkan proses bisnis dengan menambahkan [kode QR](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) ke halaman tertentu dokumen PDF dapat bermanfaat. Ada contoh cara menambahkan kode QR menggunakan GroupDocs.Signature untuk Java.
        {{< landing/code title="Tingkatkan dokumen PDF dengan kode QR">}}
        ```java {style=abap}
        // Muat dokumen yang akan ditandatangani
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Buat opsi kode QR dengan teks yang telah ditentukan sebelumnya
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Konfigurasikan jenis dan posisi pengkodean kode QR pada halaman
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // Tanda tangani dokumen dan simpan sebagai file hasil
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Gunakan tanda tangan digital untuk melindungi DOCX"
      content: |
        Anda dapat [Melindungi Dokumen](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) menggunakan tanda tangan pribadi atau perusahaan yang disimpan sebagai sertifikat digital. Dokumen yang diamankan dengan sertifikat tidak dapat diubah tanpa membatalkan tanda tangannya.
        {{< landing/code title="Gunakan tanda tangan digital untuk melindungi DOCX">}}
        ```java {style=abap}   
        // Muat dokumen yang akan ditandatangani secara digital
        Signature signature = new Signature("file_to_sign.docx");
        
        // Tentukan opsi penandatanganan digital dan berikan jalur ke file sertifikat
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // Tetapkan kata sandi sertifikat
        options.setPassword("1234567890");

        // Tanda tangani dokumen dan simpan ke jalur yang diinginkan
        signature.sign("digitally_signed.docx", options);
        ```
        {{< /landing/code >}}

---
