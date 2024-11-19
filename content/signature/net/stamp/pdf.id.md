



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:05
draft: false
lang: id
format: Pdf
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Stempel bulat dan persegi PDF melalui C#"
head_description: "Gunakan GroupDocs.Signature for .NET untuk menghasilkan dan menyisipkan stempel yang dipersonalisasi ke dokumen PDF."

############################# Header ############################
title: "Hasilkan stempel untuk file PDF" 
description: "Integrasikan stempel yang dirancang khusus ke dalam setiap bagian dokumen Anda menggunakan GroupDocs.Signature for .NET, menawarkan fleksibilitas luas untuk penempatan dan konfigurasi stempel sesuai kebutuhan bisnis Anda."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Dapatkan unduhan gratis Anda"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "Gambaran umum GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) adalah alat serbaguna yang memungkinkan penyisipan berbagai tipe tanda tangan ke dalam dokumen, termasuk stempel yang dapat disesuaikan. Mendukung lebih dari 60 format file, mulai dari PDF dan dokumen Word hingga gambar dan file ZIP, Anda dapat memperkaya dokumen dengan teks, gambar, kode batang, metadata, sertifikat digital, dan stempel. Selain itu, Anda memiliki kontrol penuh untuk mencari, memvalidasi, memodifikasi, atau menghapus tanda tangan yang diterapkan pada file Anda.

############################# Steps ############################
steps:
    enable: true
    title: "Cara menyisipkan stempel ke dalam PDF menggunakan C#"
    content: |
      [GroupDocs.Signature](/signature/net/) menawarkan fitur pembuatan stempel yang kuat, ideal untuk meningkatkan aplikasi .NET. Manfaatkan alat ini untuk merancang dan menerapkan stempel yang sangat disesuaikan pada halaman dokumen Anda.
      
      1. Berikan dokumen PDF yang akan distempel.
      2. Gunakan StampSignOptions untuk dengan teliti mengonfigurasi semua parameter yang diperlukan.
      3. Tambahkan beberapa baris stempel sesuai kebutuhan Anda.
      4. Terapkan stempel yang telah dikonfigurasi dan simpan dokumen yang telah dimodifikasi.
   
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
        // Integrasikan jalur dokumen dengan instansi Signature
        using (Signature signature = new Signature("input.pdf"))
        {
            // Inisialisasi StampSignOptions dengan konten tanda tangan yang diperlukan
            StampSignOptions options = new StampSignOptions();
            options.Height = 180;
            options.Width = 180;

            // Incorporate satu atau beberapa baris stempel
            options.OuterLines.Add(
                new StampLine()
                {
                    Text = "* The Best Company *",
                    TextRepeatType = StampTextRepeatType.FullTextRepeat,
                    Font = new SignatureFont() { Size = 12, FamilyName = "Arial" },
                    Height = 22,
                    TextBottomIntent = 6,
                    TextColor = Color.WhiteSmoke,
                    BackgroundColor = Color.DarkSlateBlue
                }
            );

            // Simpan dokumen dengan stempel yang diterapkan
            SignResult result = signature.Sign("output.pdf", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Manfaatkan tanda tangan untuk mengamankan dan meningkatkan integritas dokumen"
  description: "Dengan pustaka GroupDocs.Signature for .NET, Anda dapat mengintegrasikan fungsionalitas tanda tangan ke dalam dokumen Anda. Sekaligus menambah, memodifikasi, memverifikasi, atau menghapus stempel khusus dan jenis tanda tangan lainnya, menawarkan fleksibilitas dan presisi untuk manajemen dokumen yang aman."
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "Tanda Tangan Stempel Didukung oleh GroupDocs.Signature"
  features:
    # feature loop
    - title: "Tanda tangan dokumen menyeluruh"
      content: "Perkaya dokumen Anda dengan menempatkan tanda tangan, termasuk teks, gambar, kode batang, kode QR, dan stempel, di posisi atau halaman mana pun dalam file. Selain itu, kelola metadata yang disematkan dan terapkan sertifikat digital untuk melindungi dari perubahan tanpa izin."

    # feature loop
    - title: "Pencarian dan validasi tanda tangan yang efisien"
      content: "Setelah menandatangani, verifikasi keaslian dan integritas tanda tangan dokumen. Gunakan fungsionalitas pencarian lanjutan untuk mengambil dan mengelola semua data tanda tangan yang disematkan dalam dokumen."

    # feature loop
    - title: "Modifikasi dan sesuaikan tanda tangan"
      content: "Sesuaikan tanda tangan yang telah dimasukkan sebelumnya dengan mudah. Apakah Anda perlu mengubah konten, posisi, ukuran, atau warna, solusi kami menawarkan fleksibilitas penuh untuk modifikasi tanda tangan."

    # feature loop
    - title: "Mudah menghapus tanda tangan"
      content: "Ketika tanda tangan perlu dihapus, GroupDocs.Signature for .NET menyediakan seperangkat alat lengkap untuk menghapus semua jenis tanda tangan, termasuk stempel, sertifikat digital, dan lainnya, memastikan dokumen Anda tetap mutakhir dan sesuai."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Terapkan stempel kustom di dokumen"
      content: |
        Temukan cara untuk merancang dan mengintegrasikan stempel kustom yang memuat detail teks penting ke dalam dokumen Anda.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Sediakan dokumen yang akan distempel
          using (Signature signature = new Signature("input.pdf"))
          {
              // Inisialisasi opsi stempel dengan konfigurasi yang diinginkan
              StampSignOptions options = new StampSignOptions()
              {
                    // Tentukan dimensi dan posisi stempel di halaman
                    Height = 200,
                    Width = 200,
                    VerticalAlignment = VerticalAlignment.Bottom,
                    HorizontalAlignment = HorizontalAlignment.Right,
                    AllPages = true
              };

              // Incorporate garis lingkar luar dengan teks
              options.OuterLines.Add(
                    new StampLine()
                    {
                        Text = "* The best  choice *",
                        TextRepeatType = StampTextRepeatType.FullTextRepeat,
                        Font = new SignatureFont() { Size = 12, FamilyName = "Arial" },
                        Height = 22,
                        TextBottomIntent = 6,
                        TextColor = Color.WhiteSmoke,
                        BackgroundColor = Color.DarkSlateBlue
                    }
              );

              // Integrasikan garis persegi bagian dalam jika perlu
              options.InnerLines.Add(
                    new StampLine()
                    { 
                        Text = "Company #1",
                        TextColor = Color.MediumVioletRed,
                        Font = new SignatureFont() { Size = 20, Bold = true },
                        Height = 40
                    }
              );

              // Finalisasi dan simpan dokumen yang telah distempel
              SignResult result = signature.Sign("output.pdf", options);
          }
          ```
        platform: "net"
        copy_title: "Salin"
        install:
          command: "dotnet add package GroupDocs.Signature"
          copy_tip: "klik untuk menyalin"
          copy_done: "disalin"
        top_links:
          #  loop
          - title: "Unduh hasil"
            icon: "download"
            link: "/examples/signature/formats/signature_stamp.pdf"
        links:
          #  loop
          - title: "Lebih banyak contoh"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET/"
          #  loop
          - title: "Dokumentasi"
            link: "https://docs.groupdocs.com/signature/net/"
            

            


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
    title: "Jelajahi fungsionalitas inti"
    exclude: "stamp"
    description: "Temukan berbagai opsi untuk membuat, mengelola, dan menghapus berbagai jenis tanda tangan, memastikan kontrol komprehensif atas alur kerja dokumen Anda."
    items: 
          
        # operation loop 1
        - name: "Tanda Tangan Elektronik"
          operation: "esign"
          link: "/signature/net/esign/pdf/"
          description: "Tambahkan berbagai jenis tanda tangan ke format file yang didukung"

        # operation loop 2
        - name: "Tambahkan teks ke dokumen"
          operation: "text"
          link: "/signature/net/text/pdf/"
          description: "Tingkatkan konten dokumen dengan tanda tangan teks yang dapat disesuaikan"

        # operation loop 3
        - name: "Tanda Tangan Gambar"
          operation: "image"
          link: "/signature/net/image/pdf/"
          description: "Tempatkan gambar di posisi mana pun dalam dokumen"

        # operation loop 4
        - name: "Hasilkan barcode"
          operation: "barcode"
          link: "/signature/net/barcode/pdf/"
          description: "Buat dan sisipkan berbagai barcode ke dalam dokumen yang didukung"

        # operation loop 5
        - name: "Hasilkan QR code"
          operation: "qrcode"
          link: "/signature/net/qrcode/pdf/"
          description: "Buat dan QR Code, termasuk QR code, untuk penandatanganan dokumen"
          
        # operation loop 6
        - name: "Sertifikat Digital"
          operation: "digital"
          link: "/signature/net/digital/pdf/"
          description: "Amankan bisnis dan tanda tangani dokumen dengan sertifikat digital"

        # operation loop 7
        - name: "Tanda Tangan Stempel"
          operation: "stamp"
          link: "/signature/net/stamp/pdf/"
          description: "Gunakan Konstruksi Stempel untuk membuat stempel bulat atau persegi yang kustom"
          
        # operation loop 8
        - name: "Cari tanda tangan"
          operation: "search"
          link: "/signature/net/search/pdf/"
          description: "Temukan tanda tangan yang ditambahkan sebelumnya dalam dokumen"
          
        # operation loop 9
        - name: "Verifikasi tanda tangan"
          operation: "verify"
          link: "/signature/net/verify/pdf/"
          description: "Verifikasi keaslian tanda tangan setelah diterapkan"
          
        # operation loop 10
        - name: "Modifikasi tanda tangan"
          operation: "modify"
          link: "/signature/net/modify/pdf/"
          description: "Edit berbagai tanda tangan dalam dokumen"
          
        # operation loop 11
        - name: "Hapus tanda tangan"
          operation: "delete"
          link: "/signature/net/delete/pdf/"
          description: "Hapus berbagai tanda tangan yang diterapkan sebelumnya"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Terapkan stempel pada berbagai format dokumen"
    exclude: "PDF"
    description: "API GroupDocs.Signature memungkinkan Anda menyematkan stempel di lebih dari 60 jenis file standar industri. Terapkan stempel khusus ke lokasi mana pun dalam dokumen Anda, memungkinkan pelacakan dan personalisasi dokumen yang lebih baik."
    items: 
          
        # format loop 1
        - name: "Stempel PDF"
          format: "PDF"
          link: "/signature/net/stamp/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Stempel DOCX"
          format: "DOCX"
          link: "/signature/net/stamp/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Stempel JPEG"
          format: "JPEG"
          link: "/signature/net/stamp/jpeg/"
          description: "Gambar JPEG"
          
        # format loop 4
        - name: "Stempel PPTX"
          format: "PPTX"
          link: "/signature/net/stamp/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 5
        - name: "Stempel XLSX"
          format: "XLSX"
          link: "/signature/net/stamp/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---