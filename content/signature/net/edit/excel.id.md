---
layout: "auto-gen"
date: 2022-07-07T12:44:18+03:00
draft: false

head_title: "Sunting &amp; Perbarui file EXCEL yang Ditandatangani Secara Digital di .NET | Menandatangani Dokumen"
head_description: "Edit file EXCEL dengan tanda tangan digital di .NET - perbarui tanda tangan elektronik dalam dokumen bisnis populer dan format file gambar."

title: "Edit Tanda Tangan Digital dalam File EXCEL"
description: "C# .NET API untuk mengedit tanda tangan elektronik secara instan dalam file EXCEL menggunakan jenis tanda tangan digital populer. Kelola properti tanda tangan dan sesuaikan opsi penandatanganan dalam dokumen dan gambar."
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
        [GroupDocs.Signature for .NET](/id/signature/net/) adalah .NET API asli untuk menandatangani dokumen secara digital menggunakan berbagai jenis tanda tangan seperti teks, gambar, kode batang, stempel, bidang formulir, kode QR, dan metadata. Pengguna dapat dengan mudah menambahkan, mengedit, memverifikasi, menghapus, dan menemukan tanda tangan digital dalam PDF, Microsoft Word, lembar kerja EXCEL, presentasi PowerPoint, Adobe Photoshop, metafile, dan format file gambar dengan dukungan tambahan untuk menyesuaikan properti tanda tangan sesuai kebutuhan.

steps:
    enable: true
    title_left: "Cara Mengedit Tanda Tangan Digital di EXCEL"
    content_left: |
        [GroupDocs.Signature](/id/signature/net/) memudahkan pengembang .NET untuk mengedit tanda tangan digital dari file EXCEL dalam aplikasi mereka dengan menerapkan beberapa langkah mudah.

        * Buat instance baru kelas Signature dan berikan jalur dokumen sumber sebagai parameter konstruktor.
        * Buat instance objek TextSearchOptions dengan properti yang diinginkan.
        * Panggil metode Pencarian untuk mendapatkan daftar TextSignatures.
        * Pilih dari daftar objek TextSignature yang harus diperbarui.
        * Panggil metode Perbarui objek Signature & berikan satu / beberapa tanda tangan ke sana.
        
    title_right: "Persyaratan sistem"
    content_right: |
        GroupDocs.Signature untuk .NET API didukung di semua platform dan sistem operasi utama. Sebelum menjalankan kode di bawah ini, pastikan Anda telah menginstal prasyarat berikut di sistem Anda.

        * Sistem Operasi: Microsoft Windows, Linux, MacOS
        * Lingkungan Pengembangan: Visual Studio, Xamarin, MonoDevelop
        * Kerangka: .NET Framework, .NET Standard, .NET Core, Mono
        * Unduh versi terbaru GroupDocs.Signature untuk .NET dari [NuGet](https://www.nuget.org/packages/groupdocs.signature)
        
    code: |
        ```cs
        using (Signature signature = new Signature("sampleSigned.pdf"))
        {
            TextSearchOptions options = new TextSearchOptions();
            // mencari tanda tangan teks dalam dokumen
            List signatures = signature.Search(options);
            if(signatures.Count > 0)
            {
                TextSignature textSignature = signatures[0];
                // ubah properti Teks
                textSignature.Text = "John Walkman";
                // ubah posisi
                textSignature.Left = textSignature.Left + 10;
                textSignature.Top = textSignature.Top + 10;
                // mengubah ukuran. Harap dicatat tidak semua dokumen mendukung perubahan ukuran tanda tangan
                textSignature.Width = 200;
                textSignature.Height = 100;
                bool result = signature.Update(textSignature);
                if(result)
                {
                    Console.WriteLine($"Signature with Text '{textSignature.Text}' was updated in the document ['{fileName}'].");
                }
                else
                {
                    Console.WriteLine($"Signature was not updated in  the document! Signature with Text '{textSignature.Text}' was not found!");
                }
            }
        }
        ```
        
demos:
    enable: true
    title: "Demo Langsung - Aplikasi Online untuk Memperbarui Tanda Tangan Digital"
    content: |
        Edit tanda tangan dalam file EXCEL sekarang juga dengan mengunjungi situs web [GroupDocs.Signature](https://products.groupdocs.app/signature/family). Demo langsung memiliki manfaat sebagai berikut.
        
about_formats:
    enable: true
    format:
        - icon: "far fa-file-excel"
          title: "Tentang Format Berkas EXCEL"
          content: |
            File spreadsheet berisi data dalam bentuk baris dan kolom. Anda dapat membuka, melihat, dan mengedit file tersebut menggunakan aplikasi perangkat lunak spreadsheet seperti Microsoft EXCEL yang sekarang tersedia untuk sistem operasi Windows dan MacOS. Demikian pula, Google sheets adalah alat pembuat dan pengeditan spreadsheet online gratis yang berfungsi dari browser web apa pun. File spreadsheet dapat disimpan dalam beberapa format file yang berbeda, masing-masing memiliki ekstensi file yang berbeda untuk representasi yang unik. Data disimpan dalam sel baik dalam bentuk biasa seperti string teks, angka, tanggal, mata uang, dll. Atau sebagai rumus yang mengubah nilai sel saat nilai sel yang direferensikan berubah. Ekstensi file spreadsheet umum dan format filenya termasuk XLSX (Microsoft EXCEL Open XML Spreadsheet), ODS (OpenDocument Spreadsheet) dan XLS (Microsoft EXCEL Binary File Format).

          link: "https://docs.fileformat.com/spreadsheet/"

more_formats:
    enable: true
    title: "Mengedit Tanda Tangan Dari Format Dokumen Digital Lainnya"
    content: |
        Dokumen multi format dan API pengeditan tanda tangan gambar untuk .NET. Perbarui tanda tangan dari beberapa format file populer seperti yang dinyatakan di bawah ini.
    format: 
        - name: "Edit tanda tangan elektronik dari PDF"
          link: "/signature/net/edit/pdf/"
          description: "Format Dokumen Portabel Adobe"

        - name: "Edit tanda tangan elektronik dari DOC"
          link: "/signature/net/edit/doc/"
          description: "Dokumen Microsoft Word"

        - name: "Edit tanda tangan elektronik dari DOCM"
          link: "/signature/net/edit/docm/"
          description: "Dokumen Berkemampuan Makro Microsoft Word"

        - name: "Edit tanda tangan elektronik dari DOCX"
          link: "/signature/net/edit/docx/"
          description: "Microsoft Word Buka Dokumen XML"

        - name: "Edit tanda tangan elektronik dari DOT"
          link: "/signature/net/edit/dot/"
          description: "Templat Dokumen Microsoft Word"

        - name: "Edit tanda tangan elektronik dari DOTX"
          link: "/signature/net/edit/dotx/"
          description: "Templat Dokumen XML Word Terbuka"

        - name: "Edit tanda tangan elektronik dari DOTM"
          link: "/signature/net/edit/dotm/"
          description: "Templat Microsoft Word Macro-Enabled"

        - name: "Edit tanda tangan elektronik dari RTF"
          link: "/signature/net/edit/rtf/"
          description: "Dokumen Teks Kaya"

        - name: "Edit tanda tangan elektronik dari ODT"
          link: "/signature/net/edit/odt/"
          description: "Buka Teks Dokumen"

        - name: "Edit tanda tangan elektronik dari OTT"
          link: "/signature/net/edit/ott/"
          description: "Templat Teks OpenDocument"

        - name: "Edit tanda tangan elektronik dari XLS"
          link: "/signature/net/edit/xls/"
          description: "Format File Biner Microsoft EXCEL"

        - name: "Edit tanda tangan elektronik dari XLSX"
          link: "/signature/net/edit/xlsx/"
          description: "Microsoft EXCEL Buka XML Spreadsheet"

        - name: "Edit tanda tangan elektronik dari XLSM"
          link: "/signature/net/edit/xlsm/"
          description: "Spreadsheet Berkemampuan Makro Microsoft EXCEL"

        - name: "Edit tanda tangan elektronik dari XLSM"
          link: "/signature/net/edit/xlsm/"
          description: "Spreadsheet Berkemampuan Makro Microsoft EXCEL"

        - name: "Edit tanda tangan elektronik dari XLSB"
          link: "/signature/net/edit/xlsb/"
          description: "Lembar Kerja Biner Microsoft EXCEL"

        - name: "Edit tanda tangan elektronik dari XLTX"
          link: "/signature/net/edit/xltx/"
          description: "Templat Microsoft EXCEL"

        - name: "Edit tanda tangan elektronik dari XLTM"
          link: "/signature/net/edit/xltm/"
          description: "Templat berkemampuan makro Microsoft EXCEL"

        - name: "Edit tanda tangan elektronik dari ODS"
          link: "/signature/net/edit/ods/"
          description: "Buka Spreadsheet Dokumen"

        - name: "Edit tanda tangan elektronik dari OTS"
          link: "/signature/net/edit/ots/"
          description: "Templat Spreadsheet OpenDocument"

        - name: "Edit tanda tangan elektronik dari PPT"
          link: "/signature/net/edit/ppt/"
          description: "Presentasi powerpoint"

        - name: "Edit tanda tangan elektronik dari PPTX"
          link: "/signature/net/edit/pptx/"
          description: "Presentasi PowerPoint Terbuka XML"

        - name: "Edit tanda tangan elektronik dari PPS"
          link: "/signature/net/edit/pps/"
          description: "Peragaan Slide Microsoft PowerPoint 97-2003"

        - name: "Edit tanda tangan elektronik dari PPSX"
          link: "/signature/net/edit/ppsx/"
          description: "PowerPoint Terbuka XML Slide Show"

        - name: "Edit tanda tangan elektronik dari POTM"
          link: "/signature/net/edit/potm/"
          description: "Templat Microsoft PowerPoint Macro-Enabled"

        - name: "Edit tanda tangan elektronik dari POTX"
          link: "/signature/net/edit/potx/"
          description: "Templat Microsoft PowerPoint"

        - name: "Edit tanda tangan elektronik dari PPTM"
          link: "/signature/net/edit/pptm/"
          description: "Presentasi Microsoft PowerPoint"

        - name: "Edit tanda tangan elektronik dari ODP"
          link: "/signature/net/edit/odp/"
          description: "Presentasi OpenDocument"

        - name: "Edit tanda tangan elektronik dari OTP"
          link: "/signature/net/edit/otp/"
          description: "Template Presentasi OpenDocument"

        - name: "Edit tanda tangan elektronik dari WEBP"
          link: "/signature/net/edit/webp/"
          description: "Gambar WebP"

        - name: "Edit tanda tangan elektronik dari TIFF"
          link: "/signature/net/edit/tiff/"
          description: "Format File Gambar yang Ditandai"

        - name: "Edit tanda tangan elektronik dari JPEG"
          link: "/signature/net/edit/jpeg/"
          description: "Gambar JPEG"

        - name: "Edit tanda tangan elektronik dari GIF"
          link: "/signature/net/edit/gif/"
          description: "Format Pertukaran Grafik"

        - name: "Edit tanda tangan elektronik dari PNG"
          link: "/signature/net/edit/png/"
          description: "Grafik Jaringan Portabel"

        - name: "Edit tanda tangan elektronik dari BMP"
          link: "/signature/net/edit/bmp/"
          description: "Format File Bitmap"

        - name: "Edit tanda tangan elektronik dari CDR"
          link: "/signature/net/edit/cdr/"
          description: "Gambar Grafis Vektor CorelDraw"

        - name: "Edit tanda tangan elektronik dari SVG"
          link: "/signature/net/edit/svg/"
          description: "Grafik Vektor Skalabel"

        - name: "Edit tanda tangan elektronik dari PSD"
          link: "/signature/net/edit/psd/"
          description: "Dokumen Adobe Photoshop"

        - name: "Edit tanda tangan elektronik dari WMF"
          link: "/signature/net/edit/wmf/"
          description: "Metafile Windows"

        - name: "Edit tanda tangan elektronik dari EMF"
          link: "/signature/net/edit/emf/"
          description: "Format Metafile yang Ditingkatkan"

        - name: "Edit tanda tangan elektronik dari CMX"
          link: "/signature/net/edit/cmx/"
          description: "Corel Metafile eXchange Gambar"

        - name: "Edit tanda tangan elektronik dari DJVU"
          link: "/signature/net/edit/djvu/"
          description: "Deja Vu"

        - name: "Edit tanda tangan elektronik dari PPSM"
          link: "/signature/net/edit/ppsm/"
          description: "Peragaan Slide Berkemampuan Makro Microsoft PowerPoint"

        - name: "Edit tanda tangan elektronik dari DCM"
          link: "/signature/net/edit/dcm/"
          description: "Pencitraan Digital dan Komunikasi dalam Kedokteran"


back_to_top:
    enable: true
---
