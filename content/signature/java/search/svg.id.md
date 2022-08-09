---
layout: "auto-gen"
date: 2022-07-07T12:44:18+03:00
draft: false

head_title: "Cari Tanda Tangan Digital di SVG melalui Java Library"
head_description: "Pustaka Java untuk mencari &amp; memvalidasi tanda tangan digital dalam file SVG menggunakan GroupDocs.Siganture API - memanipulasi Gambar, Kode Batang, Kode QR, Stempel, Teks, Optik &amp; Tanda tangan metadata dari dokumen yang ditandatangani secara digital."

title: "Cari Tanda Tangan Digital di SVG melalui Java"
description: "Java eSignature API untuk mencari &amp; memvalidasi tanda tangan digital dalam file SVG. Memanipulasi Gambar, Kode Batang, Kode QR, Stempel, Teks, Optik &amp; Tanda tangan metadata dari dokumen yang ditandatangani secara digital."
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
        [GroupDocs.Signature for Java](/id/signature/java/) adalah pustaka eSignature Java canggih untuk menandatangani dokumen secara digital menggunakan berbagai jenis tanda tangan seperti teks, gambar, kode batang, stempel, bidang formulir, kode QR, dan metadata. Dengan menambahkan hanya beberapa baris kode, perkuat aplikasi Java Anda dengan fitur untuk melihat, membuat, mengedit, memvalidasi, menghapus, dan menemukan tanda tangan digital dalam PDF, Microsoft Word, lembar kerja Excel, presentasi PowerPoint, Adobe Photoshop, metafile, dan format file gambar. API tanda tangan elektronik juga mendukung fitur tambahan untuk menyesuaikan properti tanda tangan sesuai kebutuhan.

steps:
    enable: true
    title_left: "Cara Mencari Tanda Tangan Digital dari SVG"
    content_left: |
        Contoh kode Java di bawah ini dengan jelas menunjukkan langkah-langkah untuk **mencari tanda tangan digital dalam file SVG di Java** dengan menambahkan beberapa baris kode saja.

        * Buat instance baru kelas **Signature** dan teruskan jalur dokumen sumber sebagai parameter konstruktor.
        * Buat instance objek **DigitalSearchOptions** sesuai dengan kebutuhan Anda dan tentukan opsi pencarian.
        * Panggil metode **search** dari instance kelas **Signature** dan teruskan **DigitalSearchOptions** ke dalamnya.
        
    title_right: "Persyaratan sistem"
    content_right: |
        GroupDocs.Signature untuk Java API didukung di semua platform dan sistem operasi utama. Sebelum menjalankan kode di bawah ini, pastikan Anda telah menginstal prasyarat berikut di sistem Anda.

        * Sistem Operasi: Microsoft Windows, Linux, MacOS
        * Lingkungan Pengembangan: Visual Studio, Xamarin, MonoDevelop
        * Kerangka: .NET Framework, .NET Standard, .NET Core, Mono
        * Unduh versi terbaru GroupDocs.Signature untuk Java dari [NuGet](https://www.nuget.org/packages/groupdocs.signature)
        
    code: |
        ```java
        Signature signature = new Signature("signed.pdf");
        DigitalSearchOptions options = new DigitalSearchOptions();
        // tentukan kriteria pencarian khusus
        options.setComments("Test comment");
        // kriteria masalah sertifikat
        options.setIssuerName("John");
        // subjek sertifikat digital
        options.setSubjectName("Test");
        // tentukan rentang tanggal periode tanda tangan
        options.setSignDateTimeFrom(DateUtils.addMonths(new Date(), -1));
        options.setSignDateTimeTo(new Date());
         
        // mencari tanda tangan di dokumen
        List signatures = signature.search(DigitalSignature.class, options);
        System.out.print("\nSource document contains following signatures.");
        for (DigitalSignature digitalSignature : signatures)
        {
            System.out.print("Digital signature found from "+digitalSignature.getSignTime()+" with validation flag "+digitalSignature.isValid()+". Certificate SN "+ digitalSignature.getCertificate().getType());
        }
        ```
        
demos:
    enable: true
    title: "Cari SVG Signature Live Demo"
    content: |
        Tambahkan file SVG tanda tangan elektronik sekarang juga dengan mengunjungi situs web [GroupDocs.Signature](https://products.groupdocs.app/signature/family).
        Demo langsung memiliki manfaat sebagai berikut
about_formats:
    enable: true
    format:
        - icon: "far fa-file-svg"
          title: "Apa itu Format File SVG"
          content: |
            File SVG adalah File Grafik Vektor Scalable yang menggunakan format teks berbasis XML untuk menggambarkan tampilan gambar. Kata Scalable mengacu pada fakta bahwa SVG dapat diskalakan ke berbagai ukuran tanpa kehilangan kualitas apa pun. Deskripsi berbasis teks dari file tersebut membuat mereka independen dari resolusi. Ini adalah salah satu format yang paling banyak digunakan untuk membangun situs web dan mencetak grafik untuk mencapai skalabilitas. Format tersebut hanya dapat digunakan untuk grafik dua dimensi sekalipun. File SVG dapat dilihat/dibuka di hampir semua browser modern termasuk Chrome, Internet Explorer, Firefox, dan Safari. Pelajari lebih lanjut tentang format file SVG

          link: "https://docs.fileformat.com/page-description-language/svg/"

more_formats:
    enable: true
    title: "Pilihan Lain yang Tersedia"
    content: |
        Tanda tangan digital multi-format mencari API untuk dokumen dan gambar. Temukan tanda tangan dari dalam beberapa format file populer seperti yang dinyatakan di bawah ini.
    format: 
        - name: "Cari Tanda Tangan dalam PDF"
          link: "/signature/java/search/pdf/"
          description: "Format Dokumen Portabel Adobe"

        - name: "Cari Tanda Tangan di DOC"
          link: "/signature/java/search/doc/"
          description: "Dokumen Microsoft Word"

        - name: "Cari Tanda Tangan di DOCM"
          link: "/signature/java/search/docm/"
          description: "Dokumen Berkemampuan Makro Microsoft Word"

        - name: "Cari Tanda Tangan di DOCX"
          link: "/signature/java/search/docx/"
          description: "Microsoft Word Buka Dokumen XML"

        - name: "Cari Tanda Tangan di DOT"
          link: "/signature/java/search/dot/"
          description: "Templat Dokumen Microsoft Word"

        - name: "Cari Tanda Tangan di DOTX"
          link: "/signature/java/search/dotx/"
          description: "Templat Dokumen XML Word Terbuka"

        - name: "Cari Tanda Tangan di DOTM"
          link: "/signature/java/search/dotm/"
          description: "Templat Microsoft Word Macro-Enabled"

        - name: "Cari Tanda Tangan di RTF"
          link: "/signature/java/search/rtf/"
          description: "Dokumen Teks Kaya"

        - name: "Cari Tanda Tangan di ODT"
          link: "/signature/java/search/odt/"
          description: "Buka Teks Dokumen"

        - name: "Cari Tanda Tangan di OTT"
          link: "/signature/java/search/ott/"
          description: "Templat Teks OpenDocument"

        - name: "Cari Tanda Tangan di XLS"
          link: "/signature/java/search/xls/"
          description: "Format File Biner Microsoft Excel"

        - name: "Cari Tanda Tangan di XLSX"
          link: "/signature/java/search/xlsx/"
          description: "Microsoft Excel Buka XML Spreadsheet"

        - name: "Cari Tanda Tangan di XLSM"
          link: "/signature/java/search/xlsm/"
          description: "Spreadsheet Berkemampuan Makro Microsoft Excel"

        - name: "Cari Tanda Tangan di XLSM"
          link: "/signature/java/search/xlsm/"
          description: "Spreadsheet Berkemampuan Makro Microsoft Excel"

        - name: "Cari Tanda Tangan di XLSB"
          link: "/signature/java/search/xlsb/"
          description: "Lembar Kerja Biner Microsoft Excel"

        - name: "Cari Tanda Tangan di XLTX"
          link: "/signature/java/search/xltx/"
          description: "Templat Microsoft Excel"

        - name: "Cari Tanda Tangan di XLTM"
          link: "/signature/java/search/xltm/"
          description: "Templat berkemampuan makro Microsoft Excel"

        - name: "Cari Tanda Tangan di ODS"
          link: "/signature/java/search/ods/"
          description: "Buka Spreadsheet Dokumen"

        - name: "Cari Tanda Tangan di OTS"
          link: "/signature/java/search/ots/"
          description: "Templat Spreadsheet OpenDocument"

        - name: "Cari Tanda Tangan di PPT"
          link: "/signature/java/search/ppt/"
          description: "Presentasi powerpoint"

        - name: "Cari Tanda Tangan di PPTX"
          link: "/signature/java/search/pptx/"
          description: "Presentasi PowerPoint Terbuka XML"

        - name: "Cari Tanda Tangan di PPS"
          link: "/signature/java/search/pps/"
          description: "Peragaan Slide Microsoft PowerPoint 97-2003"

        - name: "Cari Tanda Tangan di PPSX"
          link: "/signature/java/search/ppsx/"
          description: "PowerPoint Terbuka XML Slide Show"

        - name: "Cari Tanda Tangan di POTM"
          link: "/signature/java/search/potm/"
          description: "Templat Microsoft PowerPoint Macro-Enabled"

        - name: "Cari Tanda Tangan di POTX"
          link: "/signature/java/search/potx/"
          description: "Templat Microsoft PowerPoint"

        - name: "Cari Tanda Tangan di PPTM"
          link: "/signature/java/search/pptm/"
          description: "Presentasi Microsoft PowerPoint"

        - name: "Cari Tanda Tangan di ODP"
          link: "/signature/java/search/odp/"
          description: "Presentasi OpenDocument"

        - name: "Cari Tanda Tangan di OTP"
          link: "/signature/java/search/otp/"
          description: "Template Presentasi OpenDocument"

        - name: "Cari Tanda Tangan di WEBP"
          link: "/signature/java/search/webp/"
          description: "Gambar WebP"

        - name: "Cari Tanda Tangan di TIFF"
          link: "/signature/java/search/tiff/"
          description: "Format File Gambar yang Ditandai"

        - name: "Cari Tanda Tangan dalam format JPEG"
          link: "/signature/java/search/jpeg/"
          description: "Gambar JPEG"

        - name: "Cari Tanda Tangan di GIF"
          link: "/signature/java/search/gif/"
          description: "Format Pertukaran Grafik"

        - name: "Cari Tanda Tangan di PNG"
          link: "/signature/java/search/png/"
          description: "Grafik Jaringan Portabel"

        - name: "Cari Tanda Tangan di BMP"
          link: "/signature/java/search/bmp/"
          description: "Format File Bitmap"

        - name: "Cari Tanda Tangan di CDR"
          link: "/signature/java/search/cdr/"
          description: "Gambar Grafis Vektor CorelDraw"

        - name: "Cari Tanda Tangan di SVG"
          link: "/signature/java/search/svg/"
          description: "Grafik Vektor Skalabel"

        - name: "Cari Tanda Tangan di PSD"
          link: "/signature/java/search/psd/"
          description: "Dokumen Adobe Photoshop"

        - name: "Cari Tanda Tangan di WMF"
          link: "/signature/java/search/wmf/"
          description: "Metafile Windows"

        - name: "Cari Tanda Tangan di EMF"
          link: "/signature/java/search/emf/"
          description: "Format Metafile yang Ditingkatkan"

        - name: "Cari Tanda Tangan di CMX"
          link: "/signature/java/search/cmx/"
          description: "Corel Metafile eXchange Gambar"

        - name: "Cari Tanda Tangan di DJVU"
          link: "/signature/java/search/djvu/"
          description: "Deja Vu"

        - name: "Cari Tanda Tangan di PPSM"
          link: "/signature/java/search/ppsm/"
          description: "Peragaan Slide Berkemampuan Makro Microsoft PowerPoint"

        - name: "Cari Tanda Tangan di DCM"
          link: "/signature/java/search/dcm/"
          description: "Pencitraan Digital dan Komunikasi dalam Kedokteran"


back_to_top:
    enable: true
---
