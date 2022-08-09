---
layout: "auto-gen"
date: 2022-07-07T12:44:18+03:00
draft: false

head_title: "Hasilkan GS1QR QR-code dan Masuk File BMP di .NET | Menandatangani Dokumen"
head_description: "Tanda tangani file BMP dengan tanda tangan kode QR GS1QR di .NET - tambahkan kode batang ke dokumen bisnis populer dan format file gambar."

title: "Tambahkan GS1QR kode QR ke File BMP di C#"
description: "Tanda tangani file BMP Anda menggunakan kode QR GS1QR. Memanipulasi properti tanda tangan dan mengatur opsi penandatanganan lanjutan dalam dokumen yang sesuai dengan kebutuhan Anda."
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
    title_left: "Cara Menghasilkan GS1QR QR-code untuk file BMP di C#"
    content_left: |
        [GroupDocs.Signature](/id/signature/net/) memudahkan pengembang .NET untuk menambahkan kode batang GS1QR ke file BMP dalam aplikasi mereka dengan menerapkan beberapa langkah mudah.

        * Buat instance baru kelas Signature dan berikan jalur dokumen BMP sumber sebagai parameter konstruktor.
        * Buat instance objek QrCodeSignOptions dengan teks yang diperlukan dan setel properti EncodeType ke GS1QR.
        * Metode Tanda Panggil kelas Tanda Tangan dan berikan nama file BMP keluaran dengan QrCodeSignOptions ke dalamnya.
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
        using (Signature signature = new Signature("sample.bmp"))
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

            // Masuk file BMP dan simpan hasilnya 
            signature.Sign("signed.bmp", options);
        }
        ```
        
demos:
    enable: true
    title: "Demo Langsung - Aplikasi Online untuk Menghasilkan GS1QR Tanda Tangan kode QR"
    content: |
        Tambahkan GS1QR qr-codes ke file BMP sekarang juga dengan mengunjungi situs web [GroupDocs.Signature](https://products.groupdocs.app/signature/family). Demo langsung memiliki manfaat sebagai berikut.
        
about_formats:
    enable: true
    format:
        - icon: "fas fa-qrcode"
          title: "Tentang GS1QR kode QR"
          content: |
            GS1 QR Code adalah varian dari QR Code yang sesuai dengan spesifikasi GS1. Itu dirancang khusus untuk berbagi informasi pengemasan yang diperluas, seperti nomor lot, ID produk, dan kuantitas.

          link: ""

more_formats:
    enable: true
    title: "Menandatangani Format File Lain dengan GS1QR QR-code menggunakan C#"
    content: |
        .NET .NET qr-code signatures management API untuk dokumen dan gambar. Tambahkan tanda tangan kode qr ke beberapa format file populer seperti yang dinyatakan di bawah ini.
    format: 
        - name: "Tambahkan tanda tangan elektronik ke PDF"
          link: "/signature/net/add/qrcode/pdf/gs1qr/"
          description: "Format Dokumen Portabel Adobe"

        - name: "Tambahkan tanda tangan elektronik ke DOC"
          link: "/signature/net/add/qrcode/doc/gs1qr/"
          description: "Dokumen Microsoft Word"

        - name: "Tambahkan tanda tangan elektronik ke DOCM"
          link: "/signature/net/add/qrcode/docm/gs1qr/"
          description: "Dokumen Berkemampuan Makro Microsoft Word"

        - name: "Tambahkan tanda tangan elektronik ke DOCX"
          link: "/signature/net/add/qrcode/docx/gs1qr/"
          description: "Microsoft Word Buka Dokumen XML"

        - name: "Tambahkan tanda tangan elektronik ke DOT"
          link: "/signature/net/add/qrcode/dot/gs1qr/"
          description: "Templat Dokumen Microsoft Word"

        - name: "Tambahkan tanda tangan elektronik ke DOTX"
          link: "/signature/net/add/qrcode/dotx/gs1qr/"
          description: "Templat Dokumen XML Word Terbuka"

        - name: "Tambahkan tanda tangan elektronik ke DOTM"
          link: "/signature/net/add/qrcode/dotm/gs1qr/"
          description: "Templat Microsoft Word Macro-Enabled"       

        - name: "Tambahkan tanda tangan elektronik ke ODT"
          link: "/signature/net/add/qrcode/odt/gs1qr/"
          description: "Buka Teks Dokumen"

        - name: "Tambahkan tanda tangan elektronik ke OTT"
          link: "/signature/net/add/qrcode/ott/gs1qr/"
          description: "Templat Teks OpenDocument"

        - name: "Tambahkan tanda tangan elektronik ke XLS"
          link: "/signature/net/add/qrcode/xls/gs1qr/"
          description: "Format File Biner Microsoft Excel"

        - name: "Tambahkan tanda tangan elektronik ke XLSX"
          link: "/signature/net/add/qrcode/xlsx/gs1qr/"
          description: "Microsoft Excel Buka XML Spreadsheet"

        - name: "Tambahkan tanda tangan elektronik ke XLSM"
          link: "/signature/net/add/qrcode/xlsm/gs1qr/"
          description: "Spreadsheet Berkemampuan Makro Microsoft Excel"

        - name: "Tambahkan tanda tangan elektronik ke XLSB"
          link: "/signature/net/add/qrcode/xlsb/gs1qr/"
          description: "Lembar Kerja Biner Microsoft Excel"

        - name: "Tambahkan tanda tangan elektronik ke XLTX"
          link: "/signature/net/add/qrcode/xltx/gs1qr/"
          description: "Templat Microsoft Excel"

        - name: "Tambahkan tanda tangan elektronik ke XLTM"
          link: "/signature/net/add/qrcode/xltm/gs1qr/"
          description: "Templat berkemampuan makro Microsoft Excel"

        - name: "Tambahkan tanda tangan elektronik ke ODS"
          link: "/signature/net/add/qrcode/ods/gs1qr/"
          description: "Buka Spreadsheet Dokumen"

        - name: "Tambahkan tanda tangan elektronik ke OTS"
          link: "/signature/net/add/qrcode/ots/gs1qr/"
          description: "Templat Spreadsheet OpenDocument"

        - name: "Tambahkan tanda tangan elektronik ke PPT"
          link: "/signature/net/add/qrcode/ppt/gs1qr/"
          description: "Presentasi powerpoint"

        - name: "Tambahkan tanda tangan elektronik ke PPTX"
          link: "/signature/net/add/qrcode/pptx/gs1qr/"
          description: "Presentasi PowerPoint Terbuka XML"

        - name: "Tambahkan tanda tangan elektronik ke PPS"
          link: "/signature/net/add/qrcode/pps/gs1qr/"
          description: "Peragaan Slide Microsoft PowerPoint 97-2003"

        - name: "Tambahkan tanda tangan elektronik ke PPSX"
          link: "/signature/net/add/qrcode/ppsx/gs1qr/"
          description: "PowerPoint Terbuka XML Slide Show"                              

        - name: "Tambahkan tanda tangan elektronik ke ODP"
          link: "/signature/net/add/qrcode/odp/gs1qr/"
          description: "Presentasi OpenDocument"

        - name: "Tambahkan tanda tangan elektronik ke OTP"
          link: "/signature/net/add/qrcode/otp/gs1qr/"
          description: "Template Presentasi OpenDocument"

        - name: "Tambahkan tanda tangan elektronik ke WEBP"
          link: "/signature/net/add/qrcode/webp/gs1qr/"
          description: "Gambar WebP"

        - name: "Tambahkan tanda tangan elektronik ke TIF"
          link: "/signature/net/add/qrcode/tif/gs1qr/"
          description: "Format File Gambar yang Ditandai"

        - name: "Tambahkan tanda tangan elektronik ke JPG"
          link: "/signature/net/add/qrcode/jpg/gs1qr/"
          description: "Gambar JPEG"

        - name: "Tambahkan tanda tangan elektronik ke GIF"
          link: "/signature/net/add/qrcode/gif/gs1qr/"
          description: "Format Pertukaran Grafik"

        - name: "Tambahkan tanda tangan elektronik ke PNG"
          link: "/signature/net/add/qrcode/png/gs1qr/"
          description: "Grafik Jaringan Portabel"

        - name: "Tambahkan tanda tangan elektronik ke BMP"
          link: "/signature/net/add/qrcode/bmp/gs1qr/"
          description: "Format File Bitmap"

        - name: "Tambahkan tanda tangan elektronik ke CDR"
          link: "/signature/net/add/qrcode/cdr/gs1qr/"
          description: "Gambar Grafis Vektor CorelDraw"

        - name: "Tambahkan tanda tangan elektronik ke SVG"
          link: "/signature/net/add/qrcode/svg/gs1qr/"
          description: "Grafik Vektor Skalabel"

        - name: "Tambahkan tanda tangan elektronik ke PSD"
          link: "/signature/net/add/qrcode/psd/gs1qr/"
          description: "Dokumen Adobe Photoshop"

        - name: "Tambahkan tanda tangan elektronik ke WMF"
          link: "/signature/net/add/qrcode/wmf/gs1qr/"
          description: "Metafile Windows"        

        - name: "Tambahkan tanda tangan elektronik ke CMX"
          link: "/signature/net/add/qrcode/cmx/gs1qr/"
          description: "Corel Metafile eXchange Gambar"

        - name: "Tambahkan tanda tangan elektronik ke DJVU"
          link: "/signature/net/add/qrcode/djvu/gs1qr/"
          description: "Deja Vu"

        - name: "Tambahkan tanda tangan elektronik ke PPSM"
          link: "/signature/net/add/qrcode/ppsm/gs1qr/"
          description: "Peragaan Slide Berkemampuan Makro Microsoft PowerPoint"

back_to_top:
    enable: true
---
