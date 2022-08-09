---
layout: "auto-gen"
date: 2022-07-07T12:44:18+03:00
draft: false

head_title: "Masuk file J2C dengan JPG Image Signatures di C# .NET"
head_description: "Tambahkan tanda tangan gambar JPG untuk menandatangani dokumen J2C secara digital di C# .NET - tambahkan tanda tangan elektronik khusus ke dokumen bisnis populer dan format file gambar."

title: "Tambahkan Tanda Tangan Gambar ke File J2C di .NET"
description: "Tanda tangani file J2C Anda secara digital menggunakan JPG dan jenis tanda tangan gambar populer lainnya. Memanipulasi properti tanda tangan dan mengatur opsi penandatanganan lanjutan dalam dokumen yang sesuai dengan kebutuhan Anda."
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
    title_left: "Cara Menambahkan Tanda Tangan Gambar ke J2C"
    content_left: |
        [GroupDocs.Signature](/id/signature/net/) memudahkan pengembang .NET untuk menambahkan tanda tangan gambar ke file J2C dalam aplikasi mereka dengan menerapkan beberapa langkah mudah.

        * Buat instance baru kelas Signature dan berikan jalur dokumen sumber sebagai parameter konstruktor.
        * Buat instance objek ImageSignOptions sesuai dengan kebutuhan Anda dan tentukan opsi tanda tangan Gambar.
        * Metode Call Sign dari instance kelas Signature dan berikan ImageSignOptions ke sana.
        
    title_right: "Persyaratan sistem"
    content_right: |
        GroupDocs.Signature untuk .NET API didukung di semua platform dan sistem operasi utama. Sebelum menjalankan kode di bawah ini, pastikan Anda telah menginstal prasyarat berikut di sistem Anda.

        * Sistem Operasi: Microsoft Windows, Linux, MacOS
        * Lingkungan Pengembangan: Visual Studio, Xamarin, MonoDevelop
        * Kerangka: .NET Framework, .NET Standard, .NET Core, Mono
        * Unduh versi terbaru GroupDocs.Signature untuk .NET dari [NuGet](https://www.nuget.org/packages/groupdocs.signature)
        
    code: |
        ```cs
        using (Signature signature = new Signature("sample.j2c"))
        {
            ImageSignOptions options = new ImageSignOptions("signature.jpg")
            {
                // atur posisi tanda tangan
                Left = 100,
                Top = 100,
                AllPages = true                
            };
            signature.Sign("SampleSigned.j2c", options);
        }
        ```
        
demos:
    enable: true
    title: "Demo Langsung - Aplikasi Online untuk Menambahkan Tanda Tangan Digital"
    content: |
        Tambahkan tanda tangan ke file J2C sekarang juga dengan mengunjungi situs web [GroupDocs.Signature](https://products.groupdocs.app/signature/family). Demo langsung memiliki manfaat sebagai berikut.
        
about_formats:
    enable: true
    format:
        - icon: "far fa-file-image-o"
          title: "Tentang Format Berkas J2C"
          content: |
            File dengan ekstensi .J2C adalah varian dari format file JPEG dan dikompresi dengan kompresi wavelet. Ini memiliki sistem penanda dan segmen yang hampir identik dengan format file JPEG 2000. Format file J2C seperti yang didefinisikan dalam Bagian 1 dari stand JPEG 2000 yang mendukung kompresi lossy dan lossless. Codestream JPEG 2000 dirancang untuk disematkan dalam JP2 atau format file lain, meskipun mungkin muncul dalam file itu sendiri. File J2C dapat dibuka menggunakan Adobe Photoshop 2020, Adobe Illustrator 2020, dan Corel Paintshop Pro.

          link: "https://docs.fileformat.com/image/j2c/"

more_formats:
    enable: true
    title: "Menandatangani Format Dokumen Digital Lainnya"
    content: |
        .NET API manajemen tanda tangan digital untuk dokumen dan gambar. Tambahkan tanda tangan gambar ke beberapa format file populer seperti yang dinyatakan di bawah ini.
    format: 
        - name: "Tambahkan tanda tangan gambar ke PDF"
          link: "/signature/net/add/jpg/pdf/"
          description: "Format Dokumen Portabel Adobe"

        - name: "Tambahkan tanda tangan gambar ke DOC"
          link: "/signature/net/add/jpg/doc/"
          description: "Dokumen Microsoft Word"

        - name: "Tambahkan tanda tangan gambar ke DOCM"
          link: "/signature/net/add/jpg/docm/"
          description: "Dokumen Berkemampuan Makro Microsoft Word"

        - name: "Tambahkan tanda tangan gambar ke DOCX"
          link: "/signature/net/add/jpg/docx/"
          description: "Microsoft Word Buka Dokumen XML"

        - name: "Tambahkan tanda tangan gambar ke DOT"
          link: "/signature/net/add/jpg/dot/"
          description: "Templat Dokumen Microsoft Word"

        - name: "Tambahkan tanda tangan gambar ke DOTX"
          link: "/signature/net/add/jpg/dotx/"
          description: "Templat Dokumen XML Word Terbuka"

        - name: "Tambahkan tanda tangan gambar ke DOTM"
          link: "/signature/net/add/jpg/dotm/"
          description: "Templat Microsoft Word Macro-Enabled"

        - name: "Tambahkan tanda tangan gambar ke RTF"
          link: "/signature/net/add/jpg/rtf/"
          description: "Dokumen Teks Kaya"

        - name: "Tambahkan tanda tangan gambar ke ODT"
          link: "/signature/net/add/jpg/odt/"
          description: "Buka Teks Dokumen"

        - name: "Tambahkan tanda tangan gambar ke OTT"
          link: "/signature/net/add/jpg/ott/"
          description: "Templat Teks OpenDocument"

        - name: "Tambahkan tanda tangan gambar ke XLS"
          link: "/signature/net/add/jpg/xls/"
          description: "Format File Biner Microsoft Excel"

        - name: "Tambahkan tanda tangan gambar ke XLSX"
          link: "/signature/net/add/jpg/xlsx/"
          description: "Microsoft Excel Buka XML Spreadsheet"

        - name: "Tambahkan tanda tangan gambar ke XLSM"
          link: "/signature/net/add/jpg/xlsm/"
          description: "Spreadsheet Berkemampuan Makro Microsoft Excel"

        - name: "Tambahkan tanda tangan gambar ke XLSM"
          link: "/signature/net/add/jpg/xlsm/"
          description: "Spreadsheet Berkemampuan Makro Microsoft Excel"

        - name: "Tambahkan tanda tangan gambar ke XLSB"
          link: "/signature/net/add/jpg/xlsb/"
          description: "Lembar Kerja Biner Microsoft Excel"

        - name: "Tambahkan tanda tangan gambar ke XLTX"
          link: "/signature/net/add/jpg/xltx/"
          description: "Templat Microsoft Excel"

        - name: "Tambahkan tanda tangan gambar ke XLTM"
          link: "/signature/net/add/jpg/xltm/"
          description: "Templat berkemampuan makro Microsoft Excel"

        - name: "Tambahkan tanda tangan gambar ke ODS"
          link: "/signature/net/add/jpg/ods/"
          description: "Buka Spreadsheet Dokumen"

        - name: "Tambahkan tanda tangan gambar ke OTS"
          link: "/signature/net/add/jpg/ots/"
          description: "Templat Spreadsheet OpenDocument"

        - name: "Tambahkan tanda tangan gambar ke PPT"
          link: "/signature/net/add/jpg/ppt/"
          description: "Presentasi powerpoint"

        - name: "Tambahkan tanda tangan gambar ke PPTX"
          link: "/signature/net/add/jpg/pptx/"
          description: "Presentasi PowerPoint Terbuka XML"

        - name: "Tambahkan tanda tangan gambar ke PPS"
          link: "/signature/net/add/jpg/pps/"
          description: "Peragaan Slide Microsoft PowerPoint 97-2003"

        - name: "Tambahkan tanda tangan gambar ke PPSX"
          link: "/signature/net/add/jpg/ppsx/"
          description: "PowerPoint Terbuka XML Slide Show"

        - name: "Tambahkan tanda tangan gambar ke POTM"
          link: "/signature/net/add/jpg/potm/"
          description: "Templat Microsoft PowerPoint Macro-Enabled"

        - name: "Tambahkan tanda tangan gambar ke POTX"
          link: "/signature/net/add/jpg/potx/"
          description: "Templat Microsoft PowerPoint"

        - name: "Tambahkan tanda tangan gambar ke PPTM"
          link: "/signature/net/add/jpg/pptm/"
          description: "Presentasi Microsoft PowerPoint"

        - name: "Tambahkan tanda tangan gambar ke ODP"
          link: "/signature/net/add/jpg/odp/"
          description: "Presentasi OpenDocument"

        - name: "Tambahkan tanda tangan gambar ke OTP"
          link: "/signature/net/add/jpg/otp/"
          description: "Template Presentasi OpenDocument"

        - name: "Tambahkan tanda tangan gambar ke WEBP"
          link: "/signature/net/add/jpg/webp/"
          description: "Gambar WebP"

        - name: "Tambahkan tanda tangan gambar ke TIFF"
          link: "/signature/net/add/jpg/tiff/"
          description: "Format File Gambar yang Ditandai"

        - name: "Tambahkan tanda tangan gambar ke JPEG"
          link: "/signature/net/add/jpg/jpeg/"
          description: "Gambar JPEG"

        - name: "Tambahkan tanda tangan gambar ke GIF"
          link: "/signature/net/add/jpg/gif/"
          description: "Format Pertukaran Grafik"

        - name: "Tambahkan tanda tangan gambar ke PNG"
          link: "/signature/net/add/jpg/png/"
          description: "Grafik Jaringan Portabel"

        - name: "Tambahkan tanda tangan gambar ke BMP"
          link: "/signature/net/add/jpg/bmp/"
          description: "Format File Bitmap"

        - name: "Tambahkan tanda tangan gambar ke CDR"
          link: "/signature/net/add/jpg/cdr/"
          description: "Gambar Grafis Vektor CorelDraw"

        - name: "Tambahkan tanda tangan gambar ke SVG"
          link: "/signature/net/add/jpg/svg/"
          description: "Grafik Vektor Skalabel"

        - name: "Tambahkan tanda tangan gambar ke PSD"
          link: "/signature/net/add/jpg/psd/"
          description: "Dokumen Adobe Photoshop"

        - name: "Tambahkan tanda tangan gambar ke WMF"
          link: "/signature/net/add/jpg/wmf/"
          description: "Metafile Windows"

        - name: "Tambahkan tanda tangan gambar ke EMF"
          link: "/signature/net/add/jpg/emf/"
          description: "Format Metafile yang Ditingkatkan"

        - name: "Tambahkan tanda tangan gambar ke CMX"
          link: "/signature/net/add/jpg/cmx/"
          description: "Corel Metafile eXchange Gambar"

        - name: "Tambahkan tanda tangan gambar ke DJVU"
          link: "/signature/net/add/jpg/djvu/"
          description: "Deja Vu"

        - name: "Tambahkan tanda tangan gambar ke PPSM"
          link: "/signature/net/add/jpg/ppsm/"
          description: "Peragaan Slide Berkemampuan Makro Microsoft PowerPoint"

        - name: "Tambahkan tanda tangan gambar ke DCM"
          link: "/signature/net/add/jpg/dcm/"
          description: "Pencitraan Digital dan Komunikasi dalam Kedokteran"


back_to_top:
    enable: true
---
