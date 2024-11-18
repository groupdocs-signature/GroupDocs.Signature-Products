



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:10
draft: false
lang: id
format: Docx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Tandai DOCX secara elektronik melalui C#"
head_description: "Manfaatkan DOCX untuk menambahkan berbagai jenis tanda tangan elektronik ke dokumen, memastikan keamanan dan kepatuhan di seluruh format seperti PDF, Word, Excel, Presentasi, dan Gambar."

############################# Header ############################
title: "Tanda tangan elektronik untuk file DOCX" 
description: "Sisipkan berbagai tanda tangan elektronik ke dalam dokumen Anda menggunakan GroupDocs.Signature for .NET, memastikan kepatuhan dan integritas untuk format seperti PDF, Word, Excel, Presentasi, dan Gambar."
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
    title: "Tentang API GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) menawarkan rangkaian lengkap kemampuan tanda tangan elektronik. Dengan alat ini, Anda dapat dengan mulus menambahkan, mencari, memverifikasi, memperbarui, dan menghapus tanda tangan digital di berbagai jenis dokumen, tanpa memerlukan alat pihak ketiga. Ini mendukung penandatanganan file PDF, dokumen Word, lembar Excel, presentasi PowerPoint, dan berbagai format gambar dengan mudah.

############################# Steps ############################
steps:
    enable: true
    title: "Langkah-langkah untuk menandatangani DOCX menggunakan C#"
    content: |
      [GroupDocs.Signature](/signature/net/) memungkinkan penggabungan tanda tangan kustom ke dalam file DOCX. Pengembang .NET dapat dengan mudah mengintegrasikan fungsionalitas tanda tangan ke dalam aplikasi mereka menggunakan perangkat lunak kami.
      
      1. Sediakan file DOCX kepada instance Signature untuk penandatanganan.
      2. Gunakan SignOptions untuk menentukan parameter tanda tangan.
      3. Atur atribut seperti ukuran, warna, dan konten.
      4. Simpan file yang sudah ditandatangani ke lokasi yang diinginkan.
   
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
        // Muat dokumen ke dalam instance Signature
        using (Signature signature = new Signature("input.docx"))
        {
            // Buat objek QrCodeSignOptions baru
            QrCodeSignOptions options = new QrCodeSignOptions("QR code text")
            {
                // Atur semua opsi yang diperlukan
                Left = 50,
                Top = 200,
                ForeColor = Color.Red
            };

            // Simpan dokumen yang sudah ditandatangani ke penyimpanan lokal
            SignResult result = signature.Sign("output.docx", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Tanda tangan elektronik dokumen yang canggih"
  description: "API tanda tangan elektronik kami yang canggih meningkatkan alur kerja bisnis, memungkinkan penandatanganan, validasi, modifikasi, dan pengelolaan tanda tangan elektronik secara efisien dengan kemampuan otomatisasi penuh."
  image: "/img/signature/features_esign.webp" # 500x500 px
  image_description: "Kemampuan tanda tangan elektronik"
  features:
    # feature loop
    - title: "Tanda tangan elektronik untuk dokumen kantor"
      content: "Sisipkan tanda tangan elektronik di posisi mana pun dalam dokumen. Kustomisasi dan perkaya konten dengan sertifikat digital, metadata, kode batang, atau unsur visual, sambil memastikan keaslian dan keamanan."

    # feature loop
    - title: "Manajemen tanda tangan yang komprehensif"
      content: "Setelah ditandatangani, dokumen dapat diproses lebih lanjut dengan mudah. Akses gambaran lengkap tanda tangan yang ada, memungkinkan pembaruan atau penghapusan tanda tangan yang tepat bila diperlukan."

    # feature loop
    - title: "Keamanan konten yang ditingkatkan"
      content: "Lindungi integritas dokumen Anda menggunakan sertifikat digital. Sisipkan atau ekstrak metadata untuk pelacakan dan audit dokumen yang lebih baik, memastikan kepatuhan dan keaslian konten."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cara menambahkan tanda tangan gambar ke dokumen"
      content: |
        Contoh ini menggambarkan prosedur untuk menerapkan tanda tangan gambar ke halaman tertentu dalam dokumen.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Sediakan dokumen sumber sebagai argumen
          using (Signature signature = new Signature("input.docx"))
          {
              // Tentukan jalur ke gambar dalam konfigurasi tanda tangan
              ImageSignOptions options = new ImageSignOptions("image.jpg")
              {
                  // Tentukan dimensi dan halaman target untuk tanda tangan
                  VerticalAlignment = VerticalAlignment.Bottom,
                  HorizontalAlignment = HorizontalAlignment.Right,
                  Height = 150,
                  Width = 200,
                  Margin = new Padding(50),
                  AllPages = true
              };

              // Eksekusi penerapan tanda tangan ke dokumen
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
            link: "/examples/signature/formats/signature_esign.docx"
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
    title: "Jelajahi semua fitur kami"
    exclude: "esign"
    description: "Kami bangga menawarkan banyak pilihan tanda tangan dan operasi terkait."
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
    title: "Tandai secara digital berbagai jenis format file"
    exclude: "DOCX"
    description: "API .NET memberdayakan Anda untuk menandatangani secara elektronik lebih dari 60 format file standar industri, menawarkan fleksibilitas tiada tara dalam mengamankan dokumen bisnis Anda."
    items: 
          
        # format loop 1
        - name: "Tanda Tangan Elektronik PDF"
          format: "PDF"
          link: "/signature/net/esign/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Tanda Tangan Elektronik DOCX"
          format: "DOCX"
          link: "/signature/net/esign/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Tanda Tangan Elektronik JPEG"
          format: "JPEG"
          link: "/signature/net/esign/jpeg/"
          description: "Gambar JPEG"
          
        # format loop 4
        - name: "Tanda Tangan Elektronik PPTX"
          format: "PPTX"
          link: "/signature/net/esign/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 5
        - name: "Tanda Tangan Elektronik XLSX"
          format: "XLSX"
          link: "/signature/net/esign/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---