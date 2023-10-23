---
############################# Static ############################
layout: "landing"
date: 2023-10-23T14:58:10
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
platform: "Net"
platform_tag: "net"

############################# Head ############################
head_title: ".NET, Java, Cloud API & Apl Tandatangan Dokumen Dalam Talian"
head_description: "Dapatkan penyelesaian e-tandatangan dokumen semua-dalam-satu untuk .NET, Java dan aplikasi berasaskan awan. Tandatangani format dokumen biasa dalam talian menggunakan ciri seret dan lepas mudah"

############################# Header ############################
title: "Menandatangani dokumen<br>melalui .NET API"
description: "Tandatangani dokumen dan imej digital pada mana-mana platform menggunakan API fleksibel dan penyelesaian berasaskan aplikasi kami untuk pengaturcara dan pengguna akhir."
words:
  for: "untuk"

actions:
  main: "Muat Turun NuGet Percuma"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "Pelesenan"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net"
  title: "Bersedia untuk bermula?"
  description: "Cuba ciri GroupDocs.Signature secara percuma atau minta lesen"

release:
  title: "Versi {0} dikeluarkan"
  notes: "Lihat perkara baharu"
  downloads: "Muat turun"

code:
  title: "Tandatangani fail PDF dalam C#"
  more: "Lagi contoh"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // Pilih dokumen PDF
    using (Signature signature = new Signature("sample.pdf"))
    {
        // Sediakan teks
        var options = new TextSignOptions("John Smith")
        {
            // Tetapkan warna
            ForeColor = Color.Red
        };
        // Tandatangan dokumen dan simpan ke fail
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature Overview"
  description: "API untuk melaksanakan menandatangani dokumen dan operasi berkaitan dalam aplikasi .NET"
  features:
    # feature loop
    - title: "Menambah tandatangan pada dokumen perniagaan dalam C#"
      content: "Menandatangani dokumen: Dengan GroupDocs.Signature untuk .NET, anda boleh menambah pelbagai jenis tandatangan, seperti teks, imej, kod bar dan sijil digital, pada dokumen PDF dan Office. API ini membolehkan anda menandatangani dokumen anda dengan hampir semua jenis data, termasuk metadata tersembunyi."

    # feature loop
    - title: "Memproses dokumen yang ditandatangani"
      content: "Pemprosesan tambahan: Anda boleh melakukan operasi berkuasa pada dokumen yang ditandatangani menggunakan GroupDocs.Signature. Ini termasuk mencari tandatangan sedia ada dalam dokumen perniagaan dan mengesahkannya menggunakan kriteria tertentu. Selain itu, anda boleh mendapatkan semula maklumat dokumen dan halaman pratonton melalui .NET API ini."

    # feature loop
    - title: "Menyesuaikan hasil"
      content: "GroupDocs.Signature untuk .NET menawarkan pilihan penyesuaian yang meluas. Anda boleh meletakkan tandatangan dengan tepat di mana-mana sahaja pada halaman dokumen dan melaraskan penampilannya menggunakan pelbagai tetapan. Tambahan pula, API ini menyokong penyimpanan dokumen yang diproses dalam pelbagai format yang disokong."

############################# Platforms ############################
platforms:
  enable: true
  title: "Kemerdekaan platform"
  description: "GroupDocs.Signature untuk .NET menyokong sistem pengendalian, rangka kerja dan pengurus pakej berikut"
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
    GroupDocs.Signature untuk .NET menyokong operasi dengan [format fail](https://docs.groupdocs.com/signature/net/supported-document-formats/) berikut.
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
  description: "Menandatangani PDF, Dokumen Pejabat dan Imej dengan pantas dan tepat"

  items:
    # feature loop
    - icon: "sign"
      title: "Menandatangani dokumen"
      content: "Tambahkan satu atau berbilang jenis tandatangan yang disokong dengan tepat pada mana-mana kedudukan tertentu pada dokumen perniagaan."

    # feature loop
    - icon: "custom"
      title: "Sesuaikan tandatangan"
      content: "Gunakan ciri seperti warna, fon, sempadan, putaran, dsb., untuk mengkonfigurasi penampilan tandatangan."

    # feature loop
    - icon: "password"
      title: "Perlindungan kata laluan dokumen"
      content: "Lindungi jenis dokumen tertentu dengan menetapkan kata laluan selepas menandatangani."

    # feature loop
    - icon: "protect"
      title: "Perlindungan daripada perubahan"
      content: "Cegah perubahan pada dokumen perniagaan penting selepas melampirkan tandatangan dengan sijil digital."

    # feature loop
    - icon: "convert"
      title: "Tukar fail yang ditandatangani kepada format lain"
      content: "Tukar fail yang ditandatangani kepada format yang diingini, seperti menyimpan dokumen Word sebagai PDF."

    # feature loop
    - icon: "preview"
      title: "Ekstrak pratonton halaman"
      content: "Ekstrak halaman daripada dokumen yang ditandatangani sebagai imej individu untuk pemprosesan masa hadapan."

    # feature loop
    - icon: "search"
      title: "Carian tandatangan dalam dokumen"
      content: "Dapatkan maklumat tentang tandatangan yang ditambahkan sebelum ini dalam dokumen tertentu."

    # feature loop
    - icon: "validate"
      title: "Mengesahkan dokumen yang ditandatangani"
      content: "Sahkan tandatangan dokumen yang betul menggunakan ciri pengesahan."

    # feature loop
    - icon: "update"
      title: "Kemas kini atau padamkan tandatangan"
      content: "Letakkan semula tandatangan tertentu dengan mudah pada halaman, ubah suai teksnya atau padamkannya tanpa sebarang masalah."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Sampel kod"
  description: "Sesetengah kes menggunakan GroupDocs.Signature untuk operasi .NET biasa"
  items:
    # code sample loop
    - title: "Tambahkan kod QR pada PDF"
      content: |
        Menambah [QR-codes](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) pada halaman tertentu dokumen PDF boleh meningkatkan proses perniagaan. Di bawah ialah contoh cara menambah kod QR menggunakan GroupDocs.Signature.
        {{< landing/code title="Bagaimana untuk meletakkan kod QR ke PDF.">}}
        ```csharp {style=abap}
        // Muatkan dokumen untuk ditandatangani
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Buat pilihan kod QR dengan teks yang dipratentukan
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // Konfigurasikan jenis pengekodan kod QR dan kedudukan pada halaman
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // Tandatangani dokumen dan simpan sebagai fail hasil
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Melindungi dokumen DOCX menggunakan sijil digital"
      content: |
        Anda boleh [Melindungi Dokumen](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/) menggunakan tandatangan peribadi atau korporat yang disimpan sebagai sijil digital. Dokumen yang dilindungi sedemikian tidak boleh diubah suai tanpa membatalkan tandatangan.
        {{< landing/code title="Berikut ialah cara memastikan integriti dokumen.">}}
        ```csharp {style=abap}   
        // Muatkan dokumen untuk ditandatangani secara digital
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Tentukan pilihan tandatangan digital dan berikan laluan ke fail sijil
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // Tetapkan kata laluan sijil
                Password = "1234567890"
            };
            // Tandatangani dokumen dan simpan ke laluan yang dikehendaki
            signature.Sign("digitally_signed.pdf", options);
        }
        ```
        {{< /landing/code >}}

---
