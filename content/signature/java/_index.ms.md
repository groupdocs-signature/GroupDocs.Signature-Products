---
############################# Static ############################
layout: "landing"
date: 2023-10-23T14:58:09
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: ms
#productCode: java
#otherformats: 
#breadcrumb: Put  signature on  for Java
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: ".NET, Java, Cloud API & Apl Tandatangan Dokumen Dalam Talian"
head_description: "Dapatkan penyelesaian e-tandatangan dokumen semua-dalam-satu untuk .NET, Java dan aplikasi berasaskan awan. Tandatangani format dokumen biasa dalam talian menggunakan ciri seret dan lepas mudah"

############################# Header ############################
title: "Menandatangani dokumen<br>melalui Java API"
description: "Tandatangani dokumen dan imej digital pada mana-mana platform menggunakan API fleksibel dan penyelesaian berasaskan aplikasi kami untuk pengaturcara dan pengguna akhir."
words:
  for: "untuk"

actions:
  main: "Muat Turun Maven Percuma"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-signature/"
  alt: "Pelesenan"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java"
  title: "Bersedia untuk bermula?"
  description: "Cuba ciri GroupDocs.Signature secara percuma atau minta lesen"

release:
  title: "Versi {0} dikeluarkan"
  notes: "Lihat perkara baharu"
  downloads: "Muat turun"

code:
  title: "Tandatangani fail PDF dalam Java"
  more: "Lagi contoh"
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
    
    // Sediakan teks
    TextSignOptions options = new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // Tandatangan dokumen dan simpan ke fail
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature Overview"
  description: "API untuk melaksanakan menandatangani dokumen dan operasi berkaitan dalam aplikasi Java"
  features:
    # feature loop
    - title: "Dokumen perniagaan yang dipertingkatkan dengan tandatangan digital di Jawa"
      content: "Tandatangan pantas dan boleh disesuaikan: GroupDocs.Signature untuk Java menawarkan pelbagai pilihan tandatangan digital untuk PDF, imej dan dokumen Office. Anda boleh menggunakan teks, kod bar, kod QR, sijil digital, gambar atau metadata tersembunyi. Pemprosesan dokumen adalah pantas dan cekap."

    # feature loop
    - title: "Memanipulasi dokumen yang ditandatangani"
      content: "Pemprosesan dokumen lanjutan melibatkan operasi berkuasa pada dokumen yang ditandatangani menggunakan GroupDocs.Signature untuk Java. Anda boleh mencari dan mengesahkan tandatangan yang telah ditambahkan pada dokumen perniagaan menggunakan pelbagai kriteria berguna. Selain itu, anda boleh mengakses maklumat terperinci tentang dokumen atau mendapatkan imej pratonton halamannya."

    # feature loop
    - title: "Pelbagai pilihan keluaran"
      content: "Pilihan tandatangan yang mantap membolehkan anda menyesuaikan output untuk dokumen yang ditandatangani dengan GroupDocs.Signature untuk Java. Anda boleh meletakkan mana-mana tandatangan dengan tepat pada mana-mana halaman dokumen dan mengkonfigurasi penampilannya dalam pelbagai cara. API Java menyokong penyimpanan dokumen perniagaan yang ditandatangani dalam pelbagai format yang disokong dan menyediakan pilihan untuk melindunginya dengan kata laluan."

############################# Platforms ############################
platforms:
  enable: true
  title: "Kemerdekaan platform"
  description: "GroupDocs.Signature untuk Java menyokong sistem pengendalian, rangka kerja dan pengurus pakej berikut"
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
  title: "Format fail yang disokong"
  description: |
    GroupDocs.Signature untuk Java menyokong operasi dengan [format fail](https://docs.groupdocs.com/signature/java/supported-document-formats/) berikut.
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
  title: "GroupDocs.Ciri tandatangan"
  description: "Menandatangani PDF, Dokumen Pejabat dan imej dengan tandatangan digital"

  items:
    # feature loop
    - icon: "sign"
      title: "Menambah Tandatangan"
      content: "Tandatangan dokumen menggunakan pelbagai jenis tandatangan yang disokong dengan meletakkan tandatangan digital dengan tepat pada sebarang kedudukan pada mana-mana halaman."

    # feature loop
    - icon: "custom"
      title: "Menyesuaikan hasil"
      content: "Sesuaikan penampilan tandatangan dengan melaraskan warna, fon, jidar, putaran dan ciri lain untuk mencapai hasil yang diinginkan."

    # feature loop
    - icon: "password"
      title: "Melindungi dokumen dengan kata laluan"
      content: "Untuk banyak jenis dokumen yang disokong, anda boleh melindungi dokumen yang ditandatangani dengan kata laluan."

    # feature loop
    - icon: "protect"
      title: "Mencegah perubahan yang tidak dibenarkan"
      content: "Lindungi dokumen perniagaan penting yang ditandatangani dengan sijil digital daripada pengubahsuaian yang tidak dibenarkan."

    # feature loop
    - icon: "convert"
      title: "Mendapatkan hasil dalam format yang diingini"
      content: "Dapatkan fail hasil yang ditandatangani dengan mudah dalam sebarang format yang disokong. Anda juga boleh menukar dokumen MS Word kepada PDF dengan mudah."

    # feature loop
    - icon: "preview"
      title: "Pratonton dokumen"
      content: "Simpan mana-mana halaman dokumen sebagai imej untuk pemprosesan masa hadapan."

    # feature loop
    - icon: "search"
      title: "Mencari tandatangan"
      content: "Adalah mungkin untuk mendapatkan maklumat tentang tandatangan yang ditambahkan sebelum ini dalam dokumen tertentu."

    # feature loop
    - icon: "validate"
      title: "Mengesahkan dokumen"
      content: "Sahkan ketepatan tandatangan pada mana-mana dokumen yang ditandatangani."

    # feature loop
    - icon: "update"
      title: "Menguruskan tandatangan"
      content: "Sebaik sahaja tandatangan diletakkan pada halaman dokumen, ia boleh dipadamkan, dialihkan atau dikemas kini mengikut keperluan."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Sampel kod"
  description: "Sesetengah menggunakan kes biasa GroupDocs.Signature untuk operasi Java"
  items:
    # code sample loop
    - title: "Tingkatkan dokumen PDF dengan kod QR"
      content: |
        Meningkatkan proses perniagaan dengan menambahkan [QR-codes](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) pada halaman tertentu dokumen PDF boleh menjadi berharga. Terdapat contoh cara menambah kod QR menggunakan GroupDocs.Signature untuk Java.
        {{< landing/code title="Tingkatkan dokumen PDF dengan kod QR">}}
        ```java {style=abap}
        // Muatkan dokumen untuk ditandatangani
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Buat pilihan kod QR dengan teks yang dipratentukan
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Konfigurasikan jenis pengekodan kod QR dan kedudukan pada halaman
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // Tandatangani dokumen dan simpan sebagai fail hasil
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Gunakan tandatangan digital untuk melindungi DOCX"
      content: |
        Anda boleh [Safeguard a Document](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) menggunakan tandatangan peribadi atau korporat yang disimpan sebagai sijil digital. Dokumen yang dicagarkan dengan sijil tidak boleh diubah tanpa membatalkan tandatangan.
        {{< landing/code title="Gunakan tandatangan digital untuk melindungi DOCX">}}
        ```java {style=abap}   
        // Muatkan dokumen untuk ditandatangani secara digital
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Tentukan pilihan tandatangan digital dan berikan laluan ke fail sijil
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // Tetapkan kata laluan sijil
        options.setPassword("1234567890");

        // Tandatangani dokumen dan simpan ke laluan yang dikehendaki
        signature.sign("digitally_signed.pdf", options);
        ```
        {{< /landing/code >}}

---
