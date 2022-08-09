---
layout: "auto-gen"
date: 2022-07-07T12:44:18+03:00
draft: false

head_title: "Contoh Kode Java untuk Melihat &amp; Edit Tanda Tangan Digital dari WORD File"
head_description: "Contoh kode Java untuk melihat dan mengedit tanda tangan digital dari file WORD menggunakan GroupDocs.Siganture API - tambahkan tanda tangan elektronik khusus ke dokumen bisnis populer dan format file gambar."

title: "Edit Tanda Tangan Digital di WORD melalui Java"
description: "Pustaka Java untuk melihat &amp; mengedit tanda tangan digital dalam file WORD menggunakan jenis tanda tangan elektronik populer. Kelola properti WORD dan sesuaikan opsi penandatanganan dalam dokumen dan gambar."
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
        [GroupDocs.Signature for Java](/id/signature/java/) adalah pustaka Java canggih untuk menandatangani dokumen secara digital menggunakan berbagai jenis tanda tangan seperti teks, gambar, kode batang, stempel, bidang formulir, kode QR, dan metadata. Dengan menambahkan hanya beberapa baris kode, perkuat aplikasi Java Anda dengan fitur untuk melihat, menambah, memperbarui, memvalidasi, menghapus, dan mencari tanda tangan digital dalam PDF, Microsoft WORD, lembar kerja Excel, presentasi PowerPoint, Adobe Photoshop, metafile, dan format file gambar. API tanda tangan elektronik juga mendukung fitur tambahan untuk menyesuaikan properti tanda tangan sesuai kebutuhan.

steps:
    enable: true
    title_left: "Cara Mengedit Tanda Tangan Digital di WORD"
    content_left: |
        Contoh kode di bawah ini dengan jelas menunjukkan langkah-langkah tentang **cara mengedit tanda tangan digital dalam file WORD yang sudah ditandatangani di Java** menggunakan pustaka [GroupDocs.Signature](/id/signature/java/) dengan menambahkan beberapa baris kode saja.

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
                boolean result = signature.update("sampleSigned-output.word",imageSignature);
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
    title: "Edit WORD Signature Live Demo"
    content: |
        Tambahkan file WORD tanda tangan elektronik sekarang juga dengan mengunjungi situs web [GroupDocs.Signature](https://products.groupdocs.app/signature/family).
        Demo langsung memiliki manfaat sebagai berikut
about_formats:
    enable: true
    format:
        - icon: "far fa-file-word"
          title: "Apa itu Format File WORD"
          content: |
            File pemrosesan WORD berisi informasi pengguna dalam format teks biasa atau teks kaya. Format file teks biasa berisi teks yang tidak diformat dan tidak ada pengaturan font atau halaman, dll. yang dapat diterapkan. Sebaliknya, format file teks kaya memungkinkan opsi pemformatan seperti pengaturan jenis font, gaya (tebal, miring, garis bawah, dll.), margin halaman, judul, poin dan angka, dan beberapa fitur pemformatan lainnya. Penggunaan file teks biasa telah berkurang secara signifikan dengan berlalunya waktu karena ada komputer dan program yang lebih kuat yang tersedia untuk menawarkan pemrosesan file teks kaya. Microsoft WORD untuk Windows, Mac, iOS dan Android adalah prosesor WORD yang kuat yang dapat membuka, membaca, dan mengedit format file dokumen tersebut selain editor teks lainnya. Ekstensi file teks biasa yang umum dan format file terkait termasuk TXT, CSV, sedangkan ekstensi file untuk dokumen teks kaya termasuk DOCX, DOC, dan RTF. Pelajari lebih lanjut tentang format file WORD

          link: "https://docs.fileformat.com/word-processing/"

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
          description: "Dokumen Microsoft WORD"

        - name: "Edit tanda tangan elektronik dari DOCM"
          link: "/signature/java/edit/docm/"
          description: "Dokumen Microsoft WORD Macro-Enabled"

        - name: "Edit tanda tangan elektronik dari DOCX"
          link: "/signature/java/edit/docx/"
          description: "Microsoft WORD Buka Dokumen XML"

        - name: "Edit tanda tangan elektronik dari DOT"
          link: "/signature/java/edit/dot/"
          description: "Templat Dokumen Microsoft WORD"

        - name: "Edit tanda tangan elektronik dari DOTX"
          link: "/signature/java/edit/dotx/"
          description: "WORD Buka Templat Dokumen XML"

        - name: "Edit tanda tangan elektronik dari DOTM"
          link: "/signature/java/edit/dotm/"
          description: "Template Microsoft WORD Macro-Enabled"

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
          description: "Lembar Kerja Biner Microsoft Excel"

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
