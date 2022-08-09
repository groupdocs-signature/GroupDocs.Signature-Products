---
layout: "auto-gen"
date: 2022-07-07T12:44:18+03:00
draft: false

head_title: "Hasilkan AZTEC QR-code dan Masuk File PPS di .NET | Menandatangani Dokumen"
head_description: "Tanda tangani file PPS dengan tanda tangan kode QR AZTEC di .NET - tambahkan kode batang ke dokumen bisnis populer dan format file gambar."

title: "Tambahkan AZTEC kode QR ke File PPS di C#"
description: "Tandatangani file PPS Anda menggunakan kode QR AZTEC. Memanipulasi properti tanda tangan dan mengatur opsi penandatanganan lanjutan dalam dokumen yang sesuai dengan kebutuhan Anda."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Unduh Uji Coba Gratis"
    link: "https://downloads.groupdocs.com/signature/net"

submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"

    middle:
        button:

            - link: "https://apireference.groupdocs.com/signature/net"
              text: "Referensi API"

            - link: "https://github.com/groupdocs-signature"
              text: "Contoh Kode"

            - link: "https://products.groupdocs.app/signature/family"
              text: "Demo Langsung"

            - link: "https://purchase.groupdocs.com/pricing/signature/net"
              text: "Harga"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/net"
        link_buy: "https://purchase.groupdocs.com"

about:
    enable: true
    title: "Tentang GroupDocs.Signature untuk .NET API"
    content: |
        [GroupDocs.Signature for .NET](/id/signature/net/) adalah .NET API asli untuk menandatangani dokumen digital secara elektronik menggunakan berbagai jenis tanda tangan seperti teks, gambar, kode batang, stempel, bidang formulir, kode QR, dan metadata. Pengguna dapat menambahkan, mengedit, memverifikasi, menghapus, dan mencari tanda tangan digital dalam PDF, Microsoft Word, lembar kerja Excel, presentasi PowerPoint, Adobe Photoshop, metafile, dan format file gambar dengan dukungan tambahan untuk menyesuaikan properti tanda tangan sesuai kebutuhan.

steps:
    enable: true
    title_left: "Cara Menghasilkan AZTEC QR-code untuk file PPS di C#"
    content_left: |
        [GroupDocs.Signature](/id/signature/net/) memudahkan pengembang .NET untuk menambahkan kode batang AZTEC ke file PPS dalam aplikasi mereka dengan menerapkan beberapa langkah mudah.

        * Buat instance baru kelas Signature dan berikan jalur dokumen PPS sumber sebagai parameter konstruktor.
        * Buat instance objek QrCodeSignOptions dengan teks yang diperlukan dan setel properti EncodeType ke AZTEC.
        * Metode Tanda Panggil kelas Tanda Tangan dan berikan nama file PPS keluaran dengan QrCodeSignOptions ke dalamnya.
        * Analisis hasil SignResult untuk memeriksa tanda tangan yang baru dibuat jika diperlukan.
        
    title_right: "Persyaratan sistem"
    content_right: |
        GroupDocs.Signature untuk .NET API didukung di semua platform dan sistem operasi utama. Sebelum menjalankan kode di bawah ini, pastikan Anda telah menginstal prasyarat berikut di sistem Anda.

        * Sistem Operasi: Microsoft Windows, Linux, MacOS
        * Lingkungan Pengembangan: Visual Studio, Xamarin, MonoDevelop
        * Kerangka: .NET Framework, .NET Standard, .NET Core, Mono
        * Unduh versi terbaru GroupDocs.Signature untuk .NET dari [NuGet](https://www.nuget.org/packages/groupdocs.signature)
        
    code: |
        ```cs
        using (Signature signature = new Signature("sample.pps"))
        {
            // Inisialisasi opsi kode-qr dengan teks yang telah ditentukan
            QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith")
            {
                // atur jenis penyandian QRCode
                EncodeType = QrCodeTypes.QR,
                
                // atur posisi tanda tangan
                Left = 50,
                Top = 150,
                Width = 200,
                Height = 50
            };

            // Masuk file PPS dan simpan hasilnya 
            signature.Sign("signed.pps", options);
        }
        ```
        
demos:
    enable: true
    title: "Demo Langsung - Aplikasi Online untuk Menghasilkan AZTEC Tanda Tangan kode QR"
    content: |
        Tambahkan AZTEC qr-codes ke file PPS sekarang juga dengan mengunjungi situs web [GroupDocs.Signature](https://products.groupdocs.app/signature/family). Demo langsung memiliki manfaat sebagai berikut.
        
about_formats:
    enable: true
    format:
        - icon: "fas fa-qrcode"
          title: "Tentang AZTEC kode QR"
          content: |
            Kode AZTEC adalah simbologi matriks tujuan umum dua dimensi (2-D) yang dirancang untuk memiliki akurasi lebih tinggi daripada simbologi 2-D lainnya. Simbol Kode AZTEC dapat mengkodekan hingga 3.832 digit angka; 3.067 karakter alfabet; atau 1.914 byte data. Kode AZTEC ditemukan oleh Andrew Longacre, Jr. dan Robert Hussey pada tahun 1995. Kode tersebut diterbitkan oleh AIM, Inc. pada tahun 1997. Meskipun kode AZTEC telah dipatenkan, paten tersebut secara resmi dijadikan domain publik. Kode AZTEC juga diterbitkan sebagai standar ISO/IEC 24778:2008. Dinamakan berdasarkan kemiripan pola penemu pusat dengan piramida AZTEC, kode AZTEC berpotensi menggunakan lebih sedikit ruang daripada kode batang matriks lainnya karena tidak memerlukan zona tenang kosong di sekitarnya.

          link: ""

more_formats:
    enable: true
    title: "Menandatangani Format File Lain dengan AZTEC QR-code menggunakan C#"
    content: |
        .NET .NET qr-code signatures management API untuk dokumen dan gambar. Tambahkan tanda tangan kode qr ke beberapa format file populer seperti yang dinyatakan di bawah ini.
    format: 
        - name: "Tambahkan tanda tangan elektronik ke PDF"
          link: "/signature/net/add/qrcode/pdf/aztec/"
          description: "Format Dokumen Portabel Adobe"

        - name: "Tambahkan tanda tangan elektronik ke DOC"
          link: "/signature/net/add/qrcode/doc/aztec/"
          description: "Dokumen Microsoft Word"

        - name: "Tambahkan tanda tangan elektronik ke DOCM"
          link: "/signature/net/add/qrcode/docm/aztec/"
          description: "Dokumen Berkemampuan Makro Microsoft Word"

        - name: "Tambahkan tanda tangan elektronik ke DOCX"
          link: "/signature/net/add/qrcode/docx/aztec/"
          description: "Microsoft Word Buka Dokumen XML"

        - name: "Tambahkan tanda tangan elektronik ke DOT"
          link: "/signature/net/add/qrcode/dot/aztec/"
          description: "Templat Dokumen Microsoft Word"

        - name: "Tambahkan tanda tangan elektronik ke DOTX"
          link: "/signature/net/add/qrcode/dotx/aztec/"
          description: "Templat Dokumen XML Word Terbuka"

        - name: "Tambahkan tanda tangan elektronik ke DOTM"
          link: "/signature/net/add/qrcode/dotm/aztec/"
          description: "Templat Microsoft Word Macro-Enabled"       

        - name: "Tambahkan tanda tangan elektronik ke ODT"
          link: "/signature/net/add/qrcode/odt/aztec/"
          description: "Buka Teks Dokumen"

        - name: "Tambahkan tanda tangan elektronik ke OTT"
          link: "/signature/net/add/qrcode/ott/aztec/"
          description: "Templat Teks OpenDocument"

        - name: "Tambahkan tanda tangan elektronik ke XLS"
          link: "/signature/net/add/qrcode/xls/aztec/"
          description: "Format File Biner Microsoft Excel"

        - name: "Tambahkan tanda tangan elektronik ke XLSX"
          link: "/signature/net/add/qrcode/xlsx/aztec/"
          description: "Microsoft Excel Buka XML Spreadsheet"

        - name: "Tambahkan tanda tangan elektronik ke XLSM"
          link: "/signature/net/add/qrcode/xlsm/aztec/"
          description: "Spreadsheet Berkemampuan Makro Microsoft Excel"

        - name: "Tambahkan tanda tangan elektronik ke XLSB"
          link: "/signature/net/add/qrcode/xlsb/aztec/"
          description: "Lembar Kerja Biner Microsoft Excel"

        - name: "Tambahkan tanda tangan elektronik ke XLTX"
          link: "/signature/net/add/qrcode/xltx/aztec/"
          description: "Templat Microsoft Excel"

        - name: "Tambahkan tanda tangan elektronik ke XLTM"
          link: "/signature/net/add/qrcode/xltm/aztec/"
          description: "Templat berkemampuan makro Microsoft Excel"

        - name: "Tambahkan tanda tangan elektronik ke ODS"
          link: "/signature/net/add/qrcode/ods/aztec/"
          description: "Buka Spreadsheet Dokumen"

        - name: "Tambahkan tanda tangan elektronik ke OTS"
          link: "/signature/net/add/qrcode/ots/aztec/"
          description: "Templat Spreadsheet OpenDocument"

        - name: "Tambahkan tanda tangan elektronik ke PPT"
          link: "/signature/net/add/qrcode/ppt/aztec/"
          description: "Presentasi powerpoint"

        - name: "Tambahkan tanda tangan elektronik ke PPTX"
          link: "/signature/net/add/qrcode/pptx/aztec/"
          description: "Presentasi PowerPoint Terbuka XML"

        - name: "Tambahkan tanda tangan elektronik ke PPS"
          link: "/signature/net/add/qrcode/pps/aztec/"
          description: "Peragaan Slide Microsoft PowerPoint 97-2003"

        - name: "Tambahkan tanda tangan elektronik ke PPSX"
          link: "/signature/net/add/qrcode/ppsx/aztec/"
          description: "PowerPoint Terbuka XML Slide Show"                              

        - name: "Tambahkan tanda tangan elektronik ke ODP"
          link: "/signature/net/add/qrcode/odp/aztec/"
          description: "Presentasi OpenDocument"

        - name: "Tambahkan tanda tangan elektronik ke OTP"
          link: "/signature/net/add/qrcode/otp/aztec/"
          description: "Template Presentasi OpenDocument"

        - name: "Tambahkan tanda tangan elektronik ke WEBP"
          link: "/signature/net/add/qrcode/webp/aztec/"
          description: "Gambar WebP"

        - name: "Tambahkan tanda tangan elektronik ke TIF"
          link: "/signature/net/add/qrcode/tif/aztec/"
          description: "Format File Gambar yang Ditandai"

        - name: "Tambahkan tanda tangan elektronik ke JPG"
          link: "/signature/net/add/qrcode/jpg/aztec/"
          description: "Gambar JPEG"

        - name: "Tambahkan tanda tangan elektronik ke GIF"
          link: "/signature/net/add/qrcode/gif/aztec/"
          description: "Format Pertukaran Grafik"

        - name: "Tambahkan tanda tangan elektronik ke PNG"
          link: "/signature/net/add/qrcode/png/aztec/"
          description: "Grafik Jaringan Portabel"

        - name: "Tambahkan tanda tangan elektronik ke BMP"
          link: "/signature/net/add/qrcode/bmp/aztec/"
          description: "Format File Bitmap"

        - name: "Tambahkan tanda tangan elektronik ke CDR"
          link: "/signature/net/add/qrcode/cdr/aztec/"
          description: "Gambar Grafis Vektor CorelDraw"

        - name: "Tambahkan tanda tangan elektronik ke SVG"
          link: "/signature/net/add/qrcode/svg/aztec/"
          description: "Grafik Vektor Skalabel"

        - name: "Tambahkan tanda tangan elektronik ke PSD"
          link: "/signature/net/add/qrcode/psd/aztec/"
          description: "Dokumen Adobe Photoshop"

        - name: "Tambahkan tanda tangan elektronik ke WMF"
          link: "/signature/net/add/qrcode/wmf/aztec/"
          description: "Metafile Windows"        

        - name: "Tambahkan tanda tangan elektronik ke CMX"
          link: "/signature/net/add/qrcode/cmx/aztec/"
          description: "Corel Metafile eXchange Gambar"

        - name: "Tambahkan tanda tangan elektronik ke DJVU"
          link: "/signature/net/add/qrcode/djvu/aztec/"
          description: "Deja Vu"

        - name: "Tambahkan tanda tangan elektronik ke PPSM"
          link: "/signature/net/add/qrcode/ppsm/aztec/"
          description: "Peragaan Slide Berkemampuan Makro Microsoft PowerPoint"

back_to_top:
    enable: true
---
