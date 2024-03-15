---
############################# Static ############################
layout: "landing"
date: 2024-03-15T20:32:51
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Node.js
lang: ms
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
head_title: "API Tandatangan Digital Node.js - GroupDocs.Signature"
head_description: "Sepadukan e-tandatangan selamat dalam apl Node.js dengan GroupDocs.Signature. Perkemas aliran kerja menandatangani dokumen dengan mudah dan cekap."

############################# Header ############################
title: "Menandatangani dokumen<br>dengan API Node.js"
description: "Tandatangani dokumen dan imej digital pada mana-mana platform menggunakan API fleksibel dan penyelesaian berasaskan aplikasi kami untuk pengaturcara dan pengguna akhir."
words:
  for: "untuk"

actions:
  main: "Muat turun daripada NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "Pelesenan"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "Bersedia untuk bermula?"
  description: "Cuba ciri GroupDocs.Signature secara percuma atau minta lesen"

release:
  title: "Versi {0} dikeluarkan"
  notes: "Lihat perkara baharu"
  downloads: "Muat turun"

code:
  title: "Menandatangani PDF oleh Node.js"
  more: "Lagi contoh"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.signature"
  content: |
    ```javascript {style=abap}   
    // Pilih dokumen PDF
    let signature = new Signature("sample.pdf");
    
    // Sediakan teks
    let options = new TextSignOptions("John Smith");
    
    // Tetapkan warna
    options.ForeColor = Color.Red;
    
    // Tandatangan dokumen dan simpan ke fail
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature Overview"
  description: "Pustaka menandatangani dokumen yang sedia untuk digunakan dalam aplikasi Node.js"
  features:
    # feature loop
    - title: "Penyelesaian Tandatangan Digital untuk Dokumen Perniagaan dengan Node.js"
      content: "GroupDocs.Signature for Node.js via Java menawarkan set komprehensif pilihan tandatangan digital untuk PDF, dokumen Office dan imej. Teks, kod bar, imej, sijil digital dan metadata tersedia. Pemprosesan dokumen yang diperkemas memastikan kecekapan."

    # feature loop
    - title: "Manipulasi Lanjutan Dokumen Ditandatangani"
      content: "GroupDocs.Signature memberi anda kuasa untuk memproses dokumen yang ditandatangani. Cari dan sahkan tandatangan menggunakan pelbagai kriteria. Selain itu, ekstrak maklumat dokumen terperinci atau hasilkan imej pratonton halaman."

    # feature loop
    - title: "Format Output Pelbagai"
      content: "Penyelesaian kami menyediakan kawalan yang meluas ke atas format output dokumen yang ditandatangani. Letakkan tandatangan dengan tepat pada mana-mana halaman dan sesuaikan penampilannya. Simpan dokumen yang ditandatangani dalam pelbagai format yang disokong dan selamatkannya dengan kata laluan secara pilihan."

############################# Platforms ############################
platforms:
  enable: true
  title: "Kemerdekaan platform"
  description: "GroupDocs.Signature for Node.js via Java melaksanakan pemprosesan dokumen dengan pelbagai sistem pengendalian"
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
  title: "Format fail yang disokong"
  description: |
    GroupDocs.Signature for Node.js via Java memudahkan operasi untuk [format fail popular](https://docs.groupdocs.com/signature/java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Format Microsoft Office
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Imej & Format Lain
        * **Mudah alih:** PDF
        * **Imej:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Format pejabat lain:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Format lain
        * **Web:** HTML, MHTML
        * **Arkib:** ZIP, TAR, 7Z
        * **Sijil:** PFX

############################# Features ############################
features:
  enable: true
  title: "Ciri-ciri GroupDocs.Signature"
  description: "Tandatangani PDF, dokumen Pejabat dan imej dengan tandatangan digital"

  items:
    # feature loop
    - icon: "sign"
      title: "Tandatangan Perniagaan"
      content: "Gunakan pelbagai jenis tandatangan untuk menandatangani dokumen. Letakkan tandatangan digital dengan tepat pada mana-mana lokasi halaman."

    # feature loop
    - icon: "custom"
      title: "Menyesuaikan Penampilan Tandatangan"
      content: "Sesuaikan aspek visual tandatangan dengan melaraskan warna, fon, jidar, putaran dan banyak lagi untuk mencapai hasil yang anda inginkan."

    # feature loop
    - icon: "password"
      title: "Dokumen Dilindungi Kata Laluan"
      content: "Untuk kebanyakan format dokumen yang disokong, lindungi dokumen yang ditandatangani dengan kata laluan untuk keselamatan tambahan."

    # feature loop
    - icon: "protect"
      title: "Mencegah Pengubahsuaian Tanpa Kebenaran"
      content: "Lindungi dokumen perniagaan penting yang ditandatangani dengan sijil digital daripada perubahan yang tidak dibenarkan."

    # feature loop
    - icon: "convert"
      title: "Format Output yang Diingini"
      content: "Dapatkan dokumen yang ditandatangani dengan mudah dalam sebarang format yang disokong. Tukar dokumen MS Word kepada format PDF dengan mudah."

    # feature loop
    - icon: "preview"
      title: "Pratonton Dokumen"
      content: "Simpan halaman dokumen individu sebagai imej untuk keperluan masa hadapan."

    # feature loop
    - icon: "search"
      title: "Carian Tandatangan"
      content: "Dapatkan maklumat tentang tandatangan yang ditambahkan sebelum ini dalam dokumen anda."

    # feature loop
    - icon: "validate"
      title: "Pengesahan Dokumen"
      content: "Sahkan ketulenan tandatangan yang dibentangkan dalam mana-mana dokumen."

    # feature loop
    - icon: "update"
      title: "Pengurusan Tandatangan"
      content: "Padam, pindahkan atau ubah suai sebarang tandatangan yang diletakkan pada mana-mana halaman dokumen."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Sampel kod"
  description: "Contoh ilustrasi yang mempamerkan operasi biasa GroupDocs.Signature for Node.js via Java."
  items:
    # code sample loop
    - title: "Tandai PDF dengan Kod QR"
      content: |
        Menggabungkan [kod bar](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) ke dalam halaman dokumen PDF tertentu boleh menyelaraskan proses perniagaan. Bahagian ini menyediakan contoh menambah kod QR menggunakan GroupDocs.Signature for Node.js via Java.
        {{< landing/code title="Bagaimana untuk meletakkan kod QR ke PDF.">}}
        ```javascript {style=abap}
        // Muatkan dokumen untuk ditandatangani
        let signature = new Signature("file_to_sign.pdf");
        
        // Buat pilihan kod QR dengan teks yang dipratentukan
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Konfigurasikan jenis pengekodan kod QR dan kedudukan pada halaman
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // Tandatangani dokumen dan simpan sebagai fail hasil
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Melindungi DOCX dengan Tandatangan Digital"
      content: |
        [Lindungi Dokumen anda](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) dengan tandatangan berdasarkan sijil digital. Tandatangan digital melindungi dokumen perniagaan anda daripada perubahan kandungan.
        {{< landing/code title="Berikut ialah cara memastikan integriti dokumen.">}}
        ```javascript {style=abap}   
        // Muatkan dokumen untuk ditandatangani secara digital
        let signature = new Signature("file_to_sign.docx");
        
        // Tentukan pilihan tandatangan digital dan berikan laluan ke fail sijil
        let options = new DigitalSignOptions("certificate.pfx");

        // Tetapkan kata laluan sijil
        options.Password = "1234567890";

        // Tandatangani dokumen dan simpan ke laluan yang dikehendaki
        signature.Sign("digitally_signed.docx", options);

        ```
        {{< /landing/code >}}

---
