



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:51
draft: false
lang: id
format: Docx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Menambahkan tanda tangan gambar ke file DOCX dengan C#"
head_description: "Sisipkan tanda tangan gambar pada file DOCX untuk .NET menggunakan beberapa baris kode. Gunakan API GroupDocs.Signature for .NET untuk menambahkan gambar."

############################# Header ############################
title: "Tambahkan tanda tangan gambar ke file DOCX" 
description: "Manfaatkan GroupDocs.Signature for .NET untuk mengintegrasikan gambar secara mulus ke dalam berbagai format dokumen kantor, termasuk PDF, Word, Excel, dan file gambar. Menggabungkan gambar tanda tangan atasan Anda dapat menciptakan kesan profesional yang mencolok, meningkatkan daya tarik visual dan keaslian dokumen Anda."
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
    title: "Temukan GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) menawarkan kemampuan komprehensif untuk menyisipkan tanda tangan gambar di lokasi mana pun di setiap halaman dalam dokumen bisnis Anda. Tingkatkan alur kerja operasional Anda dengan mengintegrasikan gambar ke dalam PDF, dokumen Word, spreadsheet Excel, presentasi PowerPoint, dan berbagai format gambar populer melalui pustaka kami yang kuat.

############################# Steps ############################
steps:
    enable: true
    title: "Cara menambahkan gambar di mana saja dalam DOCX menggunakan C#"
    content: |
      Manfaatkan [GroupDocs.Signature](/signature/net/) untuk memberdayakan aplikasi .NET dengan kemampuan untuk menyisipkan tanda tangan ke dalam halaman mana pun dokumen DOCX. Tingkatkan kemampuan produk Anda tanpa hambatan dengan mengintegrasikan solusi kami.
      
      1. Inisialisasi kelas Signature dengan dokumen DOCX.
      2. Manfaatkan ImageSignOptions untuk menentukan gambar tanda tangan.
      3. Tempatkan gambar secara tepat di lokasi halaman yang diinginkan.
      4. Simpan dokumen yang baru ditandatangani ke lokasi yang ditentukan.
   
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
        // Inisialisasi Signature dengan jalur ke dokumen
        using (Signature signature = new Signature("input.docx"))
        {
            // Konfigurasi ImageSignOptions menggunakan gambar untuk tanda tangan
            ImageSignOptions options = new ImageSignOptions("company_logo.jpg")
            {
                // Posisikan gambar di sudut kiri atas semua halaman
                AllPages = true,
                Left = 100,
                Top = 200
            };

            // Simpan dokumen yang ditandatangani
            SignResult result = signature.Sign("output.docx", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Solusi tanda tangan dokumen yang komprehensif"
  description: "Kami dengan senang hati mempersembahkan berbagai fungsionalitas tanda tangan yang didukung oleh API kami. Tambahkan, modifikasi, hapus, cari, dan verifikasi berbagai jenis tanda tangan, termasuk tanda tangan berbasis gambar, tanpa esfuerzo."
  image: "/img/signature/features_image.webp" # 500x500 px
  image_description: "Tanda Tangan Gambar"
  features:
    # feature loop
    - title: "Sisipkan gambar ke dalam dokumen kantor"
      content: "Sisipkan tanda tangan elektronik dan gambar di posisi yang ditentukan pada halaman dokumen mana pun. Tingkatkan konten dokumen Anda dengan teks, gambar, kode batang, metadata, atau sertifikat digital untuk meningkatkan fungsionalitas dan keamanan."

    # feature loop
    - title: "Pencarian dan verifikasi tanda tangan"
      content: "Kelola dokumen yang ditandatangani dengan memverifikasi keaslian dan integritas tanda tangan. Ambil daftar komprehensif semua tanda tangan dalam dokumen dan periksa atribut spesifiknya."

    # feature loop
    - title: "Modifikasi tanda tangan"
      content: "Kadang-kadang, tanda tangan dalam dokumen mungkin perlu diperbarui. Sesuaikan konten, tampilan, ukuran, atau posisi tanda tangan yang ada untuk memenuhi kebutuhan yang berkembang."

    # feature loop
    - title: "Hapus tanda tangan yang tidak diperlukan"
      content: "API kami memfasilitasi operasi CRUD penuh untuk sebagian besar tipe tanda tangan. Anda dapat dengan efisien menghapus tanda tangan dari hampir semua format dokumen yang didukung jika diperlukan."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Amankan konten dokumen dengan tanda tangan gambar"
      content: |
        Temukan cara memperkaya dokumen bisnis dengan menyisipkan gambar, memberikan informasi tambahan.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Pilih dokumen yang akan ditandatangani
          using (Signature signature = new Signature("input.docx"))
          {
              // Buat opsi gambar dengan jalur gambar yang ditentukan
              ImageSignOptions options = new ImageSignOptions("manager_signature.jpg")
              {
                    // Tentukan dimensi tanda tangan gambar
                    Width = 100,
                    Height = 100,

                    // Posisikan gambar di sudut kanan bawah
                    VerticalAlignment = VerticalAlignment.Bottom,
                    HorizontalAlignment = HorizontalAlignment.Right,

                    // Terapkan padding yang diperlukan dari tepi halaman
                    Margin = new Padding() { Bottom = 120, Right = 120 },

                    // Opsional, tambahkan border kustom ke gambar
                    Border = new Border()
                    {
                        Visible = true,
                        Color = Color.Red,
                        DashStyle = DashStyle.DashDotDot,
                        Weight = 5
                    },

                    // Putar tanda tangan untuk penyelarasan optimal
                    RotationAngle = 45
              };

              // Simpan dokumen yang diperbarui ke lokasi yang diinginkan
              SignResult result = signature.Sign("output.docx", options);
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
            link: "/examples/signature/formats/signature_image.docx"
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
    title: "Pahami penawaran fitur kami"
    exclude: "image"
    description: "Jelajahi berbagai jenis tanda tangan dan operasi kuat yang disediakan oleh platform kami"
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
    title: "Integrasikan gambar ke dalam berbagai format file"
    exclude: "DOCX"
    description: "Manfaatkan API .NET untuk melampirkan format gambar yang didukung ke berbagai dokumen. Sesuaikan ukuran, posisi, pilih halaman tertentu, dan terapkan tanda tangan berbasis gambar ke dokumen Anda."
    items: 
          
        # format loop 1
        - name: "Tanda Tangan PDF dengan Gambar"
          format: "PDF"
          link: "/signature/net/image/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Tanda Tangan DOCX dengan Gambar"
          format: "DOCX"
          link: "/signature/net/image/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Tanda Tangan JPEG dengan Gambar"
          format: "JPEG"
          link: "/signature/net/image/jpeg/"
          description: "Gambar JPEG"
          
        # format loop 4
        - name: "Tanda Tangan PPTX dengan Gambar"
          format: "PPTX"
          link: "/signature/net/image/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 5
        - name: "Tanda Tangan XLSX dengan Gambar"
          format: "XLSX"
          link: "/signature/net/image/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---