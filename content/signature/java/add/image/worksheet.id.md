---
layout: "auto-gen"
date: 2022-07-07T12:44:18+03:00
draft: false

head_title: "Menandatangani Lembar Kerja Excel dengan Tanda Tangan Gambar di Java"
head_description: "Tambahkan tanda tangan gambar untuk menandatangani Lembar Kerja Excel di Java secara digital - tambahkan tanda tangan elektronik khusus ke dokumen bisnis populer dan format file gambar."

title: "Tambahkan Tanda Tangan Gambar ke Lembar Kerja di .NET"
description: "Tambahkan tanda tangan digital ke Lembar Kerja Anda menggunakan jenis tanda tangan gambar populer. Tambahkan tanda tangan gambar khusus secara aman dengan memanipulasi properti tanda tangan - siapkan opsi penandatanganan lanjutan dalam dokumen yang sesuai dengan kebutuhan Anda."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Unduh Uji Coba Gratis"
    link: "https://downloads.groupdocs.com/signature/java"

submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"

    middle:
        button:

            - link: "https://apireference.groupdocs.com/signature/java"
              text: "Referensi API"

            - link: "https://github.com/groupdocs-signature"
              text: "Contoh Kode"

            - link: "https://products.groupdocs.app/signature/family"
              text: "Demo Langsung"

            - link: "https://purchase.groupdocs.com/pricing/signature/java"
              text: "Harga"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/java"
        link_buy: "https://purchase.groupdocs.com"

about:
    enable: true
    title: "Tentang GroupDocs.Signature untuk Java API"
    content: |
        [GroupDocs.Signature for Java](/id/signature/java/) adalah Java API asli untuk menandatangani dokumen digital secara elektronik menggunakan berbagai jenis tanda tangan seperti teks, gambar, kode batang, stempel, bidang formulir, kode QR, dan metadata. Pengguna dapat menambah, memperbarui, memvalidasi, menghapus, dan mencari tanda tangan digital dalam PDF, Microsoft Word, lembar kerja Excel, presentasi PowerPoint, Adobe Photoshop, OpenDocument, metafile, dan format file gambar dengan dukungan tambahan untuk menyesuaikan properti tanda tangan sesuai kebutuhan.

steps:
    enable: true
    title_left: "Tambahkan Tanda Tangan Gambar ke Lembar Kerja"
    content_left: |
        [GroupDocs.Signature](/id/signature/java/) memudahkan pengembang Java untuk menambahkan tanda tangan gambar ke Lembar Kerja dalam aplikasi mereka dengan menerapkan beberapa langkah mudah.

        * Buat instance baru kelas Signature dan berikan jalur dokumen sumber sebagai parameter konstruktor.
        * Buat instance objek ImageSignOptions sesuai dengan kebutuhan Anda dan tentukan opsi tanda tangan Gambar.
        * Metode Call Sign dari instance kelas Signature dan berikan ImageSignOptions ke sana.
        
    title_right: "Persyaratan sistem"
    content_right: |
        GroupDocs.Signature untuk Java API didukung di semua platform dan sistem operasi utama. Sebelum menjalankan kode di bawah ini, pastikan Anda telah menginstal prasyarat berikut di sistem Anda.

        * Sistem Operasi: Microsoft Windows, Linux, MacOS
        * Lingkungan Pengembangan: NetBeans, IntelliJ IDEA, Eclipse
        * Kerangka: Java 7 (1.7) dan di atasnya
        * Unduh versi terbaru GroupDocs.Signature untuk Java dari [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
        
    code: |
        ```cs
        Signature signature = new Signature("sample.xlsx"))
        
        ImageSignOptions options = new ImageSignOptions("signature.jpg") ;
        
        // atur posisi tanda tangan
        options.setLeft(100);
        options.setTop(100);

        // mengatur nomor halaman
        options.setPageNumber(1);

        // menandatangani dokumen ke file
        signature.sign("SampleSigned.xlsx", options);
        ```
        
demos:
    enable: true
    title: "Demo Langsung - Aplikasi Online untuk Menambahkan Tanda Tangan Digital"
    content: |
        Tambahkan tanda tangan elektronik ke file Lembar Kerja sekarang juga dengan mengunjungi situs web [GroupDocs.Signature](https://products.groupdocs.app/signature/family). Demo langsung memiliki manfaat sebagai berikut.
        
about_formats:
    enable: true
    format:
        - icon: "far fa-file-excel-o"
          title: "Tentang Format File Spreadsheet"
          content: |
            File spreadsheet berisi data dalam bentuk baris dan kolom. File spreadsheet dapat disimpan dalam beberapa format file yang berbeda, masing-masing memiliki ekstensi file yang berbeda untuk representasi yang unik. Data disimpan dalam sel baik dalam bentuk biasa seperti string teks, angka, tanggal, mata uang, dll. Atau sebagai rumus yang mengubah nilai sel saat nilai sel yang direferensikan berubah. Ekstensi file spreadsheet umum dan format filenya termasuk XLSX (Microsoft Excel Open XML Spreadsheet), ODS (OpenDocument Spreadsheet) dan XLS (Microsoft Excel Binary File Format).

          link: "https://docs.fileformat.com/spreadsheet/"

more_formats:
    enable: true
    title: "Menandatangani Format Dokumen Digital Lainnya"
    content: |
        API manajemen tanda tangan digital Java untuk dokumen dan gambar. Tambahkan tanda tangan gambar ke beberapa format file populer seperti yang dinyatakan di bawah ini.
    format: 
        - name: "Tambahkan tanda tangan gambar ke PDF"
          link: "/signature/java/add/image/pdf/"
          description: "Format Dokumen Portabel Adobe"

        - name: "Tambahkan tanda tangan gambar ke DOC"
          link: "/signature/java/add/image/doc/"
          description: "Dokumen Microsoft Word"

        - name: "Tambahkan tanda tangan gambar ke DOCM"
          link: "/signature/java/add/image/docm/"
          description: "Dokumen Berkemampuan Makro Microsoft Word"

        - name: "Tambahkan tanda tangan gambar ke DOCX"
          link: "/signature/java/add/image/docx/"
          description: "Microsoft Word Buka Dokumen XML"

        - name: "Tambahkan tanda tangan gambar ke DOT"
          link: "/signature/java/add/image/dot/"
          description: "Templat Dokumen Microsoft Word"

        - name: "Tambahkan tanda tangan gambar ke DOTX"
          link: "/signature/java/add/image/dotx/"
          description: "Templat Dokumen XML Word Terbuka"

        - name: "Tambahkan tanda tangan gambar ke DOTM"
          link: "/signature/java/add/image/dotm/"
          description: "Templat Microsoft Word Macro-Enabled"

        - name: "Tambahkan tanda tangan gambar ke RTF"
          link: "/signature/java/add/image/rtf/"
          description: "Dokumen Teks Kaya"

        - name: "Tambahkan tanda tangan gambar ke ODT"
          link: "/signature/java/add/image/odt/"
          description: "Buka Teks Dokumen"

        - name: "Tambahkan tanda tangan gambar ke OTT"
          link: "/signature/java/add/image/ott/"
          description: "Templat Teks OpenDocument"

        - name: "Tambahkan tanda tangan gambar ke XLS"
          link: "/signature/java/add/image/xls/"
          description: "Format File Biner Microsoft Excel"

        - name: "Tambahkan tanda tangan gambar ke XLSX"
          link: "/signature/java/add/image/xlsx/"
          description: "Microsoft Excel Buka XML Spreadsheet"

        - name: "Tambahkan tanda tangan gambar ke XLSM"
          link: "/signature/java/add/image/xlsm/"
          description: "Spreadsheet Berkemampuan Makro Microsoft Excel"

        - name: "Tambahkan tanda tangan gambar ke XLSM"
          link: "/signature/java/add/image/xlsm/"
          description: "Spreadsheet Berkemampuan Makro Microsoft Excel"

        - name: "Tambahkan tanda tangan gambar ke XLSB"
          link: "/signature/java/add/image/xlsb/"
          description: "Microsoft Excel Biner WORKSHEET"

        - name: "Tambahkan tanda tangan gambar ke XLTX"
          link: "/signature/java/add/image/xltx/"
          description: "Templat Microsoft Excel"

        - name: "Tambahkan tanda tangan gambar ke XLTM"
          link: "/signature/java/add/image/xltm/"
          description: "Templat berkemampuan makro Microsoft Excel"

        - name: "Tambahkan tanda tangan gambar ke ODS"
          link: "/signature/java/add/image/ods/"
          description: "Buka Spreadsheet Dokumen"

        - name: "Tambahkan tanda tangan gambar ke OTS"
          link: "/signature/java/add/image/ots/"
          description: "Templat Spreadsheet OpenDocument"

        - name: "Tambahkan tanda tangan gambar ke PPT"
          link: "/signature/java/add/image/ppt/"
          description: "Presentasi powerpoint"

        - name: "Tambahkan tanda tangan gambar ke PPTX"
          link: "/signature/java/add/image/pptx/"
          description: "Presentasi PowerPoint Terbuka XML"

        - name: "Tambahkan tanda tangan gambar ke PPS"
          link: "/signature/java/add/image/pps/"
          description: "Peragaan Slide Microsoft PowerPoint 97-2003"

        - name: "Tambahkan tanda tangan gambar ke PPSX"
          link: "/signature/java/add/image/ppsx/"
          description: "PowerPoint Terbuka XML Slide Show"

        - name: "Tambahkan tanda tangan gambar ke POTM"
          link: "/signature/java/add/image/potm/"
          description: "Templat Microsoft PowerPoint Macro-Enabled"

        - name: "Tambahkan tanda tangan gambar ke POTX"
          link: "/signature/java/add/image/potx/"
          description: "Templat Microsoft PowerPoint"

        - name: "Tambahkan tanda tangan gambar ke PPTM"
          link: "/signature/java/add/image/pptm/"
          description: "Presentasi Microsoft PowerPoint"

        - name: "Tambahkan tanda tangan gambar ke ODP"
          link: "/signature/java/add/image/odp/"
          description: "Presentasi OpenDocument"

        - name: "Tambahkan tanda tangan gambar ke OTP"
          link: "/signature/java/add/image/otp/"
          description: "Template Presentasi OpenDocument"

        - name: "Tambahkan tanda tangan gambar ke WEBP"
          link: "/signature/java/add/image/webp/"
          description: "Gambar WebP"

        - name: "Tambahkan tanda tangan gambar ke TIFF"
          link: "/signature/java/add/image/tiff/"
          description: "Format File Gambar yang Ditandai"

        - name: "Tambahkan tanda tangan gambar ke JPEG"
          link: "/signature/java/add/image/jpeg/"
          description: "Gambar JPEG"

        - name: "Tambahkan tanda tangan gambar ke GIF"
          link: "/signature/java/add/image/gif/"
          description: "Format Pertukaran Grafik"

        - name: "Tambahkan tanda tangan gambar ke PNG"
          link: "/signature/java/add/image/png/"
          description: "Grafik Jaringan Portabel"

        - name: "Tambahkan tanda tangan gambar ke BMP"
          link: "/signature/java/add/image/bmp/"
          description: "Format File Bitmap"

        - name: "Tambahkan tanda tangan gambar ke CDR"
          link: "/signature/java/add/image/cdr/"
          description: "Gambar Grafis Vektor CorelDraw"

        - name: "Tambahkan tanda tangan gambar ke SVG"
          link: "/signature/java/add/image/svg/"
          description: "Grafik Vektor Skalabel"

        - name: "Tambahkan tanda tangan gambar ke PSD"
          link: "/signature/java/add/image/psd/"
          description: "Dokumen Adobe Photoshop"

        - name: "Tambahkan tanda tangan gambar ke WMF"
          link: "/signature/java/add/image/wmf/"
          description: "Metafile Windows"

        - name: "Tambahkan tanda tangan gambar ke EMF"
          link: "/signature/java/add/image/emf/"
          description: "Format Metafile yang Ditingkatkan"

        - name: "Tambahkan tanda tangan gambar ke CMX"
          link: "/signature/java/add/image/cmx/"
          description: "Corel Metafile eXchange Gambar"

        - name: "Tambahkan tanda tangan gambar ke DJVU"
          link: "/signature/java/add/image/djvu/"
          description: "Deja Vu"

        - name: "Tambahkan tanda tangan gambar ke PPSM"
          link: "/signature/java/add/image/ppsm/"
          description: "Peragaan Slide Berkemampuan Makro Microsoft PowerPoint"

        - name: "Tambahkan tanda tangan gambar ke DCM"
          link: "/signature/java/add/image/dcm/"
          description: "Pencitraan Digital dan Komunikasi dalam Kedokteran"


back_to_top:
    enable: true
---
