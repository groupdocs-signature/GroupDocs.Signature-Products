---
############################# Static ############################
layout: "landing"
date: 2023-09-14T19:07:22
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
platform: "Net"
platform_tag: "net"

############################# Head ############################
head_title: ".NET, Java, Cloud API & Aplikasi Tanda Tangan Dokumen Online"
head_description: "Dapatkan solusi e-signature dokumen all-in-one untuk .NET, Java, dan aplikasi berbasis cloud. Tandatangani format dokumen umum secara online menggunakan fitur drag and drop sederhana"

############################# Header ############################
title: "Menandatangani dokumen<br>melalui .NET API"
description: "Menandatangani dokumen dan gambar digital di platform apa pun menggunakan API fleksibel dan solusi berbasis aplikasi kami untuk pemrogram dan pengguna akhir."
words:
  for: "untuk"

actions:
  main: "Unduh NuGet Gratis"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "Perizinan"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net"
  title: "Siap untuk memulai?"
  description: "Coba fitur GroupDocs.Signature secara gratis atau minta lisensi"

release:
  title: "Versi {0} dirilis"
  notes: "Lihat apa yang baru"
  downloads: "Unduhan"

code:
  title: "Menandatangani file PDF di C#"
  more: "Lebih banyak contoh"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // Pilih dokumen PDF
    using (Signature signature = new Signature("sample.pdf"))
    {
        // Berikan teks
        var options = new TextSignOptions("John Smith")
        {
            // Tetapkan warna
            ForeColor = Color.Red
        };
        // Tanda tangani dokumen dan simpan ke file
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Ikhtisar Tanda Tangan"
  description: "API untuk melakukan penandatanganan dokumen dan operasi terkait dalam aplikasi .NET"
  features:
    # feature loop
    - title: "Menambahkan tanda tangan ke dokumen bisnis di C#"
      content: "Penandatanganan dokumen: Dengan GroupDocs.Signature untuk .NET, Anda dapat menambahkan berbagai jenis tanda tangan, seperti teks, gambar, kode batang, dan sertifikat digital, ke dokumen PDF dan Office. API ini memungkinkan Anda menandatangani dokumen dengan hampir semua tipe data, termasuk metadata tersembunyi."

    # feature loop
    - title: "Memproses dokumen yang ditandatangani"
      content: "Pemrosesan tambahan: Anda dapat melakukan operasi canggih pada dokumen yang ditandatangani menggunakan GroupDocs.Signature. Ini termasuk mencari tanda tangan yang ada dalam dokumen bisnis dan memverifikasinya menggunakan kriteria tertentu. Selain itu, Anda dapat mengambil informasi dokumen dan melihat halaman pratinjau melalui .NET API ini."

    # feature loop
    - title: "Menyesuaikan hasil"
      content: "GroupDocs.Signature untuk .NET menawarkan opsi penyesuaian yang luas. Anda dapat secara tepat memposisikan tanda tangan di mana saja pada halaman dokumen dan menyesuaikan tampilannya menggunakan berbagai pengaturan. Selain itu, API ini mendukung penyimpanan dokumen yang diproses dalam berbagai format yang didukung."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independensi platform"
  description: "GroupDocs.Signature untuk .NET mendukung sistem operasi, kerangka kerja, dan manajer paket berikut"
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
    GroupDocs.Signature untuk .NET mendukung operasi dengan [format file](https://docs.groupdocs.com/signature/net/supported-document-formats/) berikut.
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
  description: "Menandatangani PDF, Dokumen Office, dan Gambar dengan cepat dan akurat"

  items:
    # feature loop
    - icon: "sign"
      title: "Penandatanganan dokumen"
      content: "Tambahkan satu atau beberapa jenis tanda tangan yang didukung secara akurat pada posisi tertentu pada dokumen bisnis."

    # feature loop
    - icon: "custom"
      title: "Sesuaikan tanda tangan"
      content: "Manfaatkan fitur seperti warna, font, batas, rotasi, dll., untuk mengonfigurasi tampilan tanda tangan."

    # feature loop
    - icon: "password"
      title: "Perlindungan kata sandi dokumen"
      content: "Amankan jenis dokumen tertentu dengan menetapkan kata sandi setelah penandatanganan."

    # feature loop
    - icon: "protect"
      title: "Perlindungan dari perubahan"
      content: "Cegah perubahan pada dokumen bisnis penting setelah menambahkan tanda tangan dengan sertifikat digital."

    # feature loop
    - icon: "convert"
      title: "Konversikan file yang ditandatangani ke format lain"
      content: "Konversikan file yang ditandatangani ke format yang diinginkan, seperti menyimpan dokumen Word sebagai PDF."

    # feature loop
    - icon: "preview"
      title: "Ekstrak pratinjau halaman"
      content: "Ekstrak halaman dari dokumen yang ditandatangani sebagai gambar individual untuk diproses di masa mendatang."

    # feature loop
    - icon: "search"
      title: "Pencarian tanda tangan dalam dokumen"
      content: "Ambil informasi tentang tanda tangan yang ditambahkan sebelumnya dalam dokumen tertentu."

    # feature loop
    - icon: "validate"
      title: "Validasi dokumen yang ditandatangani"
      content: "Verifikasi penandatanganan dokumen yang benar menggunakan fitur validasi."

    # feature loop
    - icon: "update"
      title: "Perbarui atau hapus tanda tangan"
      content: "Ubah posisi tanda tangan tertentu dengan mudah di halaman, ubah teksnya, atau hapus tanpa masalah apa pun."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Contoh kode"
  description: "Beberapa kasus penggunaan GroupDocs.Signature untuk operasi .NET"
  items:
    # code sample loop
    - title: "Tambahkan kode QR ke PDF"
      content: |
        Menambahkan [kode QR](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) ke halaman tertentu dokumen PDF dapat meningkatkan proses bisnis. Di bawah ini adalah contoh cara menambahkan kode QR menggunakan GroupDocs.Signature.
        {{< landing/code title="Cara memasukkan kode QR ke PDF.">}}
        ```csharp {style=abap}
        // Muat dokumen yang akan ditandatangani
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Buat opsi kode QR dengan teks yang telah ditentukan sebelumnya
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // Konfigurasikan jenis dan posisi pengkodean kode QR pada halaman
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // Tanda tangani dokumen dan simpan sebagai file hasil
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Melindungi dokumen DOCX menggunakan sertifikat digital"
      content: |
        Anda dapat [Melindungi Dokumen](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/) menggunakan tanda tangan pribadi atau perusahaan yang disimpan sebagai sertifikat digital. Dokumen yang dilindungi tersebut tidak dapat diubah tanpa membatalkan tanda tangannya.
        {{< landing/code title="Berikut cara memastikan integritas dokumen.">}}
        ```csharp {style=abap}   
        // Muat dokumen yang akan ditandatangani secara digital
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Tentukan opsi penandatanganan digital dan berikan jalur ke file sertifikat
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // Tetapkan kata sandi sertifikat
                Password = "1234567890"
            };
            // Tanda tangani dokumen dan simpan ke jalur yang diinginkan
            signature.Sign("digitally_signed.pdf", options);
        }
        ```
        {{< /landing/code >}}

---
