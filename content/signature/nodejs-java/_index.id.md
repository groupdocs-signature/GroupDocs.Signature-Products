---
############################# Static ############################
layout: "landing"
date: 2024-04-02T11:33:18
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Node.js
lang: id
#productCode: nodejs-java
#otherformats: 
#breadcrumb: Put  signature on  for JavaScript
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

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
head_title: "API Tanda Tangan Digital Node.js - GroupDocs.Signature"
head_description: "Integrasikan tanda tangan elektronik yang aman di aplikasi Node.js dengan GroupDocs.Signature. Sederhanakan alur kerja penandatanganan dokumen dengan mudah dan efisien."

############################# Header ############################
title: "Menandatangani dokumen<br>dengan API Node.js"
description: "Menandatangani dokumen dan gambar digital di platform apa pun menggunakan API fleksibel dan solusi berbasis aplikasi kami untuk pemrogram dan pengguna akhir."
words:
  for: "untuk"

actions:
  main: "Unduh dari NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "Perizinan"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/nodejs-java/"
  title: "Siap untuk memulai?"
  description: "Coba fitur GroupDocs.Signature secara gratis atau minta lisensi"

release:
  title: "Versi {0} dirilis"
  notes: "Lihat apa yang baru"
  downloads: "Unduhan"

code:
  title: "Menandatangani PDF dengan Node.js"
  more: "Lebih banyak contoh"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.signature"
  content: |
    ```javascript {style=abap}   
    // Pilih dokumen PDF
    let signature = new Signature("sample.pdf");
    
    // Berikan teks
    let options = new TextSignOptions("John Smith");
    
    // Tetapkan warna
    options.ForeColor = Color.Red;
    
    // Tanda tangani dokumen dan simpan ke file
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Ikhtisar Tanda Tangan"
  description: "Pustaka penandatanganan dokumen yang siap digunakan di aplikasi Node.js"
  features:
    # feature loop
    - title: "Solusi Tanda Tangan Digital untuk Dokumen Bisnis dengan Node.js"
      content: "GroupDocs.Signature for Node.js via Java menawarkan serangkaian opsi tanda tangan digital lengkap untuk PDF, dokumen Office, dan gambar. Teks, kode batang, gambar, sertifikat digital, dan metadata tersedia. Pemrosesan dokumen yang efisien memastikan efisiensi."

    # feature loop
    - title: "Manipulasi Tingkat Lanjut atas Dokumen yang Ditandatangani"
      content: "GroupDocs.Signature memberdayakan Anda untuk memproses dokumen yang ditandatangani. Cari dan validasi tanda tangan menggunakan berbagai kriteria. Selain itu, ekstrak informasi dokumen terperinci atau buat gambar pratinjau halaman."

    # feature loop
    - title: "Format Keluaran Beragam"
      content: "Solusi kami memberikan kontrol ekstensif atas format keluaran dokumen yang ditandatangani. Posisikan tanda tangan secara tepat di halaman mana pun dan sesuaikan tampilannya. Simpan dokumen yang ditandatangani dalam berbagai format yang didukung dan amankan secara opsional dengan kata sandi."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independensi platform"
  description: "GroupDocs.Signature for Node.js via Java melakukan pemrosesan dokumen dengan berbagai sistem operasi"
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
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "Format file yang didukung"
  description: |
    GroupDocs.Signature for Node.js via Java memfasilitasi pengoperasian untuk [format file populer](https://docs.groupdocs.com/signature/java/supported-document-formats/).
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
  description: "Tanda tangani PDF, dokumen Office, dan gambar dengan tanda tangan digital"

  items:
    # feature loop
    - icon: "sign"
      title: "Tanda Tangan Bisnis"
      content: "Gunakan berbagai jenis tanda tangan untuk menandatangani dokumen. Tempatkan tanda tangan digital secara tepat di lokasi halaman mana pun."

    # feature loop
    - icon: "custom"
      title: "Menyesuaikan Tampilan Tanda Tangan"
      content: "Sesuaikan aspek visual tanda tangan dengan menyesuaikan warna, font, batas, rotasi, dan lainnya untuk mencapai hasil yang Anda inginkan."

    # feature loop
    - icon: "password"
      title: "Dokumen yang Dilindungi Kata Sandi"
      content: "Untuk banyak format dokumen yang didukung, lindungi dokumen yang ditandatangani dengan kata sandi untuk keamanan tambahan."

    # feature loop
    - icon: "protect"
      title: "Mencegah Modifikasi Tidak Sah"
      content: "Lindungi dokumen bisnis penting yang ditandatangani dengan sertifikat digital dari perubahan yang tidak sah."

    # feature loop
    - icon: "convert"
      title: "Format Keluaran yang Diinginkan"
      content: "Dapatkan dokumen yang ditandatangani dengan mudah dalam format apa pun yang didukung. Konversikan dokumen MS Word ke format PDF dengan mudah."

    # feature loop
    - icon: "preview"
      title: "Pratinjau Dokumen"
      content: "Simpan halaman dokumen individual sebagai gambar untuk kebutuhan masa depan."

    # feature loop
    - icon: "search"
      title: "Pencarian Tanda Tangan"
      content: "Ambil informasi tentang tanda tangan yang ditambahkan sebelumnya dalam dokumen Anda."

    # feature loop
    - icon: "validate"
      title: "Validasi Dokumen"
      content: "Verifikasi keaslian tanda tangan yang disajikan dalam dokumen apa pun."

    # feature loop
    - icon: "update"
      title: "Manajemen Tanda Tangan"
      content: "Hapus, pindahkan, atau ubah tanda tangan apa pun yang ditempatkan pada halaman dokumen mana pun."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Contoh kode"
  description: "Contoh ilustratif yang menampilkan operasi GroupDocs.Signature for Node.js via Java yang umum"
  items:
    # code sample loop
    - title: "Tandai PDF dengan Kode QR"
      content: |
        Memasukkan [barcode](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) ke dalam halaman dokumen PDF tertentu dapat menyederhanakan proses bisnis. Bagian ini memberikan contoh penambahan kode QR menggunakan GroupDocs.Signature for Node.js via Java.
        {{< landing/code title="Cara memasukkan kode QR ke PDF.">}}
        ```javascript {style=abap}
        // Muat dokumen yang akan ditandatangani
        let signature = new Signature("file_to_sign.pdf");
        
        // Buat opsi kode QR dengan teks yang telah ditentukan sebelumnya
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Konfigurasikan jenis dan posisi pengkodean kode QR pada halaman
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // Tanda tangani dokumen dan simpan sebagai file hasil
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Melindungi DOCX dengan Tanda Tangan Digital"
      content: |
        [Lindungi Dokumen Anda](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) dengan tanda tangan berdasarkan sertifikat digital. Tanda tangan digital melindungi dokumen bisnis Anda dari perubahan konten.
        {{< landing/code title="Berikut cara memastikan integritas dokumen.">}}
        ```javascript {style=abap}   
        // Muat dokumen yang akan ditandatangani secara digital
        let signature = new Signature("file_to_sign.docx");
        
        // Tentukan opsi penandatanganan digital dan berikan jalur ke file sertifikat
        let options = new DigitalSignOptions("certificate.pfx");

        // Tetapkan kata sandi sertifikat
        options.Password = "1234567890";

        // Tanda tangani dokumen dan simpan ke jalur yang diinginkan
        signature.Sign("digitally_signed.docx", options);

        ```
        {{< /landing/code >}}

---
