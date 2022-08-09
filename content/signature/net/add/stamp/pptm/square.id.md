---
layout: "auto-gen"
date: 2022-07-07T12:44:18+03:00
draft: false

head_title: "Tambahkan Stempel SQUARE dan Tanda Tangani File PPTM| Menandatangani Dokumen"
head_description: "Tanda tangani file PPTM dengan tanda tangan stempel SQUARE - tambahkan stempel ke dokumen bisnis populer dan format file gambar."

title: "Tambahkan Tanda Tangan Cap SQUARE ke File PPTM"
description: "Masuk file PPTM Anda menggunakan stempel SQUARE di C#. Memanipulasi properti tanda tangan dan mengatur opsi penandatanganan lanjutan dalam dokumen yang sesuai dengan kebutuhan Anda."
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
    title_left: "Cara menandatangani file PPTM dengan Stempel SQUARE"
    content_left: |
        [GroupDocs.Signature](/id/signature/net/) memudahkan pengembang .NET untuk menambahkan stempel SQUARE ke file PPTM dalam aplikasi mereka dengan menerapkan beberapa langkah mudah.

        * Buat instance baru kelas Signature dan berikan jalur dokumen PPTM sumber sebagai parameter konstruktor.
        * Buat instance objek StampSignOptions dengan teks yang diperlukan dan setel properti EncodeType ke SQUARE.
        * Metode Tanda Panggil kelas Tanda Tangan dan berikan nama file PPTM keluaran dengan StampSignOptions ke dalamnya.
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
        using (Signature signature = new Signature("sample.pptm"))
        {
            // Atur tampilan stempel SQUARE - ukuran, posisi di halaman dokumen, ukuran font, warna, dll.
            StampSignOptions signOptions = new StampSignOptions
            {
                StampType = StampTypes.Square,
                Height = 300,
                Width = 300,
                VerticalAlignment = VerticalAlignment.Center,
                HorizontalAlignment = HorizontalAlignment.Left,
                Background = new Background() { Color = Color.DarkOrange, Transparency = 0.5 },
                ImageFilePath = "handwrite_signature.jpg",
            };

            // Tambahkan garis luar tanda tangan
            signOptions.OuterLines.Add(
                new StampLine
                {
                    Text = "* Mr. John Smith *",
                    TextRepeatType = StampTextRepeatType.FullTextRepeat,
                    Font = new SignatureFont() { Size = 12, FamilyName = "Arial" },
                    Height = 30,
                    TextBottomIntent = 6,
                    TextColor = Color.WhiteSmoke,
                    BackgroundColor = Color.DarkSlateBlue
                }
            );

            // Masuk file PPTM dan simpan hasilnya 
            signature.Sign("signed.pptm", options);
        }
        ```
        
demos:
    enable: true
    title: "Demo Langsung - Aplikasi Online untuk Menghasilkan Tanda Tangan Stempel SQUARE"
    content: |
        Tambahkan stempel SQUARE ke file PPTM sekarang juga dengan mengunjungi situs web [GroupDocs.Signature](https://products.groupdocs.app/signature/family). Demo langsung memiliki manfaat sebagai berikut.
        
about_formats:
    enable: true
    format:
        - icon: "fas fa-stamp"
          title: "Tentang Stempel SQUARE"
          content: |
            Perangko SQUARE populer digunakan untuk inisial dan sebagai stempel loyalitas, juga digunakan dengan kontrol dokumen, kontrol kualitas, serta pemeriksaan dokumen.

          link: ""

more_formats:
    enable: true
    title: "Menandatangani Format File Lain dengan SQUARE Stamp menggunakan C#"
    content: |
        API manajemen tanda tangan stempel .NET untuk dokumen dan gambar. Tambahkan tanda tangan cap ke beberapa format file populer seperti yang dinyatakan di bawah ini.
    format: 
        - name: "Tambahkan tanda tangan elektronik ke PDF"
          link: "/signature/net/add/stamp/pdf/square/"
          description: "Format Dokumen Portabel Adobe"

        - name: "Tambahkan tanda tangan elektronik ke DOC"
          link: "/signature/net/add/stamp/doc/square/"
          description: "Dokumen Microsoft Word"

        - name: "Tambahkan tanda tangan elektronik ke DOCM"
          link: "/signature/net/add/stamp/docm/square/"
          description: "Dokumen Berkemampuan Makro Microsoft Word"

        - name: "Tambahkan tanda tangan elektronik ke DOCX"
          link: "/signature/net/add/stamp/docx/square/"
          description: "Microsoft Word Buka Dokumen XML"

        - name: "Tambahkan tanda tangan elektronik ke DOT"
          link: "/signature/net/add/stamp/dot/square/"
          description: "Templat Dokumen Microsoft Word"

        - name: "Tambahkan tanda tangan elektronik ke DOTX"
          link: "/signature/net/add/stamp/dotx/square/"
          description: "Templat Dokumen XML Word Terbuka"

        - name: "Tambahkan tanda tangan elektronik ke DOTM"
          link: "/signature/net/add/stamp/dotm/square/"
          description: "Templat Microsoft Word Macro-Enabled"       

        - name: "Tambahkan tanda tangan elektronik ke ODT"
          link: "/signature/net/add/stamp/odt/square/"
          description: "Buka Teks Dokumen"

        - name: "Tambahkan tanda tangan elektronik ke OTT"
          link: "/signature/net/add/stamp/ott/square/"
          description: "Templat Teks OpenDocument"

        - name: "Tambahkan tanda tangan elektronik ke XLS"
          link: "/signature/net/add/stamp/xls/square/"
          description: "Format File Biner Microsoft Excel"

        - name: "Tambahkan tanda tangan elektronik ke XLSX"
          link: "/signature/net/add/stamp/xlsx/square/"
          description: "Microsoft Excel Buka XML Spreadsheet"

        - name: "Tambahkan tanda tangan elektronik ke XLSM"
          link: "/signature/net/add/stamp/xlsm/square/"
          description: "Spreadsheet Berkemampuan Makro Microsoft Excel"

        - name: "Tambahkan tanda tangan elektronik ke XLSB"
          link: "/signature/net/add/stamp/xlsb/square/"
          description: "Lembar Kerja Biner Microsoft Excel"

        - name: "Tambahkan tanda tangan elektronik ke XLTX"
          link: "/signature/net/add/stamp/xltx/square/"
          description: "Templat Microsoft Excel"

        - name: "Tambahkan tanda tangan elektronik ke XLTM"
          link: "/signature/net/add/stamp/xltm/square/"
          description: "Templat berkemampuan makro Microsoft Excel"

        - name: "Tambahkan tanda tangan elektronik ke ODS"
          link: "/signature/net/add/stamp/ods/square/"
          description: "Buka Spreadsheet Dokumen"

        - name: "Tambahkan tanda tangan elektronik ke OTS"
          link: "/signature/net/add/stamp/ots/square/"
          description: "Templat Spreadsheet OpenDocument"

        - name: "Tambahkan tanda tangan elektronik ke PPT"
          link: "/signature/net/add/stamp/ppt/square/"
          description: "Presentasi powerpoint"

        - name: "Tambahkan tanda tangan elektronik ke PPTX"
          link: "/signature/net/add/stamp/pptx/square/"
          description: "Presentasi PowerPoint Terbuka XML"

        - name: "Tambahkan tanda tangan elektronik ke PPS"
          link: "/signature/net/add/stamp/pps/square/"
          description: "Peragaan Slide Microsoft PowerPoint 97-2003"

        - name: "Tambahkan tanda tangan elektronik ke PPSX"
          link: "/signature/net/add/stamp/ppsx/square/"
          description: "PowerPoint Terbuka XML Slide Show"                              

        - name: "Tambahkan tanda tangan elektronik ke ODP"
          link: "/signature/net/add/stamp/odp/square/"
          description: "Presentasi OpenDocument"

        - name: "Tambahkan tanda tangan elektronik ke OTP"
          link: "/signature/net/add/stamp/otp/square/"
          description: "Template Presentasi OpenDocument"

        - name: "Tambahkan tanda tangan elektronik ke WEBP"
          link: "/signature/net/add/stamp/webp/square/"
          description: "Gambar WebP"

        - name: "Tambahkan tanda tangan elektronik ke TIF"
          link: "/signature/net/add/stamp/tif/square/"
          description: "Format File Gambar yang Ditandai"

        - name: "Tambahkan tanda tangan elektronik ke JPG"
          link: "/signature/net/add/stamp/jpg/square/"
          description: "Gambar JPEG"

        - name: "Tambahkan tanda tangan elektronik ke GIF"
          link: "/signature/net/add/stamp/gif/square/"
          description: "Format Pertukaran Grafik"

        - name: "Tambahkan tanda tangan elektronik ke PNG"
          link: "/signature/net/add/stamp/png/square/"
          description: "Grafik Jaringan Portabel"

        - name: "Tambahkan tanda tangan elektronik ke BMP"
          link: "/signature/net/add/stamp/bmp/square/"
          description: "Format File Bitmap"

        - name: "Tambahkan tanda tangan elektronik ke CDR"
          link: "/signature/net/add/stamp/cdr/square/"
          description: "Gambar Grafis Vektor CorelDraw"

        - name: "Tambahkan tanda tangan elektronik ke SVG"
          link: "/signature/net/add/stamp/svg/square/"
          description: "Grafik Vektor Skalabel"

        - name: "Tambahkan tanda tangan elektronik ke PSD"
          link: "/signature/net/add/stamp/psd/square/"
          description: "Dokumen Adobe Photoshop"

        - name: "Tambahkan tanda tangan elektronik ke WMF"
          link: "/signature/net/add/stamp/wmf/square/"
          description: "Metafile Windows"        

        - name: "Tambahkan tanda tangan elektronik ke CMX"
          link: "/signature/net/add/stamp/cmx/square/"
          description: "Corel Metafile eXchange Gambar"

        - name: "Tambahkan tanda tangan elektronik ke DJVU"
          link: "/signature/net/add/stamp/djvu/square/"
          description: "Deja Vu"

        - name: "Tambahkan tanda tangan elektronik ke PPSM"
          link: "/signature/net/add/stamp/ppsm/square/"
          description: "Peragaan Slide Berkemampuan Makro Microsoft PowerPoint"

back_to_top:
    enable: true
---
