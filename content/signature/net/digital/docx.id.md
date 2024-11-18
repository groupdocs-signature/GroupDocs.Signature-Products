



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:59
draft: false
lang: id
format: Docx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Menambahkan tanda tangan elektronik digital ke file DOCX dengan C#"
head_description: "Pasang tanda tangan digital pada file DOCX menggunakan C# dengan hanya beberapa baris kode. Gunakan GroupDocs.Signature for .NET untuk menandatangani berbagai format file."

############################# Header ############################
title: "eSign DOCX dengan tanda tangan digital" 
description: "Lindungi integritas dokumen bisnis Anda dengan menyegelnya menggunakan sertifikat digital melalui fitur kuat dari GroupDocs.Signature for .NET. Kami menawarkan solusi serbaguna untuk menandai dan mengamankan dokumen Anda."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Unduh gratis"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "Tentang GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) adalah solusi tanda tangan canggih yang memfasilitasi berbagai tugas pemrosesan dokumen. Solusi ini memungkinkan Anda menyematkan teks, gambar, sertifikat digital, dan cap ke dalam file di lebih dari 60 format, termasuk PDF, MS Office, gambar, file ZIP, dan format bisnis penting lainnya. Selain itu, dokumen yang ditandatangani dapat dengan mudah dicari, diverifikasi, dimodifikasi, atau dihapus sesuai kebutuhan.

############################# Steps ############################
steps:
    enable: true
    title: "Cara mengamankan DOCX dengan sertifikat digital di C#"
    content: |
      [GroupDocs.Signature](/signature/net/) memberdayakan pengembang .NET untuk melindungi dokumen DOCX dari perubahan menggunakan tanda tangan digital. Tingkatkan aplikasi bisnis Anda dengan kemampuan perlindungan data yang kuat.
      
      1. Serahkan dokumen DOCX ke konstruktor kelas Signature.
      2. Gunakan sertifikat digital dan kata sandinya untuk mengamankan dokumen.
      3. Jika perlu, tambahkan representasi visual dari tanda tangan digital pada halaman dokumen.
      4. Tandatangani dokumen untuk memastikan bahwa itu tetap tidak berubah.
   
    code:
      platform: "net"
      copy_title: "Salin"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Contoh tanda tangan"
      install:
        command: "dotnet add package GroupDocs.Signature"
        copy_tip: "klik untuk menyalin"
        copy_done: "disalin"
      links:
        #  loop
        - title: "Lebih banyak contoh"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET/"
        #  loop
        - title: "Dokumentasi"
          link: "https://docs.groupdocs.com/signature/net/"
          
      content: |
        ```csharp {style=abap}
        // Manfaatkan Signature untuk menandatangani dokumen secara digital
        using (Signature signature = new Signature("input.docx"))
        {
            // Sediakan sertifikat digital dan kata sandi terkait
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                Password = "1234567890",

                // Konfigurasikan representasi visual jika diperlukan
                PageNumber = 1,
                Left = 50,
                Top = 50
            };

            // Amankan dokumen dengan sertifikat digital
            SignResult result = signature.Sign("output.docx", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Tingkatkan atau lindungi konten dokumen dengan tanda tangan"
  description: "Koleksi GroupDocs.Signature for .NET dirancang untuk menandatangani semua format file yang umum. Sederhanakan proses bisnis Anda dengan menambahkan, memodifikasi, memverifikasi, atau menghapus berbagai tanda tangan."
  image: "/img/signature/features_digital.webp" # 500x500 px
  image_description: "Fitur Utama dari GroupDocs.Signature"
  features:
    # feature loop
    - title: "Sisipkan tanda tangan ke dalam dokumen"
      content: "Sisipkan Teks, Gambar, Kode Barkode, Kode QR, atau Tanda tangan cap dengan presisi di setiap halaman dokumen yang didukung. Anda juga dapat menambah atau mengedit metadata tersembunyi, seperti EXIF, pada gambar dan sebagian besar jenis file. Pastikan integritas konten dokumen Anda dengan tanda tangan digital."

    # feature loop
    - title: "Cari dan verifikasi tanda tangan"
      content: "Pemrosesan pasca-tanda tangan menawarkan banyak kemungkinan. Verifikasi bahwa dokumen yang telah Anda tandatangani telah diproses dengan benar. Untuk kontrol yang lebih besar, ambil daftar lengkap semua tanda tangan melalui fungsi pencarian."

    # feature loop
    - title: "Modifikasi tanda tangan"
      content: "Sebagian besar jenis tanda tangan sepenuhnya dapat diedit. Anda memiliki fleksibilitas untuk menyesuaikan teks, memindahkan elemen, mengubah warna, mengubah ukuran, dan lainnya."

    # feature loop
    - title: "Hapus tanda tangan yang tidak diperlukan"
      content: "Solusi kami menyediakan operasi CRUD lengkap untuk tanda tangan. Jika diperlukan, Anda dapat menghapus berbagai jenis tanda tangan, termasuk sertifikat digital, dari dokumen Anda."
      
  code_samples:
    # code sample loop
    - title: "Amankan dokumen dengan tanda tangan digital"
      content: |
        Pelajari cara mencegah perubahan dokumen menggunakan tanda tangan digital.
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        // Sediakan dokumen untuk ditandatangani
        using (Signature signature = new Signature("input.docx"))
        {
            // Gunakan sertifikat digital yang valid dengan kata sandi terkait
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                Password = "1234567890",

                // Tentukan informasi teks tambahan jika ada
                Reason = "Security issue",
                Contact = "John Smith",
                Location = "Office D.W.",

                // Sisipkan gambar dan opsi lainnya untuk representasi visual
                ImageFilePath = "image.png",
                AllPages = true,
                VerticalAlignment = VerticalAlignment.Center,
                HorizontalAlignment = HorizontalAlignment.Left,
                Width = 60,
                Height = 80,

                Margin = new Padding() {  Bottom = 10, Right = 10 }
            };

            // Simpan dokumen yang diamankan ke lokasi yang ditentukan
            SignResult result = signature.Sign("output.docx", options);
        }
        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "Siap untuk memulai?"
  description: "Coba fitur GroupDocs.Signature secara gratis atau minta lisensi"
  items:
    #  loop
    - title: "Unduhan Nuget"
      link: "https://releases.groupdocs.com/signature/net/"
      color: "red"
        #  loop
    - title: "Lisensi"
      link: "https://purchase.groupdocs.com/pricing/signature/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Lihat fitur unggulan kami"
    exclude: "digital"
    description: "Kami menyediakan berbagai format tanda tangan dan operasi yang kuat"
    items: 
          
        # operation loop 1
        - name: "Tanda Tangan Elektronik"
          operation: "esign"
          link: "/signature/net/esign/docx/"
          description: "Tambahkan berbagai jenis tanda tangan ke format file yang didukung"

        # operation loop 2
        - name: "Tambahkan teks ke dokumen"
          operation: "text"
          link: "/signature/net/text/docx/"
          description: "Tingkatkan konten dokumen dengan tanda tangan teks yang dapat disesuaikan"

        # operation loop 3
        - name: "Tanda Tangan Gambar"
          operation: "image"
          link: "/signature/net/image/docx/"
          description: "Tempatkan gambar di posisi mana pun dalam dokumen"

        # operation loop 4
        - name: "Hasilkan barcode"
          operation: "barcode"
          link: "/signature/net/barcode/docx/"
          description: "Buat dan sisipkan berbagai barcode ke dalam dokumen yang didukung"

        # operation loop 5
        - name: "Hasilkan QR code"
          operation: "qrcode"
          link: "/signature/net/qrcode/docx/"
          description: "Buat dan QR Code, termasuk QR code, untuk penandatanganan dokumen"
          
        # operation loop 6
        - name: "Sertifikat Digital"
          operation: "digital"
          link: "/signature/net/digital/docx/"
          description: "Amankan bisnis dan tanda tangani dokumen dengan sertifikat digital"

        # operation loop 7
        - name: "Tanda Tangan Stempel"
          operation: "stamp"
          link: "/signature/net/stamp/docx/"
          description: "Gunakan Konstruksi Stempel untuk membuat stempel bulat atau persegi yang kustom"
          
        # operation loop 8
        - name: "Cari tanda tangan"
          operation: "search"
          link: "/signature/net/search/docx/"
          description: "Temukan tanda tangan yang ditambahkan sebelumnya dalam dokumen"
          
        # operation loop 9
        - name: "Verifikasi tanda tangan"
          operation: "verify"
          link: "/signature/net/verify/docx/"
          description: "Verifikasi keaslian tanda tangan setelah diterapkan"
          
        # operation loop 10
        - name: "Modifikasi tanda tangan"
          operation: "modify"
          link: "/signature/net/modify/docx/"
          description: "Edit berbagai tanda tangan dalam dokumen"
          
        # operation loop 11
        - name: "Hapus tanda tangan"
          operation: "delete"
          link: "/signature/net/delete/docx/"
          description: "Hapus berbagai tanda tangan yang diterapkan sebelumnya"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Tandatangani dokumen dalam berbagai format"
    exclude: "DOCX"
    description: "API .NET memberi Anda kemampuan untuk memproses lebih dari 60 format yang berbeda. Anda dapat dengan mudah membuat dan menyisipkan berbagai tanda tangan di seluruh halaman, menerapkan sertifikat digital untuk keamanan konten, dan mengelola tanda tangan yang ada dalam dokumen secara efisien."
    items: 
          
        # format loop 1
        - name: "Lindungi PDF"
          format: "PDF"
          link: "/signature/net/digital/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Lindungi DOCX"
          format: "DOCX"
          link: "/signature/net/digital/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Lindungi PPTX"
          format: "PPTX"
          link: "/signature/net/digital/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 4
        - name: "Lindungi XLSX"
          format: "XLSX"
          link: "/signature/net/digital/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---