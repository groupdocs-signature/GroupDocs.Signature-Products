---
layout: "auto-gen"
date: 2022-07-07T12:44:18+03:00
draft: false

head_title: "Cara Menambahkan Tanda Tangan Digital ke File SPREADSHEET di Java"
head_description: "Pelajari cara menambahkan tanda tangan digital ke file SPREADSHEET di Java menggunakan GroupDocs.Siganture API - tambahkan tanda tangan elektronik khusus ke dokumen bisnis populer dan format file gambar."

title: "Tambahkan Tanda Tangan Digital ke SPREADSHEET di Java"
description: "Amankan file SPREADSHEET Anda dengan menambahkan jenis tanda tangan digital populer menggunakan perpustakaan Java. Memanipulasi properti tanda tangan elektronik dan mengatur opsi penandatanganan sebelumnya dalam dokumen yang mungkin Anda perlukan."
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
        [GroupDocs.Signature for Java](/id/signature/java/) adalah pustaka Java canggih untuk menandatangani dokumen secara digital menggunakan berbagai jenis tanda tangan seperti teks, gambar, kode batang, stempel, bidang formulir, kode QR, dan metadata. Dengan menambahkan hanya beberapa baris kode, perkuat aplikasi Java Anda dengan fitur untuk menambah, mengedit, memverifikasi, menghapus, dan mencari tanda tangan digital dalam PDF, Microsoft Word, lembar kerja Excel, presentasi PowerPoint, Adobe Photoshop, metafile, dan format file gambar. API tanda tangan elektronik juga mendukung fitur tambahan untuk menyesuaikan properti tanda tangan sesuai kebutuhan.

steps:
    enable: true
    title_left: "Cara Menambahkan Tanda Tangan Digital dalam File SPREADSHEET"
    content_left: |
        Contoh kode di bawah ini dengan jelas menunjukkan langkah-langkah tentang **cara menambahkan tanda tangan digital ke file SPREADSHEET menggunakan pustaka [GroupDocs.Signature](/id/signature/java/) di Java** dengan menambahkan beberapa baris kode saja.

        * Buat instance baru dari kelas [Signature](https://apireference.groupdocs.com/java/signature/com.groupdocs.signature/Signature) dan teruskan jalur dokumen sumber sebagai parameter konstruktor.
        * Buat instance objek [DigitalSignOptions](https://apireference.groupdocs.com/java/signature/com.groupdocs.signature.options.sign/DigitalSignOptions) dengan sertifikat & kata sandi yang diperlukan.
        * Hubungi [Sign](https://apireference.groupdocs.com/java/signature/com.groupdocs.signature/Signature#sign(java.io.OutputStream,%20com.groupdocs.signature.options.sign.SignOptions)) metode instance kelas [Signature](https://apireference.groupdocs.com/java/signature/com.groupdocs.signature/Signature); berikan DigitalSignOptions ke sana.
        * Analisis hasil [SignResult](https://apireference.groupdocs.com/java/signature/com.groupdocs.signature.domain/SignResult) untuk memeriksa tanda tangan yang baru dibuat jika diperlukan.
        
    title_right: "Persyaratan sistem"
    content_right: |
        GroupDocs.Signature untuk Java API didukung di semua platform dan sistem operasi utama. Sebelum menjalankan kode di bawah ini, pastikan Anda telah menginstal prasyarat berikut di sistem Anda.

        * Sistem Operasi: Microsoft Windows, Linux, MacOS
        * Lingkungan Pengembangan: Visual Studio, Xamarin, MonoDevelop
        * Kerangka: .NET Framework, .NET Standard, .NET Core, Mono
        * Unduh versi terbaru GroupDocs.Signature untuk Java dari [NuGet](https://www.nuget.org/packages/groupdocs.signature)
        
    code: |
        ```java
        Signature signature = new Signature("sample.pdf"); 
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");
         
        // sertifikasi kata sandi
        options.setPassword("1234567890");
        // detail sertifikat digital
        options.setReason("Sign");
        options.setContact("JohnSmith");
        options.setLocation("Office1");
         
        // gambar sebagai tampilan sertifikat digital pada halaman dokumen
        options.setImageFilePath("sample.jpg");
        //
        options.setAllPages(true);
        options.setWidth(80);
        options.setHeight(60);
        options.setVerticalAlignment(VerticalAlignment.Bottom);
        options.setHorizontalAlignment(HorizontalAlignment.Right);
        Padding padding = new Padding();
        padding.setBottom(10);
        padding.setRight(10);
        options.setMargin(padding);
         
        SignResult signResult = signature.sign("signed.spreadsheet", options);
        // menganalisis hasil
        System.out.print("List of newly created signatures:");
        int number = 1;
        for(BaseSignature temp : signResult.getSucceeded())
        {
            System.out.print("Signature #"+ number++ +": Type: "+temp.getSignatureType()+" Id:"+temp.getSignatureId()+
                    ",Location: "+temp.getLeft()+"x"+temp.getTop()+". Size: "+temp.getWidth()+"x"+temp.getHeight());
        }
        ```
        
demos:
    enable: true
    title: "Tambahkan SPREADSHEET Signature Live Demo"
    content: |
        Tambahkan file SPREADSHEET tanda tangan elektronik sekarang juga dengan mengunjungi situs web [GroupDocs.Signature](https://products.groupdocs.app/signature/family).
        Demo langsung memiliki manfaat sebagai berikut
about_formats:
    enable: true
    format:
        - icon: "far fa-file-spreadsheet"
          title: "Apa itu Format File SPREADSHEET"
          content: |
            File SPREADSHEET berisi data dalam bentuk baris dan kolom. Anda dapat membuka, melihat, dan mengedit file tersebut menggunakan aplikasi perangkat lunak SPREADSHEET seperti Microsoft Excel yang sekarang tersedia untuk sistem operasi Windows dan MacOS. Demikian pula, Google sheets adalah alat pembuat dan pengeditan SPREADSHEET online gratis yang berfungsi dari browser web apa pun. File SPREADSHEET dapat disimpan dalam beberapa format file yang berbeda, masing-masing memiliki ekstensi file yang berbeda untuk representasi yang unik. Data disimpan dalam sel baik dalam bentuk biasa seperti string teks, angka, tanggal, mata uang, dll. Atau sebagai rumus yang mengubah nilai sel saat nilai sel yang direferensikan berubah. Ekstensi file SPREADSHEET umum dan format filenya termasuk XLSX (Microsoft Excel Open XML SPREADSHEET), ODS (OpenDocument SPREADSHEET) dan XLS (Microsoft Excel Binary File Format). Pelajari lebih lanjut tentang format file SPREADSHEET

          link: "https://docs.fileformat.com/spreadsheet/"

more_formats:
    enable: true
    title: "Pilihan Lain yang Tersedia"
    content: |
        API tanda tangan digital multi-format untuk dokumen dan gambar. Tambahkan tanda tangan ke beberapa format file populer seperti yang dinyatakan di bawah ini.
    format: 
        - name: "Tambahkan tanda tangan elektronik ke PDF"
          link: "/signature/java/add/pdf/"
          description: "Format Dokumen Portabel Adobe"

        - name: "Tambahkan tanda tangan elektronik ke DOC"
          link: "/signature/java/add/doc/"
          description: "Dokumen Microsoft Word"

        - name: "Tambahkan tanda tangan elektronik ke DOCM"
          link: "/signature/java/add/docm/"
          description: "Dokumen Berkemampuan Makro Microsoft Word"

        - name: "Tambahkan tanda tangan elektronik ke DOCX"
          link: "/signature/java/add/docx/"
          description: "Microsoft Word Buka Dokumen XML"

        - name: "Tambahkan tanda tangan elektronik ke DOT"
          link: "/signature/java/add/dot/"
          description: "Templat Dokumen Microsoft Word"

        - name: "Tambahkan tanda tangan elektronik ke DOTX"
          link: "/signature/java/add/dotx/"
          description: "Templat Dokumen XML Word Terbuka"

        - name: "Tambahkan tanda tangan elektronik ke DOTM"
          link: "/signature/java/add/dotm/"
          description: "Templat Microsoft Word Macro-Enabled"

        - name: "Tambahkan tanda tangan elektronik ke RTF"
          link: "/signature/java/add/rtf/"
          description: "Dokumen Teks Kaya"

        - name: "Tambahkan tanda tangan elektronik ke ODT"
          link: "/signature/java/add/odt/"
          description: "Buka Teks Dokumen"

        - name: "Tambahkan tanda tangan elektronik ke OTT"
          link: "/signature/java/add/ott/"
          description: "Templat Teks OpenDocument"

        - name: "Tambahkan tanda tangan elektronik ke XLS"
          link: "/signature/java/add/xls/"
          description: "Format File Biner Microsoft Excel"

        - name: "Tambahkan tanda tangan elektronik ke XLSX"
          link: "/signature/java/add/xlsx/"
          description: "Microsoft Excel Buka XML SPREADSHEET"

        - name: "Tambahkan tanda tangan elektronik ke XLSM"
          link: "/signature/java/add/xlsm/"
          description: "Microsoft Excel Makro-Diaktifkan SPREADSHEET"

        - name: "Tambahkan tanda tangan elektronik ke XLSM"
          link: "/signature/java/add/xlsm/"
          description: "Microsoft Excel Makro-Diaktifkan SPREADSHEET"

        - name: "Tambahkan tanda tangan elektronik ke XLSB"
          link: "/signature/java/add/xlsb/"
          description: "Lembar Kerja Biner Microsoft Excel"

        - name: "Tambahkan tanda tangan elektronik ke XLTX"
          link: "/signature/java/add/xltx/"
          description: "Templat Microsoft Excel"

        - name: "Tambahkan tanda tangan elektronik ke XLTM"
          link: "/signature/java/add/xltm/"
          description: "Templat berkemampuan makro Microsoft Excel"

        - name: "Tambahkan tanda tangan elektronik ke ODS"
          link: "/signature/java/add/ods/"
          description: "Buka Dokumen SPREADSHEET"

        - name: "Tambahkan tanda tangan elektronik ke OTS"
          link: "/signature/java/add/ots/"
          description: "Templat SPREADSHEET Dokumen Terbuka"

        - name: "Tambahkan tanda tangan elektronik ke PPT"
          link: "/signature/java/add/ppt/"
          description: "Presentasi powerpoint"

        - name: "Tambahkan tanda tangan elektronik ke PPTX"
          link: "/signature/java/add/pptx/"
          description: "Presentasi PowerPoint Terbuka XML"

        - name: "Tambahkan tanda tangan elektronik ke PPS"
          link: "/signature/java/add/pps/"
          description: "Peragaan Slide Microsoft PowerPoint 97-2003"

        - name: "Tambahkan tanda tangan elektronik ke PPSX"
          link: "/signature/java/add/ppsx/"
          description: "PowerPoint Terbuka XML Slide Show"

        - name: "Tambahkan tanda tangan elektronik ke POTM"
          link: "/signature/java/add/potm/"
          description: "Templat Microsoft PowerPoint Macro-Enabled"

        - name: "Tambahkan tanda tangan elektronik ke POTX"
          link: "/signature/java/add/potx/"
          description: "Templat Microsoft PowerPoint"

        - name: "Tambahkan tanda tangan elektronik ke PPTM"
          link: "/signature/java/add/pptm/"
          description: "Presentasi Microsoft PowerPoint"

        - name: "Tambahkan tanda tangan elektronik ke ODP"
          link: "/signature/java/add/odp/"
          description: "Presentasi OpenDocument"

        - name: "Tambahkan tanda tangan elektronik ke OTP"
          link: "/signature/java/add/otp/"
          description: "Template Presentasi OpenDocument"

        - name: "Tambahkan tanda tangan elektronik ke WEBP"
          link: "/signature/java/add/webp/"
          description: "Gambar WebP"

        - name: "Tambahkan tanda tangan elektronik ke TIFF"
          link: "/signature/java/add/tiff/"
          description: "Format File Gambar yang Ditandai"

        - name: "Tambahkan tanda tangan elektronik ke JPEG"
          link: "/signature/java/add/jpeg/"
          description: "Gambar JPEG"

        - name: "Tambahkan tanda tangan elektronik ke GIF"
          link: "/signature/java/add/gif/"
          description: "Format Pertukaran Grafik"

        - name: "Tambahkan tanda tangan elektronik ke PNG"
          link: "/signature/java/add/png/"
          description: "Grafik Jaringan Portabel"

        - name: "Tambahkan tanda tangan elektronik ke BMP"
          link: "/signature/java/add/bmp/"
          description: "Format File Bitmap"

        - name: "Tambahkan tanda tangan elektronik ke CDR"
          link: "/signature/java/add/cdr/"
          description: "Gambar Grafis Vektor CorelDraw"

        - name: "Tambahkan tanda tangan elektronik ke SVG"
          link: "/signature/java/add/svg/"
          description: "Grafik Vektor Skalabel"

        - name: "Tambahkan tanda tangan elektronik ke PSD"
          link: "/signature/java/add/psd/"
          description: "Dokumen Adobe Photoshop"

        - name: "Tambahkan tanda tangan elektronik ke WMF"
          link: "/signature/java/add/wmf/"
          description: "Metafile Windows"

        - name: "Tambahkan tanda tangan elektronik ke EMF"
          link: "/signature/java/add/emf/"
          description: "Format Metafile yang Ditingkatkan"

        - name: "Tambahkan tanda tangan elektronik ke CMX"
          link: "/signature/java/add/cmx/"
          description: "Corel Metafile eXchange Gambar"

        - name: "Tambahkan tanda tangan elektronik ke DJVU"
          link: "/signature/java/add/djvu/"
          description: "Deja Vu"

        - name: "Tambahkan tanda tangan elektronik ke PPSM"
          link: "/signature/java/add/ppsm/"
          description: "Peragaan Slide Berkemampuan Makro Microsoft PowerPoint"

        - name: "Tambahkan tanda tangan elektronik ke DCM"
          link: "/signature/java/add/dcm/"
          description: "Pencitraan Digital dan Komunikasi dalam Kedokteran"


back_to_top:
    enable: true
---
