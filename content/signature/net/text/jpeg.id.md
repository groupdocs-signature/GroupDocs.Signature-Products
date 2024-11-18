



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:55
draft: false
lang: id
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Buat tanda tangan teks untuk JPEG menggunakan aplikasi C#"
head_description: "Manfaatkan kekuatan API C# untuk menggabungkan tanda tangan berbasis teks ke dalam file JPEG, mendukung berbagai format termasuk PDF, Word, Excel, Presentasi, Gambar, dan ZIP."

############################# Header ############################
title: "Sisipkan tanda tangan teks dalam JPEG dengan lancar" 
description: "Integrasikan tanda tangan teks kustom ke dalam dokumen bisnis Anda menggunakan GroupDocs.Signature for .NET. Optimalkan proses organisasi dengan kemampuan kustomisasi tanda tangan yang serbaguna."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Coba gratis hari ini"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "Temukan solusi GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) menyediakan platform canggih untuk menyisipkan tanda tangan teks yang sangat dapat disesuaikan, menyederhanakan alur kerja dokumen Anda. Sesuaikan konten dan atribut visual tanda tangan teks, menerapkannya secara mulus di seluruh halaman untuk meningkatkan manajemen dokumen dan efisiensi operasional.

############################# Steps ############################
steps:
    enable: true
    title: "Cara membuat dan menambahkan tanda tangan teks ke JPEG menggunakan C#"
    content: |
      [GroupDocs.Signature](/signature/net/) memfasilitasi penggabungan tanda tangan teks ke dalam file JPEG dalam aplikasi .NET. Tingkatkan kemampuan produk Anda dengan cepat menggunakan solusi kami yang komprehensif.
      
      1. Sampaikan dokumen JPEG sebagai parameter ke konstruktor kelas Signature.
      2. Buat TextSignOptions dengan teks tanda tangan yang diperlukan.
      3. Tentukan atribut visual untuk tanda tangan.
      4. Sisipkan tanda tangan teks ke halaman yang ditentukan dalam dokumen.
   
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
        // Inisialisasi Signature dengan jalur dokumen
        using (Signature signature = new Signature("input.jpeg"))
        {
            // Buat instance dari TextSignOptions dengan teks tanda tangan yang diinginkan
            TextSignOptions options = new TextSignOptions("Approved")
            {
                // Konfigurasi warna teks dan atribut font
                ForeColor = Color.Red,
                Font = new SignatureFont { Size = 12, FamilyName = "Comic Sans MS" }
            };

            // Integrasikan tanda tangan teks ke dalam dokumen
            SignResult result = signature.Sign("output.jpeg", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Manajemen tanda tangan teks yang komprehensif"
  description: "GroupDocs.Signature for .NET memberdayakan organisasi Anda dengan meningkatkan alur kerja dokumen melalui penambahan tanda tangan teks yang dapat disesuaikan di berbagai format file populer. Kelola penampilan, penempatan, dan konten tanda tangan ini untuk memenuhi kebutuhan spesifik Anda."
  image: "/img/signature/features_text.webp" # 500x500 px
  image_description: "Jelajahi Fitur GroupDocs.Signature"
  features:
    # feature loop
    - title: "Tanda tangan dokumen yang serbaguna"
      content: "Terapkan berbagai tanda tangan—termasuk teks, gambar, kode batang, kode QR, dan cap—ke setiap halaman dokumen yang didukung. Manfaatkan metadata untuk memasukkan konten tersembunyi, sambil melindungi informasi sensitif melalui penggunaan sertifikat digital."

    # feature loop
    - title: "Pencarian dan otentikasi tanda tangan"
      content: "Pastikan validitas dan integritas dokumen yang ditandatangani dengan memanfaatkan alat verifikasi tanda tangan yang kuat. Lakukan pencarian untuk mendapatkan daftar komprehensif semua tanda tangan dalam dokumen untuk analisis lebih lanjut."

    # feature loop
    - title: "Perbarui atau hapus tanda tangan"
      content: "Modifikasi konten, properti visual, atau penempatan tanda tangan yang telah disisipkan sebelumnya dengan mudah. Jika perlu, hapus tanda tangan yang tidak diinginkan untuk menjaga konten dokumen yang akurat dan relevan."

    # feature loop
    - title: "Tanda tangan teks yang khusus"
      content: "Terapkan tanda tangan teks yang spesifik untuk dokumen, seperti watermark untuk dokumen Word atau stiker untuk PDF, untuk memberikan lapisan kustomisasi dan kontrol tambahan."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Sisipkan tanda tangan teks dalam dokumen"
      content: |
        Temukan cara untuk menggabungkan tanda tangan teks ke dalam dokumen bisnis untuk menyederhanakan proses.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Pilih dokumen yang akan ditandatangani
          using (Signature signature = new Signature("input.jpeg"))
          {
              // Buat opsi teks dengan konten yang ditentukan
              TextSignOptions options = new TextSignOptions("Rescheduled to 03/04/2025")
              {
                    // Tentukan dimensi dan posisi tanda tangan di halaman
                    Left = 100,
                    Top = 180,
                    Width = 230,
                    Height = 30,

                    // Terapkan padding dari tepi halaman untuk tanda tangan
                    Margin = new Padding() { Top = 20, Right = 20 },

                    // Sesuaikan warna teks dan gaya font
                    ForeColor = Color.OrangeRed,
                    Font = new SignatureFont { Size = 12, FamilyName = "Comic Sans MS" },

                    // Gabungkan border di sekitar tanda tangan teks
                    Border = new Border()
                    {
                        Color = Color.OrangeRed,
                        DashStyle = DashStyle.Dash,
                        Transparency = 0.5,
                        Visible = true,
                        Weight = 2
                    },

                    // Terapkan kustomisasi latar belakang jika perlu
                    Background = new Background()
                    {
                        Color = Color.LightYellow,
                        Transparency = 0.8
                    },

                    // Opsi simpan teks sebagai gambar untuk memastikan kompatibilitas
                    SignatureImplementation = TextSignatureImplementation.Image
              };

              // Simpan dokumen dengan tanda tangan teks yang terintegrasi
              SignResult result = signature.Sign("output.jpeg", options);
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
            link: "/examples/signature/formats/signature_text.jpeg"
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
    title: "Fitur lanjutan dan opsi tanda tangan"
    exclude: "text"
    description: "API kami mendukung manajemen siklus hidup penuh dari tujuh jenis tanda tangan, menawarkan kemampuan CRUD yang komprehensif untuk mengelola, memverifikasi, dan menyesuaikan tanda tangan Anda."
    items: 
          
        # operation loop 1
        - name: "Tanda Tangan Elektronik"
          operation: "esign"
          link: "/signature/net/esign/jpeg/"
          description: "Tambahkan berbagai jenis tanda tangan ke format file yang didukung"

        # operation loop 2
        - name: "Tambahkan teks ke dokumen"
          operation: "text"
          link: "/signature/net/text/jpeg/"
          description: "Tingkatkan konten dokumen dengan tanda tangan teks yang dapat disesuaikan"

        # operation loop 3
        - name: "Tanda Tangan Gambar"
          operation: "image"
          link: "/signature/net/image/jpeg/"
          description: "Tempatkan gambar di posisi mana pun dalam dokumen"

        # operation loop 4
        - name: "Hasilkan barcode"
          operation: "barcode"
          link: "/signature/net/barcode/jpeg/"
          description: "Buat dan sisipkan berbagai barcode ke dalam dokumen yang didukung"

        # operation loop 5
        - name: "Hasilkan QR code"
          operation: "qrcode"
          link: "/signature/net/qrcode/jpeg/"
          description: "Buat dan QR Code, termasuk QR code, untuk penandatanganan dokumen"
          
        # operation loop 6
        - name: "Sertifikat Digital"
          operation: "digital"
          link: "/signature/net/digital/pdf/"
          description: "Amankan bisnis dan tanda tangani dokumen dengan sertifikat digital"

        # operation loop 7
        - name: "Tanda Tangan Stempel"
          operation: "stamp"
          link: "/signature/net/stamp/jpeg/"
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
    title: "Sisipkan tanda tangan teks di berbagai format file"
    exclude: "JPEG"
    description: "Dengan API .NET kami, Anda dapat menyisipkan tanda tangan teks ke dalam berbagai dokumen Office. Ambil kontrol penuh atas siklus hidup dokumen Anda dengan menambahkan tanda tangan teks yang meningkatkan fungsionalitas dan keamanan."
    items: 
          
        # format loop 1
        - name: "Tanda Tangan Teks PDF"
          format: "PDF"
          link: "/signature/net/text/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Tanda Tangan Teks DOCX"
          format: "DOCX"
          link: "/signature/net/text/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Tanda Tangan Teks JPEG"
          format: "JPEG"
          link: "/signature/net/text/jpeg/"
          description: "Gambar JPEG"
          
        # format loop 4
        - name: "Tanda Tangan Teks PPTX"
          format: "PPTX"
          link: "/signature/net/text/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 5
        - name: "Tanda Tangan Teks XLSX"
          format: "XLSX"
          link: "/signature/net/text/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---