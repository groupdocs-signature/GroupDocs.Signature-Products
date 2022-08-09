---
layout: "auto-gen"
date: 2022-07-07T12:44:18+03:00
draft: false

head_title: "Hapus Tanda Tangan Digital dari PNG di Java"
head_description: "Pustaka Java untuk menghapus &amp; hapus tanda tangan digital dari file PNG menggunakan GroupDocs.Signature API - memanipulasi Gambar, Kode Batang, Kode QR, Stempel, Teks, Optik &amp; Tanda tangan metadata dari dokumen yang ditandatangani secara digital."

title: "Hapus Tanda Tangan Digital dari PNG melalui Java"
description: "Pustaka Java eSignature untuk menghapus tanda tangan digital dari file PNG. Mudah memanipulasi tanda tangan Gambar, Barcode, QR-Code, Cap, Teks, Optik dan Metadata dari dokumen yang ditandatangani secara digital."
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
        [GroupDocs.Signature for Java](/id/signature/java/) adalah pustaka eSignature Java canggih untuk menandatangani dokumen secara digital menggunakan berbagai jenis tanda tangan seperti teks, gambar, kode batang, stempel, bidang formulir, kode QR, dan metadata. Dengan menambahkan hanya beberapa baris kode, perkuat aplikasi Java Anda dengan fitur untuk melihat, menambah, mengedit, memvalidasi, menghapus, dan mencari tanda tangan digital dalam PDF, Microsoft Word, lembar kerja Excel, presentasi PowerPoint, Adobe Photoshop, metafile, dan format file gambar. API tanda tangan elektronik juga mendukung fitur tambahan untuk menyesuaikan properti tanda tangan sesuai kebutuhan.

steps:
    enable: true
    title_left: "Cara Menghapus Tanda Tangan Digital dari PNG"
    content_left: |
        Contoh kode Java di bawah ini dengan jelas menunjukkan langkah-langkah untuk **menghapus tanda tangan teks dari file PNG di Java** dengan menambahkan beberapa baris kode saja.

        * Buat instance baru kelas **Signature** dan teruskan jalur dokumen sumber sebagai parameter konstruktor.
        * Buat instance objek **TextSearchOptions** dengan properti yang diinginkan.
        * Panggil metode **search** untuk mendapatkan daftar **TextSignatures**.
        * Pilih objek **TextSignature** yang harus dihapus dari dokumen.
        * Panggil metode **Signature** objek **delete**, berikan satu atau beberapa tanda tangan ke objek tersebut.
        * Analisis hasil **DeleteResult** untuk mengonfirmasi bahwa tanda tangan telah diperbarui atau tidak.
        
    title_right: "Persyaratan sistem"
    content_right: |
        GroupDocs.Signature untuk Java API didukung di semua platform dan sistem operasi utama. Sebelum menjalankan kode di bawah ini, pastikan Anda telah menginstal prasyarat berikut di sistem Anda.

        * Sistem Operasi: Microsoft Windows, Linux, MacOS
        * Lingkungan Pengembangan: Visual Studio, Xamarin, MonoDevelop
        * Kerangka: .NET Framework, .NET Standard, .NET Core, Mono
        * Unduh versi terbaru GroupDocs.Signature untuk Java dari [NuGet](https://www.nuget.org/packages/groupdocs.signature)
        
    code: |
        ```java
        // inisialisasi instance Tanda Tangan
        Signature signature = new Signature("signed.pdf");
         
        TextSearchOptions options = new TextSearchOptions();
         
        List signatures = signature.search(TextSignature.class,options);
        List signaturesToDelete = new ArrayList();
        // kumpulkan tanda tangan untuk dihapus
        for (TextSignature temp : signatures)
        {
            if (temp.getText().contains("JS"))
            {
                signaturesToDelete.add(temp);
            }
        }
        // hapus tanda tangan
        DeleteResult deleteResult = signature.delete("signed.png", signaturesToDelete);
        if (deleteResult.getSucceeded().size() == signaturesToDelete.size())
        {
            System.out.print("All signatures were successfully deleted!");
        }
        else
        {
            System.out.print("Successfully deleted signatures : " + deleteResult.getSucceeded().size());
            System.out.print("Not deleted signatures : " + deleteResult.getFailed().size());
        }
        System.out.print("List of deleted signatures:");
        for(BaseSignature temp : deleteResult.getSucceeded())
        {
            System.out.print("Signature# Id:"+temp.getSignatureId()+", Location: "+temp.getLeft()+"x"+temp.getTop()+". Size: "+temp.getWidth()+"x"+temp.getHeight());
        }
        ```
        
demos:
    enable: true
    title: "Hapus PNG Signature Live Demo"
    content: |
        Tambahkan file PNG tanda tangan elektronik sekarang juga dengan mengunjungi situs web [GroupDocs.Signature](https://products.groupdocs.app/signature/family).
        Demo langsung memiliki manfaat sebagai berikut
about_formats:
    enable: true
    format:
        - icon: "far fa-file-png"
          title: "Apa itu Format File PNG"
          content: |
            PNG, Portable Network Graphics, mengacu pada jenis format file gambar raster yang menggunakan kompresi tanpa kehilangan. Format file ini dibuat sebagai pengganti Graphics Interchange Format (GIF) dan tidak memiliki batasan hak cipta. Namun, format file PNG tidak mendukung animasi. Format file PNG mendukung kompresi gambar tanpa kehilangan yang membuatnya populer di kalangan penggunanya. Dengan berlalunya waktu, PNG telah berkembang sebagai salah satu format file gambar yang paling banyak digunakan. Hampir semua Sistem Operasi memiliki dukungan untuk membuka file PNG. Misalnya, penampil Microsoft Windows memiliki kemampuan untuk membuka file PNG karena OS secara default memiliki dukungan yang tersedia sebagai bagian dari penginstalan. Pelajari lebih lanjut tentang format file PNG

          link: "https://docs.fileformat.com/image/png/"

more_formats:
    enable: true
    title: "Pilihan Lain yang Tersedia"
    content: |
        API penghapusan tanda tangan digital multi-format untuk dokumen dan gambar. Hapus tanda tangan dari beberapa format file populer seperti yang dinyatakan di bawah ini.
    format: 
        - name: "Hapus Tanda Tangan dari PDF"
          link: "/signature/java/remove/pdf/"
          description: "Format Dokumen Portabel Adobe"

        - name: "Hapus Tanda Tangan dari DOC"
          link: "/signature/java/remove/doc/"
          description: "Dokumen Microsoft Word"

        - name: "Hapus Tanda Tangan dari DOCM"
          link: "/signature/java/remove/docm/"
          description: "Dokumen Berkemampuan Makro Microsoft Word"

        - name: "Hapus Tanda Tangan dari DOCX"
          link: "/signature/java/remove/docx/"
          description: "Microsoft Word Buka Dokumen XML"

        - name: "Hapus Tanda Tangan dari DOT"
          link: "/signature/java/remove/dot/"
          description: "Templat Dokumen Microsoft Word"

        - name: "Hapus Tanda Tangan dari DOTX"
          link: "/signature/java/remove/dotx/"
          description: "Templat Dokumen XML Word Terbuka"

        - name: "Hapus Tanda Tangan dari DOTM"
          link: "/signature/java/remove/dotm/"
          description: "Templat Microsoft Word Macro-Enabled"

        - name: "Hapus Tanda Tangan dari RTF"
          link: "/signature/java/remove/rtf/"
          description: "Dokumen Teks Kaya"

        - name: "Hapus Tanda Tangan dari ODT"
          link: "/signature/java/remove/odt/"
          description: "Buka Teks Dokumen"

        - name: "Hapus Tanda Tangan dari OTT"
          link: "/signature/java/remove/ott/"
          description: "Templat Teks OpenDocument"

        - name: "Hapus Tanda Tangan dari XLS"
          link: "/signature/java/remove/xls/"
          description: "Format File Biner Microsoft Excel"

        - name: "Hapus Tanda Tangan dari XLSX"
          link: "/signature/java/remove/xlsx/"
          description: "Microsoft Excel Buka XML Spreadsheet"

        - name: "Hapus Tanda Tangan dari XLSM"
          link: "/signature/java/remove/xlsm/"
          description: "Spreadsheet Berkemampuan Makro Microsoft Excel"

        - name: "Hapus Tanda Tangan dari XLSM"
          link: "/signature/java/remove/xlsm/"
          description: "Spreadsheet Berkemampuan Makro Microsoft Excel"

        - name: "Hapus Tanda Tangan dari XLSB"
          link: "/signature/java/remove/xlsb/"
          description: "Lembar Kerja Biner Microsoft Excel"

        - name: "Hapus Tanda Tangan dari XLTX"
          link: "/signature/java/remove/xltx/"
          description: "Templat Microsoft Excel"

        - name: "Hapus Tanda Tangan dari XLTM"
          link: "/signature/java/remove/xltm/"
          description: "Templat berkemampuan makro Microsoft Excel"

        - name: "Hapus Tanda Tangan dari ODS"
          link: "/signature/java/remove/ods/"
          description: "Buka Spreadsheet Dokumen"

        - name: "Hapus Tanda Tangan dari OTS"
          link: "/signature/java/remove/ots/"
          description: "Templat Spreadsheet OpenDocument"

        - name: "Hapus Tanda Tangan dari PPT"
          link: "/signature/java/remove/ppt/"
          description: "Presentasi powerpoint"

        - name: "Hapus Tanda Tangan dari PPTX"
          link: "/signature/java/remove/pptx/"
          description: "Presentasi PowerPoint Terbuka XML"

        - name: "Hapus Tanda Tangan dari PPS"
          link: "/signature/java/remove/pps/"
          description: "Peragaan Slide Microsoft PowerPoint 97-2003"

        - name: "Hapus Tanda Tangan dari PPSX"
          link: "/signature/java/remove/ppsx/"
          description: "PowerPoint Terbuka XML Slide Show"

        - name: "Hapus Tanda Tangan dari POTM"
          link: "/signature/java/remove/potm/"
          description: "Templat Microsoft PowerPoint Macro-Enabled"

        - name: "Hapus Tanda Tangan dari POTX"
          link: "/signature/java/remove/potx/"
          description: "Templat Microsoft PowerPoint"

        - name: "Hapus Tanda Tangan dari PPTM"
          link: "/signature/java/remove/pptm/"
          description: "Presentasi Microsoft PowerPoint"

        - name: "Hapus Tanda Tangan dari ODP"
          link: "/signature/java/remove/odp/"
          description: "Presentasi OpenDocument"

        - name: "Hapus Tanda Tangan dari OTP"
          link: "/signature/java/remove/otp/"
          description: "Template Presentasi OpenDocument"

        - name: "Hapus Tanda Tangan dari WEBP"
          link: "/signature/java/remove/webp/"
          description: "Gambar WebP"

        - name: "Hapus Tanda Tangan dari TIFF"
          link: "/signature/java/remove/tiff/"
          description: "Format File Gambar yang Ditandai"

        - name: "Hapus Tanda Tangan dari JPEG"
          link: "/signature/java/remove/jpeg/"
          description: "Gambar JPEG"

        - name: "Hapus Tanda Tangan dari GIF"
          link: "/signature/java/remove/gif/"
          description: "Format Pertukaran Grafik"

        - name: "Hapus Tanda Tangan dari PNG"
          link: "/signature/java/remove/png/"
          description: "Grafik Jaringan Portabel"

        - name: "Hapus Tanda Tangan dari BMP"
          link: "/signature/java/remove/bmp/"
          description: "Format File Bitmap"

        - name: "Hapus Tanda Tangan dari CDR"
          link: "/signature/java/remove/cdr/"
          description: "Gambar Grafis Vektor CorelDraw"

        - name: "Hapus Tanda Tangan dari SVG"
          link: "/signature/java/remove/svg/"
          description: "Grafik Vektor Skalabel"

        - name: "Hapus Tanda Tangan dari PSD"
          link: "/signature/java/remove/psd/"
          description: "Dokumen Adobe Photoshop"

        - name: "Hapus Tanda Tangan dari WMF"
          link: "/signature/java/remove/wmf/"
          description: "Metafile Windows"

        - name: "Hapus Tanda Tangan dari EMF"
          link: "/signature/java/remove/emf/"
          description: "Format Metafile yang Ditingkatkan"

        - name: "Hapus Tanda Tangan dari CMX"
          link: "/signature/java/remove/cmx/"
          description: "Corel Metafile eXchange Gambar"

        - name: "Hapus Tanda Tangan dari DJVU"
          link: "/signature/java/remove/djvu/"
          description: "Deja Vu"

        - name: "Hapus Tanda Tangan dari PPSM"
          link: "/signature/java/remove/ppsm/"
          description: "Peragaan Slide Berkemampuan Makro Microsoft PowerPoint"

        - name: "Hapus Tanda Tangan dari DCM"
          link: "/signature/java/remove/dcm/"
          description: "Pencitraan Digital dan Komunikasi dalam Kedokteran"


back_to_top:
    enable: true
---
