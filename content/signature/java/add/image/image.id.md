---
layout: "auto-gen"
date: 2022-07-07T12:44:18+03:00
draft: false

head_title: "Tanda tangani file IMAGE dengan IMAGE Signatures di Java"
head_description: "Tambahkan tanda tangan IMAGE untuk menandatangani dokumen IMAGE secara digital di Jawa - tambahkan tanda tangan elektronik khusus ke dokumen bisnis populer dan format file IMAGE."

title: "Tambahkan IMAGE Tanda Tangan ke IMAGE File Di Jawa"
description: "Tambahkan tanda tangan digital ke file IMAGE Anda menggunakan jenis tanda tangan IMAGE yang populer. Tambahkan tanda tangan IMAGE khusus secara aman dengan memanipulasi properti tanda tangan - siapkan opsi penandatanganan lanjutan dalam dokumen yang sesuai dengan kebutuhan Anda."
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
        [GroupDocs.Signature for Java](/id/signature/java/) adalah Java API asli untuk menandatangani dokumen digital secara elektronik menggunakan berbagai jenis tanda tangan seperti teks, IMAGE, kode batang, stempel, bidang formulir, kode QR, dan metadata. Pengguna dapat menambahkan, memperbarui, memvalidasi, menghapus, dan mencari tanda tangan digital dalam PDF, Microsoft Word, lembar kerja Excel, presentasi PowerPoint, Adobe Photoshop, OpenDocument, metafile, dan format file IMAGE dengan dukungan tambahan untuk menyesuaikan properti tanda tangan sesuai kebutuhan.

steps:
    enable: true
    title_left: "Cara Menambahkan Tanda Tangan IMAGE ke IMAGE"
    content_left: |
        [GroupDocs.Signature](/id/signature/java/) memudahkan pengembang Java untuk menambahkan tanda tangan IMAGE ke file IMAGE dalam aplikasi mereka dengan menerapkan beberapa langkah mudah.

        * Buat instance baru kelas Signature dan berikan jalur dokumen sumber sebagai parameter konstruktor.
        * Buat instance objek ImageSignOptions sesuai dengan kebutuhan Anda dan tentukan opsi tanda tangan IMAGE.
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
        Signature signature = new Signature("sample.bmp"))
        
        ImageSignOptions options = new ImageSignOptions("signature.jpg") ;
        
        // atur posisi tanda tangan
        options.setLeft(100);
        options.setTop(100);

        // mengatur nomor halaman
        options.setPageNumber(1);

        // menandatangani dokumen ke file
        signature.sign("SampleSigned.bmp", options);
        ```
        
demos:
    enable: true
    title: "Demo Langsung - Aplikasi Online untuk Menambahkan Tanda Tangan Digital"
    content: |
        Tambahkan tanda tangan elektronik ke file IMAGE sekarang juga dengan mengunjungi situs web [GroupDocs.Signature](https://products.groupdocs.app/signature/family). Demo langsung memiliki manfaat sebagai berikut.
        
about_formats:
    enable: true
    format:
        - icon: "far fa-file-image-o"
          title: "Tentang Format Berkas IMAGE"
          content: |
            Format file IMAGE adalah metode standar untuk mengatur dan menyimpan gambar di perangkat seperti komputer, tablet, dan ponsel cerdas. Gambar digital menyimpan data IMAGE dalam kisi piksel 2 dimensi di mana setiap piksel merupakan representasi warna dalam hal jumlah bit. Jenis file IMAGE diklasifikasikan ke dalam format IMAGE vektor dan format IMAGE raster. Gambar 3D adalah jenis lain dari format file IMAGE vektor yang digunakan untuk mengelola gambar 3D.

          link: "https://docs.fileformat.com/image/"

more_formats:
    enable: true
    title: "Menandatangani Format Dokumen Digital Lainnya"
    content: |
        API manajemen tanda tangan digital Java untuk dokumen dan gambar. Tambahkan tanda tangan IMAGE ke beberapa format file populer seperti yang dinyatakan di bawah ini.
    format: 
        - name: "Tambahkan IMAGE tanda tangan ke PDF"
          link: "/signature/java/add/image/pdf/"
          description: "Format Dokumen Portabel Adobe"

        - name: "Tambahkan IMAGE tanda tangan ke DOC"
          link: "/signature/java/add/image/doc/"
          description: "Dokumen Microsoft Word"

        - name: "Tambahkan IMAGE tanda tangan ke DOCM"
          link: "/signature/java/add/image/docm/"
          description: "Dokumen Berkemampuan Makro Microsoft Word"

        - name: "Tambahkan IMAGE tanda tangan ke DOCX"
          link: "/signature/java/add/image/docx/"
          description: "Microsoft Word Buka Dokumen XML"

        - name: "Tambahkan IMAGE tanda tangan ke DOT"
          link: "/signature/java/add/image/dot/"
          description: "Templat Dokumen Microsoft Word"

        - name: "Tambahkan IMAGE tanda tangan ke DOTX"
          link: "/signature/java/add/image/dotx/"
          description: "Templat Dokumen XML Word Terbuka"

        - name: "Tambahkan IMAGE tanda tangan ke DOTM"
          link: "/signature/java/add/image/dotm/"
          description: "Templat Microsoft Word Macro-Enabled"

        - name: "Tambahkan IMAGE tanda tangan ke RTF"
          link: "/signature/java/add/image/rtf/"
          description: "Dokumen Teks Kaya"

        - name: "Tambahkan IMAGE tanda tangan ke ODT"
          link: "/signature/java/add/image/odt/"
          description: "Buka Teks Dokumen"

        - name: "Tambahkan IMAGE tanda tangan ke OTT"
          link: "/signature/java/add/image/ott/"
          description: "Templat Teks OpenDocument"

        - name: "Tambahkan IMAGE tanda tangan ke XLS"
          link: "/signature/java/add/image/xls/"
          description: "Format File Biner Microsoft Excel"

        - name: "Tambahkan IMAGE tanda tangan ke XLSX"
          link: "/signature/java/add/image/xlsx/"
          description: "Microsoft Excel Buka XML Spreadsheet"

        - name: "Tambahkan tanda tangan IMAGE ke XLSM"
          link: "/signature/java/add/image/xlsm/"
          description: "Spreadsheet Berkemampuan Makro Microsoft Excel"

        - name: "Tambahkan tanda tangan IMAGE ke XLSM"
          link: "/signature/java/add/image/xlsm/"
          description: "Spreadsheet Berkemampuan Makro Microsoft Excel"

        - name: "Tambahkan IMAGE tanda tangan ke XLSB"
          link: "/signature/java/add/image/xlsb/"
          description: "Lembar Kerja Biner Microsoft Excel"

        - name: "Tambahkan tanda tangan IMAGE ke XLTX"
          link: "/signature/java/add/image/xltx/"
          description: "Templat Microsoft Excel"

        - name: "Tambahkan tanda tangan IMAGE ke XLTM"
          link: "/signature/java/add/image/xltm/"
          description: "Templat berkemampuan makro Microsoft Excel"

        - name: "Tambahkan IMAGE tanda tangan ke ODS"
          link: "/signature/java/add/image/ods/"
          description: "Buka Spreadsheet Dokumen"

        - name: "Tambahkan IMAGE tanda tangan ke OTS"
          link: "/signature/java/add/image/ots/"
          description: "Templat Spreadsheet OpenDocument"

        - name: "Tambahkan IMAGE tanda tangan ke PPT"
          link: "/signature/java/add/image/ppt/"
          description: "Presentasi powerpoint"

        - name: "Tambahkan tanda tangan IMAGE ke PPTX"
          link: "/signature/java/add/image/pptx/"
          description: "Presentasi PowerPoint Terbuka XML"

        - name: "Tambahkan IMAGE tanda tangan ke PPS"
          link: "/signature/java/add/image/pps/"
          description: "Peragaan Slide Microsoft PowerPoint 97-2003"

        - name: "Tambahkan IMAGE tanda tangan ke PPSX"
          link: "/signature/java/add/image/ppsx/"
          description: "PowerPoint Terbuka XML Slide Show"

        - name: "Tambahkan IMAGE tanda tangan ke POTM"
          link: "/signature/java/add/image/potm/"
          description: "Templat Microsoft PowerPoint Macro-Enabled"

        - name: "Tambahkan IMAGE tanda tangan ke POTX"
          link: "/signature/java/add/image/potx/"
          description: "Templat Microsoft PowerPoint"

        - name: "Tambahkan IMAGE tanda tangan ke PPTM"
          link: "/signature/java/add/image/pptm/"
          description: "Presentasi Microsoft PowerPoint"

        - name: "Tambahkan IMAGE tanda tangan ke ODP"
          link: "/signature/java/add/image/odp/"
          description: "Presentasi OpenDocument"

        - name: "Tambahkan IMAGE tanda tangan ke OTP"
          link: "/signature/java/add/image/otp/"
          description: "Template Presentasi OpenDocument"

        - name: "Tambahkan IMAGE tanda tangan ke WEBP"
          link: "/signature/java/add/image/webp/"
          description: "WebP IMAGE"

        - name: "Tambahkan IMAGE tanda tangan ke TIFF"
          link: "/signature/java/add/image/tiff/"
          description: "Ditandai Format File IMAGE"

        - name: "Tambahkan tanda tangan IMAGE ke JPEG"
          link: "/signature/java/add/image/jpeg/"
          description: "JPEG IMAGE"

        - name: "Tambahkan IMAGE tanda tangan ke GIF"
          link: "/signature/java/add/image/gif/"
          description: "Format Pertukaran Grafik"

        - name: "Tambahkan IMAGE tanda tangan ke PNG"
          link: "/signature/java/add/image/png/"
          description: "Grafik Jaringan Portabel"

        - name: "Tambahkan IMAGE tanda tangan ke BMP"
          link: "/signature/java/add/image/bmp/"
          description: "Format File Bitmap"

        - name: "Tambahkan IMAGE tanda tangan ke CDR"
          link: "/signature/java/add/image/cdr/"
          description: "Gambar Grafis Vektor CorelDraw"

        - name: "Tambahkan IMAGE tanda tangan ke SVG"
          link: "/signature/java/add/image/svg/"
          description: "Grafik Vektor Skalabel"

        - name: "Tambahkan tanda tangan IMAGE ke PSD"
          link: "/signature/java/add/image/psd/"
          description: "Dokumen Adobe Photoshop"

        - name: "Tambahkan IMAGE tanda tangan ke WMF"
          link: "/signature/java/add/image/wmf/"
          description: "Metafile Windows"

        - name: "Tambahkan IMAGE tanda tangan ke EMF"
          link: "/signature/java/add/image/emf/"
          description: "Format Metafile yang Ditingkatkan"

        - name: "Tambahkan IMAGE tanda tangan ke CMX"
          link: "/signature/java/add/image/cmx/"
          description: "Corel Metafile eXchange IMAGE"

        - name: "Tambahkan IMAGE tanda tangan ke DJVU"
          link: "/signature/java/add/image/djvu/"
          description: "Deja Vu"

        - name: "Tambahkan IMAGE tanda tangan ke PPSM"
          link: "/signature/java/add/image/ppsm/"
          description: "Peragaan Slide Berkemampuan Makro Microsoft PowerPoint"

        - name: "Tambahkan IMAGE tanda tangan ke DCM"
          link: "/signature/java/add/image/dcm/"
          description: "Pencitraan Digital dan Komunikasi dalam Kedokteran"


back_to_top:
    enable: true
---
