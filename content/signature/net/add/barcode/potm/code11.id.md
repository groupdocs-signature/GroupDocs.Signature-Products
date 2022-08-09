---
layout: "auto-gen"
date: 2022-07-07T12:44:18+03:00
draft: false

head_title: "Hasilkan CODE11 Barcode dan Masuk File POTM di .NET | Menandatangani Dokumen"
head_description: "Tanda tangani file POTM dengan tanda tangan kode batang CODE11 di .NET - tambahkan kode batang ke dokumen bisnis populer dan format file gambar."

title: "Tambahkan CODE11 Barcode Signatures ke File POTM di C#"
description: "Tanda tangani file POTM Anda menggunakan kode batang CODE11. Memanipulasi properti tanda tangan dan mengatur opsi penandatanganan lanjutan dalam dokumen yang sesuai dengan kebutuhan Anda."
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
    title_left: "Cara Menghasilkan CODE11 Barcode untuk file POTM di C#"
    content_left: |
        [GroupDocs.Signature](/id/signature/net/) memudahkan pengembang .NET untuk menambahkan kode batang CODE11 ke file POTM dalam aplikasi mereka dengan menerapkan beberapa langkah mudah.

        * Buat instance baru kelas Signature dan berikan jalur dokumen POTM sumber sebagai parameter konstruktor.
        * Buat instance objek BarcodeSignOptions dengan teks yang diperlukan dan setel properti EncodeType ke CODE11.
        * Metode Tanda Panggil kelas Tanda Tangan dan berikan nama file POTM keluaran dengan BarcodeSignOptions ke dalamnya.
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
        using (Signature signature = new Signature("sample.potm"))
        {
            // Inisialisasi opsi kode batang dengan teks kode batang yang telah ditentukan sebelumnya
            BarcodeSignOptions options = new BarcodeSignOptions("JohnSmith")
            {
                // atur jenis penyandian kode batang
                EncodeType = BarcodeTypes.Code11,

                // atur posisi tanda tangan
                Left = 50,
                Top = 150,
                Width = 200,
                Height = 50
            };

            // Tanda tangani file POTM dan simpan hasilnya 
            signature.Sign("signed.potm", options);
        }
        ```
        
demos:
    enable: true
    title: "Demo Langsung - Aplikasi Online untuk Menghasilkan CODE11 Barcode Signatures"
    content: |
        Tambahkan kode batang CODE11 ke file POTM sekarang juga dengan mengunjungi situs web [GroupDocs.Signature](https://products.groupdocs.app/signature/family). Demo langsung memiliki manfaat sebagai berikut.
        
about_formats:
    enable: true
    format:
        - icon: "fas fa-barcode"
          title: "Tentang CODE11 Barcode"
          content: |
            Kode 11 adalah simbologi barcode yang dikembangkan oleh Intermec pada tahun 1977. Digunakan terutama dalam telekomunikasi. Simbol dapat mengkodekan string panjang apa pun yang terdiri dari angka 0-9 dan karakter tanda hubung (-). Kode kedua belas mewakili karakter mulai/berhenti, biasanya dicetak sebagai '*'. Satu atau dua digit pemeriksaan modulo-11 dapat disertakan.

          link: ""

more_formats:
    enable: true
    title: "Menandatangani Format Dokumen Lain dengan CODE11 Barcode menggunakan C#"
    content: |
        .NET Barcode Signature Management API untuk dokumen dan gambar. Tambahkan tanda tangan kode batang ke beberapa format file populer seperti yang dinyatakan di bawah ini.
    format: 
        - name: "Tambahkan tanda tangan elektronik ke PDF"
          link: "/signature/net/add/barcode/pdf/code11/"
          description: "Format Dokumen Portabel Adobe"

        - name: "Tambahkan tanda tangan elektronik ke DOC"
          link: "/signature/net/add/barcode/doc/code11/"
          description: "Dokumen Microsoft Word"

        - name: "Tambahkan tanda tangan elektronik ke DOCM"
          link: "/signature/net/add/barcode/docm/code11/"
          description: "Dokumen Berkemampuan Makro Microsoft Word"

        - name: "Tambahkan tanda tangan elektronik ke DOCX"
          link: "/signature/net/add/barcode/docx/code11/"
          description: "Microsoft Word Buka Dokumen XML"

        - name: "Tambahkan tanda tangan elektronik ke DOT"
          link: "/signature/net/add/barcode/dot/code11/"
          description: "Templat Dokumen Microsoft Word"

        - name: "Tambahkan tanda tangan elektronik ke DOTX"
          link: "/signature/net/add/barcode/dotx/code11/"
          description: "Templat Dokumen XML Word Terbuka"

        - name: "Tambahkan tanda tangan elektronik ke DOTM"
          link: "/signature/net/add/barcode/dotm/code11/"
          description: "Templat Microsoft Word Macro-Enabled"       

        - name: "Tambahkan tanda tangan elektronik ke ODT"
          link: "/signature/net/add/barcode/odt/code11/"
          description: "Buka Teks Dokumen"

        - name: "Tambahkan tanda tangan elektronik ke OTT"
          link: "/signature/net/add/barcode/ott/code11/"
          description: "Templat Teks OpenDocument"

        - name: "Tambahkan tanda tangan elektronik ke XLS"
          link: "/signature/net/add/barcode/xls/code11/"
          description: "Format File Biner Microsoft Excel"

        - name: "Tambahkan tanda tangan elektronik ke XLSX"
          link: "/signature/net/add/barcode/xlsx/code11/"
          description: "Microsoft Excel Buka XML Spreadsheet"

        - name: "Tambahkan tanda tangan elektronik ke XLSM"
          link: "/signature/net/add/barcode/xlsm/code11/"
          description: "Spreadsheet Berkemampuan Makro Microsoft Excel"

        - name: "Tambahkan tanda tangan elektronik ke XLSB"
          link: "/signature/net/add/barcode/xlsb/code11/"
          description: "Lembar Kerja Biner Microsoft Excel"

        - name: "Tambahkan tanda tangan elektronik ke XLTX"
          link: "/signature/net/add/barcode/xltx/code11/"
          description: "Templat Microsoft Excel"

        - name: "Tambahkan tanda tangan elektronik ke XLTM"
          link: "/signature/net/add/barcode/xltm/code11/"
          description: "Templat berkemampuan makro Microsoft Excel"

        - name: "Tambahkan tanda tangan elektronik ke ODS"
          link: "/signature/net/add/barcode/ods/code11/"
          description: "Buka Spreadsheet Dokumen"

        - name: "Tambahkan tanda tangan elektronik ke OTS"
          link: "/signature/net/add/barcode/ots/code11/"
          description: "Templat Spreadsheet OpenDocument"

        - name: "Tambahkan tanda tangan elektronik ke PPT"
          link: "/signature/net/add/barcode/ppt/code11/"
          description: "Presentasi powerpoint"

        - name: "Tambahkan tanda tangan elektronik ke PPTX"
          link: "/signature/net/add/barcode/pptx/code11/"
          description: "Presentasi PowerPoint Terbuka XML"

        - name: "Tambahkan tanda tangan elektronik ke PPS"
          link: "/signature/net/add/barcode/pps/code11/"
          description: "Peragaan Slide Microsoft PowerPoint 97-2003"

        - name: "Tambahkan tanda tangan elektronik ke PPSX"
          link: "/signature/net/add/barcode/ppsx/code11/"
          description: "PowerPoint Terbuka XML Slide Show"                              

        - name: "Tambahkan tanda tangan elektronik ke ODP"
          link: "/signature/net/add/barcode/odp/code11/"
          description: "Presentasi OpenDocument"

        - name: "Tambahkan tanda tangan elektronik ke OTP"
          link: "/signature/net/add/barcode/otp/code11/"
          description: "Template Presentasi OpenDocument"

        - name: "Tambahkan tanda tangan elektronik ke WEBP"
          link: "/signature/net/add/barcode/webp/code11/"
          description: "Gambar WebP"

        - name: "Tambahkan tanda tangan elektronik ke TIF"
          link: "/signature/net/add/barcode/tif/code11/"
          description: "Format File Gambar yang Ditandai"

        - name: "Tambahkan tanda tangan elektronik ke JPG"
          link: "/signature/net/add/barcode/jpg/code11/"
          description: "Gambar JPEG"

        - name: "Tambahkan tanda tangan elektronik ke GIF"
          link: "/signature/net/add/barcode/gif/code11/"
          description: "Format Pertukaran Grafik"

        - name: "Tambahkan tanda tangan elektronik ke PNG"
          link: "/signature/net/add/barcode/png/code11/"
          description: "Grafik Jaringan Portabel"

        - name: "Tambahkan tanda tangan elektronik ke BMP"
          link: "/signature/net/add/barcode/bmp/code11/"
          description: "Format File Bitmap"

        - name: "Tambahkan tanda tangan elektronik ke CDR"
          link: "/signature/net/add/barcode/cdr/code11/"
          description: "Gambar Grafis Vektor CorelDraw"

        - name: "Tambahkan tanda tangan elektronik ke SVG"
          link: "/signature/net/add/barcode/svg/code11/"
          description: "Grafik Vektor Skalabel"

        - name: "Tambahkan tanda tangan elektronik ke PSD"
          link: "/signature/net/add/barcode/psd/code11/"
          description: "Dokumen Adobe Photoshop"

        - name: "Tambahkan tanda tangan elektronik ke WMF"
          link: "/signature/net/add/barcode/wmf/code11/"
          description: "Metafile Windows"        

        - name: "Tambahkan tanda tangan elektronik ke CMX"
          link: "/signature/net/add/barcode/cmx/code11/"
          description: "Corel Metafile eXchange Gambar"

        - name: "Tambahkan tanda tangan elektronik ke DJVU"
          link: "/signature/net/add/barcode/djvu/code11/"
          description: "Deja Vu"

        - name: "Tambahkan tanda tangan elektronik ke PPSM"
          link: "/signature/net/add/barcode/ppsm/code11/"
          description: "Peragaan Slide Berkemampuan Makro Microsoft PowerPoint"

back_to_top:
    enable: true
---
