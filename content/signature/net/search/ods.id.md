---
layout: "auto-gen"
date: 2022-07-07T12:44:18+03:00
draft: false

head_title: "Cari &amp; Validasi Tanda Tangan Digital dalam file ODS di C# .NET"
head_description: "C# .NET API untuk mencari tanda tangan digital dalam file ODS yang ditandatangani, gambar lain, dan format file dokumen menggunakan beberapa baris kode."

title: "Cari Tanda Tangan Digital dalam File ODS"
description: "C# .NET API asli untuk melihat &amp; cari tanda tangan digital dalam file ODS yang sudah ditandatangani dan analisis sertifikat tanda tangan. Lakukan operasi tanda tangan elektronik tingkat lanjut dalam dokumen Anda menggunakan beberapa baris kode."
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

            - link: "https://docs.groupdocs.com/signature/net/release-notes"
              text: "Catatan Rilis"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/net"
        link_buy: "https://purchase.groupdocs.com"

about:
    enable: true
    title: "Tentang GroupDocs.Signature untuk .NET API"
    content: |
        [GroupDocs.Signature for .NET](/id/signature/net/) adalah .NET API canggih untuk menandatangani dokumen digital secara elektronik menggunakan berbagai jenis tanda tangan seperti teks, gambar, kode batang, stempel, bidang formulir, kode QR, dan metadata. Pengguna dapat memuat, mengedit, memvalidasi, menyimpan, menghapus, menemukan dan melihat pratinjau tanda tangan digital dalam PDF, Microsoft Word, lembar kerja Excel, presentasi PowerPoint, Adobe Photoshop, metafile dan format file gambar, dengan dukungan tambahan untuk menyesuaikan properti tanda tangan sesuai kebutuhan.

steps:
    enable: true
    title_left: "Cara Mencari Tanda Tangan di ODS"
    content_left: |
        [GroupDocs.Signature](/id/signature/net/) memudahkan pengembang .NET untuk melihat & mencari tanda tangan digital dalam file ODS dari dalam aplikasi mereka dengan menerapkan beberapa langkah mudah.

        * Buat instance baru kelas Signature dan berikan jalur dokumen sumber sebagai parameter konstruktor.
        * Buat instance objek DigitalSearchOptions sesuai dengan kebutuhan Anda dan tentukan opsi pencarian.
        * Panggil metode Pencarian dari instance kelas Signature dan berikan DigitalSearchOptions ke sana.
        
    title_right: "Persyaratan sistem"
    content_right: |
        GroupDocs.Signature untuk .NET API didukung di semua platform dan sistem operasi utama. Sebelum menjalankan kode di bawah ini, pastikan Anda telah menginstal prasyarat berikut di sistem Anda.

        * Sistem Operasi: Microsoft Windows, Linux, MacOS
        * Lingkungan Pengembangan: Visual Studio, Xamarin, MonoDevelop
        * Kerangka: .NET Framework, .NET Standard, .NET Core, Mono
        * Unduh versi terbaru GroupDocs.Signature untuk .NET dari [NuGet](https://www.nuget.org/packages/groupdocs.signature)
        
    code: |
        ```cs
        using (Signature signature = new Signature("signed.pdf"))
        {
            DigitalSearchOptions options = new DigitalSearchOptions()
            {
                // tentukan kriteria pencarian khusus
                Comments = "Test comment",
                // kriteria masalah sertifikat
                IssuerName = "John",
                // subjek sertifikat digital
                SubjectName = "Test",
                // tentukan rentang tanggal periode tanda tangan
                SignDateTimeFrom = DateTime.Now.AddMonths(-1),
                SignDateTimeTo = DateTime.Now,
                //
            };
            // mencari tanda tangan di dokumen
            List signatures = signature.Search(options);
            Console.WriteLine("\nSource document contains following signatures.");
            foreach (var digitalSignature in signatures)
            {
                Console.WriteLine("Digital signature found from {0} with validation flag {1}. Certificate SN {2}",
                    digitalSignature.SignTime, digitalSignature.IsValid, digitalSignature.Certificate?.SerialNumber);
            }
        }
        ```
        
demos:
    enable: true
    title: "Cari ODS Signature Live Demo"
    content: |
        Tambahkan file ODS tanda tangan elektronik sekarang juga dengan mengunjungi situs web [GroupDocs.Signature](https://products.groupdocs.app/signature/family).
        Demo langsung memiliki manfaat sebagai berikut
about_formats:
    enable: true
    format:
        - icon: "far fa-file-ods"
          title: "Apa itu Format File ODS"
          content: |
            File dengan ekstensi ODS adalah singkatan dari format OpenDocument Spreadsheet Document yang dapat diedit oleh pengguna. Data disimpan di dalam file ODF ke dalam baris dan kolom. Ini adalah format berbasis XML dan merupakan salah satu dari beberapa subtipe dalam keluarga Open Document Formats (ODF). Format ditentukan sebagai bagian dari spesifikasi ODF 1.2 yang diterbitkan dan dikelola oleh OASIS. Sejumlah aplikasi di Windows serta sistem operasi lain dapat membuka file ODS untuk diedit dan dimanipulasi termasuk Microsoft Excel, NeoOffice, dan LibreOffice. File ODS juga dapat dikonversi ke format spreadsheet lain seperti XLS, XLSX, dan lainnya dengan aplikasi yang berbeda. Pelajari lebih lanjut tentang format file ODS

          link: "https://docs.fileformat.com/spreadsheet/ods/"

more_formats:
    enable: true
    title: "Pilihan Lain yang Tersedia"
    content: |
        API pencarian tanda tangan digital multi format untuk dokumen dan gambar. Temukan tanda tangan dari beberapa format file populer seperti yang dinyatakan di bawah ini.
    format: 
        - name: "Cari tanda tangan elektronik dalam PDF"
          link: "/signature/net/search/pdf/"
          description: "Format Dokumen Portabel Adobe"

        - name: "Cari tanda tangan elektronik di DOC"
          link: "/signature/net/search/doc/"
          description: "Dokumen Microsoft Word"

        - name: "Cari tanda tangan elektronik di DOCM"
          link: "/signature/net/search/docm/"
          description: "Dokumen Berkemampuan Makro Microsoft Word"

        - name: "Cari tanda tangan elektronik di DOCX"
          link: "/signature/net/search/docx/"
          description: "Microsoft Word Buka Dokumen XML"

        - name: "Cari tanda tangan elektronik di DOT"
          link: "/signature/net/search/dot/"
          description: "Templat Dokumen Microsoft Word"

        - name: "Cari tanda tangan elektronik di DOTX"
          link: "/signature/net/search/dotx/"
          description: "Templat Dokumen XML Word Terbuka"

        - name: "Cari tanda tangan elektronik di DOTM"
          link: "/signature/net/search/dotm/"
          description: "Templat Microsoft Word Macro-Enabled"

        - name: "Cari tanda tangan elektronik di RTF"
          link: "/signature/net/search/rtf/"
          description: "Dokumen Teks Kaya"

        - name: "Cari tanda tangan elektronik di ODT"
          link: "/signature/net/search/odt/"
          description: "Buka Teks Dokumen"

        - name: "Cari tanda tangan elektronik di OTT"
          link: "/signature/net/search/ott/"
          description: "Templat Teks OpenDocument"

        - name: "Cari tanda tangan elektronik di XLS"
          link: "/signature/net/search/xls/"
          description: "Format File Biner Microsoft Excel"

        - name: "Cari tanda tangan elektronik di XLSX"
          link: "/signature/net/search/xlsx/"
          description: "Microsoft Excel Buka XML Spreadsheet"

        - name: "Cari tanda tangan elektronik di XLSM"
          link: "/signature/net/search/xlsm/"
          description: "Spreadsheet Berkemampuan Makro Microsoft Excel"

        - name: "Cari tanda tangan elektronik di XLSM"
          link: "/signature/net/search/xlsm/"
          description: "Spreadsheet Berkemampuan Makro Microsoft Excel"

        - name: "Cari tanda tangan elektronik di XLSB"
          link: "/signature/net/search/xlsb/"
          description: "Lembar Kerja Biner Microsoft Excel"

        - name: "Cari tanda tangan elektronik di XLTX"
          link: "/signature/net/search/xltx/"
          description: "Templat Microsoft Excel"

        - name: "Cari tanda tangan elektronik di XLTM"
          link: "/signature/net/search/xltm/"
          description: "Templat berkemampuan makro Microsoft Excel"

        - name: "Cari tanda tangan elektronik di ODS"
          link: "/signature/net/search/ods/"
          description: "Buka Spreadsheet Dokumen"

        - name: "Cari tanda tangan elektronik di OTS"
          link: "/signature/net/search/ots/"
          description: "Templat Spreadsheet OpenDocument"

        - name: "Cari tanda tangan elektronik di PPT"
          link: "/signature/net/search/ppt/"
          description: "Presentasi powerpoint"

        - name: "Cari tanda tangan elektronik di PPTX"
          link: "/signature/net/search/pptx/"
          description: "Presentasi PowerPoint Terbuka XML"

        - name: "Cari tanda tangan elektronik di PPS"
          link: "/signature/net/search/pps/"
          description: "Peragaan Slide Microsoft PowerPoint 97-2003"

        - name: "Cari tanda tangan elektronik di PPSX"
          link: "/signature/net/search/ppsx/"
          description: "PowerPoint Terbuka XML Slide Show"

        - name: "Cari tanda tangan elektronik di POTM"
          link: "/signature/net/search/potm/"
          description: "Templat Microsoft PowerPoint Macro-Enabled"

        - name: "Cari tanda tangan elektronik di POTX"
          link: "/signature/net/search/potx/"
          description: "Templat Microsoft PowerPoint"

        - name: "Cari tanda tangan elektronik di PPTM"
          link: "/signature/net/search/pptm/"
          description: "Presentasi Microsoft PowerPoint"

        - name: "Cari tanda tangan elektronik di ODP"
          link: "/signature/net/search/odp/"
          description: "Presentasi OpenDocument"

        - name: "Cari tanda tangan elektronik dalam OTP"
          link: "/signature/net/search/otp/"
          description: "Template Presentasi OpenDocument"

        - name: "Cari tanda tangan elektronik di WEBP"
          link: "/signature/net/search/webp/"
          description: "Gambar WebP"

        - name: "Cari tanda tangan elektronik di TIFF"
          link: "/signature/net/search/tiff/"
          description: "Format File Gambar yang Ditandai"

        - name: "Cari tanda tangan elektronik dalam format JPEG"
          link: "/signature/net/search/jpeg/"
          description: "Gambar JPEG"

        - name: "Cari tanda tangan elektronik di GIF"
          link: "/signature/net/search/gif/"
          description: "Format Pertukaran Grafik"

        - name: "Cari tanda tangan elektronik di PNG"
          link: "/signature/net/search/png/"
          description: "Grafik Jaringan Portabel"

        - name: "Cari tanda tangan elektronik di BMP"
          link: "/signature/net/search/bmp/"
          description: "Format File Bitmap"

        - name: "Cari tanda tangan elektronik di CDR"
          link: "/signature/net/search/cdr/"
          description: "Gambar Grafis Vektor CorelDraw"

        - name: "Cari tanda tangan elektronik di SVG"
          link: "/signature/net/search/svg/"
          description: "Grafik Vektor Skalabel"

        - name: "Cari tanda tangan elektronik di PSD"
          link: "/signature/net/search/psd/"
          description: "Dokumen Adobe Photoshop"

        - name: "Cari tanda tangan elektronik di WMF"
          link: "/signature/net/search/wmf/"
          description: "Metafile Windows"

        - name: "Cari tanda tangan elektronik di EMF"
          link: "/signature/net/search/emf/"
          description: "Format Metafile yang Ditingkatkan"

        - name: "Cari tanda tangan elektronik di CMX"
          link: "/signature/net/search/cmx/"
          description: "Corel Metafile eXchange Gambar"

        - name: "Cari tanda tangan elektronik di DJVU"
          link: "/signature/net/search/djvu/"
          description: "Deja Vu"

        - name: "Cari tanda tangan elektronik di PPSM"
          link: "/signature/net/search/ppsm/"
          description: "Peragaan Slide Berkemampuan Makro Microsoft PowerPoint"

        - name: "Cari tanda tangan elektronik di DCM"
          link: "/signature/net/search/dcm/"
          description: "Pencitraan Digital dan Komunikasi dalam Kedokteran"


back_to_top:
    enable: true
---
