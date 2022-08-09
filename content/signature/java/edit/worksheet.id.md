---
layout: "auto-gen"
date: 2022-07-07T12:44:18+03:00
draft: false

head_title: "Contoh Kode Java untuk Melihat &amp; Edit Tanda Tangan Digital dari WORKSHEET File"
head_description: "Contoh kode Java untuk melihat dan mengedit tanda tangan digital dari file WORKSHEET menggunakan GroupDocs.Siganture API - tambahkan tanda tangan elektronik khusus ke dokumen bisnis populer dan format file gambar."

title: "Edit Tanda Tangan Digital di WORKSHEET melalui Java"
description: "Pustaka Java untuk melihat &amp; mengedit tanda tangan digital dalam file WORKSHEET menggunakan jenis tanda tangan elektronik populer. Kelola properti WORKSHEET dan sesuaikan opsi penandatanganan dalam dokumen dan gambar."
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
        [GroupDocs.Signature for Java](/id/signature/java/) adalah pustaka Java canggih untuk menandatangani dokumen secara digital menggunakan berbagai jenis tanda tangan seperti teks, gambar, kode batang, stempel, bidang formulir, kode QR, dan metadata. Dengan menambahkan hanya beberapa baris kode, perkuat aplikasi Java Anda dengan fitur untuk melihat, menambah, memperbarui, memvalidasi, menghapus, dan mencari tanda tangan digital dalam PDF, Microsoft Word, lembar kerja Excel, presentasi PowerPoint, Adobe Photoshop, metafile, dan format file gambar. API tanda tangan elektronik juga mendukung fitur tambahan untuk menyesuaikan properti tanda tangan sesuai kebutuhan.

steps:
    enable: true
    title_left: "Cara Mengedit Tanda Tangan Digital di WORKSHEET"
    content_left: |
        Contoh kode di bawah ini dengan jelas menunjukkan langkah-langkah tentang **cara mengedit tanda tangan digital dalam file WORKSHEET yang sudah ditandatangani di Java** menggunakan pustaka [GroupDocs.Signature](/id/signature/java/) dengan menambahkan beberapa baris kode saja.

        * Buat instance baru dari kelas [Signature](https://apireference.groupdocs.com/signature/java/com.groupdocs.signature/Signature) dan teruskan jalur dokumen sumber sebagai parameter konstruktor.
        * Buat instance [ImageSearchOptions](https://apireference.groupdocs.com/signature/java/com.groupdocs.signature.options.search/ImageSearchOptions) objek dengan properti yang diinginkan.
        * Hubungi [search](https://apireference.groupdocs.com/signature/java/com.groupdocs.signature/Signature#search(java.lang.Class,%20com.groupdocs.signature.options.search.SearchOptions)) metode untuk mendapatkan daftar [ImageSignatures](https://apireference.groupdocs.com/signature/java/com.groupdocs.signature.domain.signatures/ImageSignature).
        * Pilih dari daftar [ImageSignature](https://apireference.groupdocs.com/signature/java/com.groupdocs.signature.domain.signatures/ImageSignature) objek yang harus diperbarui.
        * Panggil objek [Signature](https://apireference.groupdocs.com/signature/java/com.groupdocs.signature/Signature) [update](https://apireference.groupdocs.com/signature/java/com.groupdocs .signature/Signature#update(java.io.OutputStream,%20com.groupdocs.signature.domain.signatures.BaseSignature)) dan berikan satu atau beberapa tanda tangan ke sana.
        
    title_right: "Persyaratan sistem"
    content_right: |
        GroupDocs.Signature untuk Java API didukung di semua platform dan sistem operasi utama. Sebelum menjalankan kode di bawah ini, pastikan Anda telah menginstal prasyarat berikut di sistem Anda.

        * Sistem Operasi: Microsoft Windows, Linux, MacOS
        * Lingkungan Pengembangan: Visual Studio, Xamarin, MonoDevelop
        * Kerangka: .NET Framework, .NET Standard, .NET Core, Mono
        * Unduh versi terbaru GroupDocs.Signature untuk Java dari [NuGet](https://www.nuget.org/packages/groupdocs.signature)
        
    code: |
        ```java
        Signature signature = new Signature("sampleSigned.pdf");
        try 
        {
            ImageSearchOptions options = new ImageSearchOptions();
        
            // mencari tanda tangan gambar dalam dokumen
            List signatures = signature.search(ImageSignature.class,options);
            if (signatures.size() > 0)
            {
                ImageSignature imageSignature = signatures.get(0);
                imageSignature.setLeft(100);
                imageSignature.setTop(100);
                boolean result = signature.update("sampleSigned-output.worksheet",imageSignature);
                if (result)
                {
                    System.out.print("Image signature at location " + imageSignature.getLeft() + "x" + imageSignature.getTop() + " and Size " + imageSignature.getSize() + " was updated in the document [" + fileName + ".");
                }
                else
                {
                    System.out.print("Signature was not updated in the document! Signature at location " + imageSignature.getLeft() + "x" + imageSignature.getTop() + " and Size " + imageSignature.getSize() + " was not found!");
                }
            }
        } catch (Exception e) {
            throw new GroupDocsSignatureException(e.getMessage());
        }
        ```
        
demos:
    enable: true
    title: "Edit WORKSHEET Signature Live Demo"
    content: |
        Tambahkan file WORKSHEET tanda tangan elektronik sekarang juga dengan mengunjungi situs web [GroupDocs.Signature](https://products.groupdocs.app/signature/family).
        Demo langsung memiliki manfaat sebagai berikut
about_formats:
    enable: true
    format:
        - icon: "far fa-file-worksheet"
          title: "Apa itu Format File WORKSHEET"
          content: |
            File spreadsheet berisi data dalam bentuk baris dan kolom. Anda dapat membuka, melihat, dan mengedit file tersebut menggunakan aplikasi perangkat lunak spreadsheet seperti Microsoft Excel yang sekarang tersedia untuk sistem operasi Windows dan MacOS. Demikian pula, Google sheets adalah alat pembuat dan pengeditan spreadsheet online gratis yang berfungsi dari browser web apa pun. File spreadsheet dapat disimpan dalam beberapa format file yang berbeda, masing-masing memiliki ekstensi file yang berbeda untuk representasi yang unik. Data disimpan dalam sel baik dalam bentuk biasa seperti string teks, angka, tanggal, mata uang, dll. Atau sebagai rumus yang mengubah nilai sel saat nilai sel yang direferensikan berubah. Ekstensi file spreadsheet umum dan format filenya termasuk XLSX (Microsoft Excel Open XML Spreadsheet), ODS (OpenDocument Spreadsheet) dan XLS (Microsoft Excel Binary File Format). Pelajari lebih lanjut tentang format file WORKSHEET

          link: "https://docs.fileformat.com/spreadsheet/"

more_formats:
    enable: true
    title: "Pilihan Lain yang Tersedia"
    content: |
        API pengeditan tanda tangan digital multi-format untuk dokumen dan gambar. Perbarui tanda tangan dari beberapa format file populer seperti yang dinyatakan di bawah ini.
    format: 
        - name: "Edit tanda tangan elektronik dari PDF"
          link: "/signature/java/edit/pdf/"
          description: "Format Dokumen Portabel Adobe"

        - name: "Edit tanda tangan elektronik dari DOC"
          link: "/signature/java/edit/doc/"
          description: "Dokumen Microsoft Word"

        - name: "Edit tanda tangan elektronik dari DOCM"
          link: "/signature/java/edit/docm/"
          description: "Dokumen Berkemampuan Makro Microsoft Word"

        - name: "Edit tanda tangan elektronik dari DOCX"
          link: "/signature/java/edit/docx/"
          description: "Microsoft Word Buka Dokumen XML"

        - name: "Edit tanda tangan elektronik dari DOT"
          link: "/signature/java/edit/dot/"
          description: "Templat Dokumen Microsoft Word"

        - name: "Edit tanda tangan elektronik dari DOTX"
          link: "/signature/java/edit/dotx/"
          description: "Templat Dokumen XML Word Terbuka"

        - name: "Edit tanda tangan elektronik dari DOTM"
          link: "/signature/java/edit/dotm/"
          description: "Templat Microsoft Word Macro-Enabled"

        - name: "Edit tanda tangan elektronik dari RTF"
          link: "/signature/java/edit/rtf/"
          description: "Dokumen Teks Kaya"

        - name: "Edit tanda tangan elektronik dari ODT"
          link: "/signature/java/edit/odt/"
          description: "Buka Teks Dokumen"

        - name: "Edit tanda tangan elektronik dari OTT"
          link: "/signature/java/edit/ott/"
          description: "Templat Teks OpenDocument"

        - name: "Edit tanda tangan elektronik dari XLS"
          link: "/signature/java/edit/xls/"
          description: "Format File Biner Microsoft Excel"

        - name: "Edit tanda tangan elektronik dari XLSX"
          link: "/signature/java/edit/xlsx/"
          description: "Microsoft Excel Buka XML Spreadsheet"

        - name: "Edit tanda tangan elektronik dari XLSM"
          link: "/signature/java/edit/xlsm/"
          description: "Spreadsheet Berkemampuan Makro Microsoft Excel"

        - name: "Edit tanda tangan elektronik dari XLSM"
          link: "/signature/java/edit/xlsm/"
          description: "Spreadsheet Berkemampuan Makro Microsoft Excel"

        - name: "Edit tanda tangan elektronik dari XLSB"
          link: "/signature/java/edit/xlsb/"
          description: "Microsoft Excel Biner WORKSHEET"

        - name: "Edit tanda tangan elektronik dari XLTX"
          link: "/signature/java/edit/xltx/"
          description: "Templat Microsoft Excel"

        - name: "Edit tanda tangan elektronik dari XLTM"
          link: "/signature/java/edit/xltm/"
          description: "Templat berkemampuan makro Microsoft Excel"

        - name: "Edit tanda tangan elektronik dari ODS"
          link: "/signature/java/edit/ods/"
          description: "Buka Spreadsheet Dokumen"

        - name: "Edit tanda tangan elektronik dari OTS"
          link: "/signature/java/edit/ots/"
          description: "Templat Spreadsheet OpenDocument"

        - name: "Edit tanda tangan elektronik dari PPT"
          link: "/signature/java/edit/ppt/"
          description: "Presentasi powerpoint"

        - name: "Edit tanda tangan elektronik dari PPTX"
          link: "/signature/java/edit/pptx/"
          description: "Presentasi PowerPoint Terbuka XML"

        - name: "Edit tanda tangan elektronik dari PPS"
          link: "/signature/java/edit/pps/"
          description: "Peragaan Slide Microsoft PowerPoint 97-2003"

        - name: "Edit tanda tangan elektronik dari PPSX"
          link: "/signature/java/edit/ppsx/"
          description: "PowerPoint Terbuka XML Slide Show"

        - name: "Edit tanda tangan elektronik dari POTM"
          link: "/signature/java/edit/potm/"
          description: "Templat Microsoft PowerPoint Macro-Enabled"

        - name: "Edit tanda tangan elektronik dari POTX"
          link: "/signature/java/edit/potx/"
          description: "Templat Microsoft PowerPoint"

        - name: "Edit tanda tangan elektronik dari PPTM"
          link: "/signature/java/edit/pptm/"
          description: "Presentasi Microsoft PowerPoint"

        - name: "Edit tanda tangan elektronik dari ODP"
          link: "/signature/java/edit/odp/"
          description: "Presentasi OpenDocument"

        - name: "Edit tanda tangan elektronik dari OTP"
          link: "/signature/java/edit/otp/"
          description: "Template Presentasi OpenDocument"

        - name: "Edit tanda tangan elektronik dari WEBP"
          link: "/signature/java/edit/webp/"
          description: "Gambar WebP"

        - name: "Edit tanda tangan elektronik dari TIFF"
          link: "/signature/java/edit/tiff/"
          description: "Format File Gambar yang Ditandai"

        - name: "Edit tanda tangan elektronik dari JPEG"
          link: "/signature/java/edit/jpeg/"
          description: "Gambar JPEG"

        - name: "Edit tanda tangan elektronik dari GIF"
          link: "/signature/java/edit/gif/"
          description: "Format Pertukaran Grafik"

        - name: "Edit tanda tangan elektronik dari PNG"
          link: "/signature/java/edit/png/"
          description: "Grafik Jaringan Portabel"

        - name: "Edit tanda tangan elektronik dari BMP"
          link: "/signature/java/edit/bmp/"
          description: "Format File Bitmap"

        - name: "Edit tanda tangan elektronik dari CDR"
          link: "/signature/java/edit/cdr/"
          description: "Gambar Grafis Vektor CorelDraw"

        - name: "Edit tanda tangan elektronik dari SVG"
          link: "/signature/java/edit/svg/"
          description: "Grafik Vektor Skalabel"

        - name: "Edit tanda tangan elektronik dari PSD"
          link: "/signature/java/edit/psd/"
          description: "Dokumen Adobe Photoshop"

        - name: "Edit tanda tangan elektronik dari WMF"
          link: "/signature/java/edit/wmf/"
          description: "Metafile Windows"

        - name: "Edit tanda tangan elektronik dari EMF"
          link: "/signature/java/edit/emf/"
          description: "Format Metafile yang Ditingkatkan"

        - name: "Edit tanda tangan elektronik dari CMX"
          link: "/signature/java/edit/cmx/"
          description: "Corel Metafile eXchange Gambar"

        - name: "Edit tanda tangan elektronik dari DJVU"
          link: "/signature/java/edit/djvu/"
          description: "Deja Vu"

        - name: "Edit tanda tangan elektronik dari PPSM"
          link: "/signature/java/edit/ppsm/"
          description: "Peragaan Slide Berkemampuan Makro Microsoft PowerPoint"

        - name: "Edit tanda tangan elektronik dari DCM"
          link: "/signature/java/edit/dcm/"
          description: "Pencitraan Digital dan Komunikasi dalam Kedokteran"


back_to_top:
    enable: true
---
