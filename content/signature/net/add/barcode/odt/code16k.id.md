---
layout: "auto-gen"
date: 2022-07-07T12:44:18+03:00
draft: false

head_title: "Hasilkan CODE16K Barcode dan Masuk File ODT di .NET | Menandatangani Dokumen"
head_description: "Tanda tangani file ODT dengan tanda tangan kode batang CODE16K di .NET - tambahkan kode batang ke dokumen bisnis populer dan format file gambar."

title: "Tambahkan CODE16K Barcode Signatures ke File ODT di C#"
description: "Tanda tangani file ODT Anda menggunakan kode batang CODE16K. Memanipulasi properti tanda tangan dan mengatur opsi penandatanganan lanjutan dalam dokumen yang sesuai dengan kebutuhan Anda."
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
    title_left: "Cara Menghasilkan CODE16K Barcode untuk file ODT di C#"
    content_left: |
        [GroupDocs.Signature](/id/signature/net/) memudahkan pengembang .NET untuk menambahkan kode batang CODE16K ke file ODT dalam aplikasi mereka dengan menerapkan beberapa langkah mudah.

        * Buat instance baru kelas Signature dan berikan jalur dokumen ODT sumber sebagai parameter konstruktor.
        * Buat instance objek BarcodeSignOptions dengan teks yang diperlukan dan setel properti EncodeType ke CODE16K.
        * Metode Panggil Sign dari kelas Signature dan berikan nama file ODT keluaran dengan BarcodeSignOptions ke dalamnya.
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
        using (Signature signature = new Signature("sample.odt"))
        {
            // Inisialisasi opsi kode batang dengan teks kode batang yang telah ditentukan sebelumnya
            BarcodeSignOptions options = new BarcodeSignOptions("JohnSmith")
            {
                // atur jenis penyandian kode batang
                EncodeType = BarcodeTypes.Code16K,

                // atur posisi tanda tangan
                Left = 50,
                Top = 150,
                Width = 200,
                Height = 50
            };

            // Masuk file ODT dan simpan hasilnya 
            signature.Sign("signed.odt", options);
        }
        ```
        
demos:
    enable: true
    title: "Demo Langsung - Aplikasi Online untuk Menghasilkan CODE16K Barcode Signatures"
    content: |
        Tambahkan kode batang CODE16K ke file ODT sekarang juga dengan mengunjungi situs web [GroupDocs.Signature](https://products.groupdocs.app/signature/family). Demo langsung memiliki manfaat sebagai berikut.
        
about_formats:
    enable: true
    format:
        - icon: "fas fa-barcode"
          title: "Tentang CODE16K Barcode"
          content: |
            Kode 16K adalah simbologi bertumpuk dua dimensi berdasarkan Kode 128. Ini dikembangkan pada tahun 1989 oleh Ted Williams dan telah digunakan terutama di industri perawatan kesehatan.

          link: ""

more_formats:
    enable: true
    title: "Menandatangani Format Dokumen Lain dengan CODE16K Barcode menggunakan C#"
    content: |
        .NET Barcode Signature Management API untuk dokumen dan gambar. Tambahkan tanda tangan kode batang ke beberapa format file populer seperti yang dinyatakan di bawah ini.
    format: 
        - name: "Tambahkan tanda tangan elektronik ke PDF"
          link: "/signature/net/add/barcode/pdf/code16k/"
          description: "Format Dokumen Portabel Adobe"

        - name: "Tambahkan tanda tangan elektronik ke DOC"
          link: "/signature/net/add/barcode/doc/code16k/"
          description: "Dokumen Microsoft Word"

        - name: "Tambahkan tanda tangan elektronik ke DOCM"
          link: "/signature/net/add/barcode/docm/code16k/"
          description: "Dokumen Berkemampuan Makro Microsoft Word"

        - name: "Tambahkan tanda tangan elektronik ke DOCX"
          link: "/signature/net/add/barcode/docx/code16k/"
          description: "Microsoft Word Buka Dokumen XML"

        - name: "Tambahkan tanda tangan elektronik ke DOT"
          link: "/signature/net/add/barcode/dot/code16k/"
          description: "Templat Dokumen Microsoft Word"

        - name: "Tambahkan tanda tangan elektronik ke DOTX"
          link: "/signature/net/add/barcode/dotx/code16k/"
          description: "Templat Dokumen XML Word Terbuka"

        - name: "Tambahkan tanda tangan elektronik ke DOTM"
          link: "/signature/net/add/barcode/dotm/code16k/"
          description: "Templat Microsoft Word Macro-Enabled"       

        - name: "Tambahkan tanda tangan elektronik ke ODT"
          link: "/signature/net/add/barcode/odt/code16k/"
          description: "Buka Teks Dokumen"

        - name: "Tambahkan tanda tangan elektronik ke OTT"
          link: "/signature/net/add/barcode/ott/code16k/"
          description: "Templat Teks OpenDocument"

        - name: "Tambahkan tanda tangan elektronik ke XLS"
          link: "/signature/net/add/barcode/xls/code16k/"
          description: "Format File Biner Microsoft Excel"

        - name: "Tambahkan tanda tangan elektronik ke XLSX"
          link: "/signature/net/add/barcode/xlsx/code16k/"
          description: "Microsoft Excel Buka XML Spreadsheet"

        - name: "Tambahkan tanda tangan elektronik ke XLSM"
          link: "/signature/net/add/barcode/xlsm/code16k/"
          description: "Spreadsheet Berkemampuan Makro Microsoft Excel"

        - name: "Tambahkan tanda tangan elektronik ke XLSB"
          link: "/signature/net/add/barcode/xlsb/code16k/"
          description: "Lembar Kerja Biner Microsoft Excel"

        - name: "Tambahkan tanda tangan elektronik ke XLTX"
          link: "/signature/net/add/barcode/xltx/code16k/"
          description: "Templat Microsoft Excel"

        - name: "Tambahkan tanda tangan elektronik ke XLTM"
          link: "/signature/net/add/barcode/xltm/code16k/"
          description: "Templat berkemampuan makro Microsoft Excel"

        - name: "Tambahkan tanda tangan elektronik ke ODS"
          link: "/signature/net/add/barcode/ods/code16k/"
          description: "Buka Spreadsheet Dokumen"

        - name: "Tambahkan tanda tangan elektronik ke OTS"
          link: "/signature/net/add/barcode/ots/code16k/"
          description: "Templat Spreadsheet OpenDocument"

        - name: "Tambahkan tanda tangan elektronik ke PPT"
          link: "/signature/net/add/barcode/ppt/code16k/"
          description: "Presentasi powerpoint"

        - name: "Tambahkan tanda tangan elektronik ke PPTX"
          link: "/signature/net/add/barcode/pptx/code16k/"
          description: "Presentasi PowerPoint Terbuka XML"

        - name: "Tambahkan tanda tangan elektronik ke PPS"
          link: "/signature/net/add/barcode/pps/code16k/"
          description: "Peragaan Slide Microsoft PowerPoint 97-2003"

        - name: "Tambahkan tanda tangan elektronik ke PPSX"
          link: "/signature/net/add/barcode/ppsx/code16k/"
          description: "PowerPoint Terbuka XML Slide Show"                              

        - name: "Tambahkan tanda tangan elektronik ke ODP"
          link: "/signature/net/add/barcode/odp/code16k/"
          description: "Presentasi OpenDocument"

        - name: "Tambahkan tanda tangan elektronik ke OTP"
          link: "/signature/net/add/barcode/otp/code16k/"
          description: "Template Presentasi OpenDocument"

        - name: "Tambahkan tanda tangan elektronik ke WEBP"
          link: "/signature/net/add/barcode/webp/code16k/"
          description: "Gambar WebP"

        - name: "Tambahkan tanda tangan elektronik ke TIF"
          link: "/signature/net/add/barcode/tif/code16k/"
          description: "Format File Gambar yang Ditandai"

        - name: "Tambahkan tanda tangan elektronik ke JPG"
          link: "/signature/net/add/barcode/jpg/code16k/"
          description: "Gambar JPEG"

        - name: "Tambahkan tanda tangan elektronik ke GIF"
          link: "/signature/net/add/barcode/gif/code16k/"
          description: "Format Pertukaran Grafik"

        - name: "Tambahkan tanda tangan elektronik ke PNG"
          link: "/signature/net/add/barcode/png/code16k/"
          description: "Grafik Jaringan Portabel"

        - name: "Tambahkan tanda tangan elektronik ke BMP"
          link: "/signature/net/add/barcode/bmp/code16k/"
          description: "Format File Bitmap"

        - name: "Tambahkan tanda tangan elektronik ke CDR"
          link: "/signature/net/add/barcode/cdr/code16k/"
          description: "Gambar Grafis Vektor CorelDraw"

        - name: "Tambahkan tanda tangan elektronik ke SVG"
          link: "/signature/net/add/barcode/svg/code16k/"
          description: "Grafik Vektor Skalabel"

        - name: "Tambahkan tanda tangan elektronik ke PSD"
          link: "/signature/net/add/barcode/psd/code16k/"
          description: "Dokumen Adobe Photoshop"

        - name: "Tambahkan tanda tangan elektronik ke WMF"
          link: "/signature/net/add/barcode/wmf/code16k/"
          description: "Metafile Windows"        

        - name: "Tambahkan tanda tangan elektronik ke CMX"
          link: "/signature/net/add/barcode/cmx/code16k/"
          description: "Corel Metafile eXchange Gambar"

        - name: "Tambahkan tanda tangan elektronik ke DJVU"
          link: "/signature/net/add/barcode/djvu/code16k/"
          description: "Deja Vu"

        - name: "Tambahkan tanda tangan elektronik ke PPSM"
          link: "/signature/net/add/barcode/ppsm/code16k/"
          description: "Peragaan Slide Berkemampuan Makro Microsoft PowerPoint"

back_to_top:
    enable: true
---
