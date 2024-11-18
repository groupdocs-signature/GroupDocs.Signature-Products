



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:06
draft: false
lang: id
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Hasilkan kode batang untuk JPEG menggunakan API C#"
head_description: "Hasilkan tanda tangan kode batang dan amankan dokumen JPEG menggunakan C# hanya dengan beberapa baris kode. Manfaatkan GroupDocs.Signature untuk menandatangani berbagai format file."

############################# Header ############################
title: "Hasilkan kode batang untuk dokumen JPEG" 
description: "Manfaatkan GroupDocs.Signature for .NET untuk menempatkan kode batang di mana saja dalam dokumen bisnis Anda. API kami menawarkan opsi kustomisasi yang luas untuk tanda tangan kode batang."
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
    title: "Ikhtisar GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) adalah solusi tanda tangan dokumen yang canggih yang mendukung berbagai jenis tanda tangan, termasuk teks, gambar, kode batang, sertifikat digital, dan cap. Kompatibel dengan lebih dari 60 format file—seperti PDF, MS Office, gambar, file ZIP, dan banyak lagi—alat ini memungkinkan Anda untuk tidak hanya menerapkan tanda tangan tetapi juga mencari, memverifikasi, memodifikasi, atau menghapusnya sesuai kebutuhan.

############################# Steps ############################
steps:
    enable: true
    title: "Langkah-langkah untuk menghasilkan dan menyematkan kode batang dalam file JPEG"
    content: |
      [GroupDocs.Signature](/signature/net/) memfasilitasi pembuatan kode batang dalam berbagai format populer dan penempatannya di halaman JPEG. Mendukung lebih dari 60 jenis kode batang, aplikasi .NET dapat dengan mudah ditingkatkan dengan fungsi penandatanganan kode batang dengan mengintegrasikan library kami.
      
      1. Sediakan file atau stream JPEG untuk diproses.
      2. Serahkan teks kode batang ke instance BarcodeSignOptions.
      3. Sesuaikan opsi kode batang seperti posisi, ukuran, dll.
      4. Simpan file dengan kode batang yang baru ditambahkan.
   
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
        // Instansiasi objek Signature baru dengan jalur dokumen
        using (Signature signature = new Signature("input.jpeg"))
        {
            // Gunakan BarcodeSignOptions untuk menambahkan kode batang ke dokumen
            BarcodeSignOptions options = new BarcodeSignOptions("Business data")
            {
                // Konfigurasikan jenis kode batang dan properti tambahan
                EncodeType = BarcodeTypes.Code128,
                Left = 50,
                Top = 150
            };

            // Simpan file yang ditandatangani
            SignResult result = signature.Sign("output.jpeg", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Tingkatkan dan lindungi dokumen Anda dengan kemampuan tanda tangan yang canggih"
  description: "Library GroupDocs.Signature for .NET dirancang untuk memfasilitasi penandatanganan dokumen menyeluruh dan pemrosesan di berbagai format file yang umum digunakan. Anda dapat menambahkan, menyesuaikan, memverifikasi, atau menghapus berbagai jenis tanda tangan."
  image: "/img/signature/features_barcode.webp" # 500x500 px
  image_description: "Fitur Utama GroupDocs.Signature"
  features:
    # feature loop
    - title: "Penandatanganan dokumen yang fleksibel"
      content: "Tandatangani dengan efisien setiap halaman dalam dokumen yang didukung menggunakan teks, gambar, kode batang, kode QR, atau cap. Selain itu, tambahkan metadata tersembunyi, seperti data EXIF dalam gambar, atau amankan konten dokumen Anda dari perubahan tidak sah menggunakan sertifikat digital."

    # feature loop
    - title: "Pencarian dan verifikasi tanda tangan yang menyeluruh"
      content: "Alat kami menawarkan fungsi yang kuat untuk bekerja dengan dokumen yang ditandatangani. Pastikan integritas dokumen Anda dengan memverifikasi tanda tangan, dan ambil daftar lengkap semua tanda tangan dalam dokumen dengan mudah melalui fitur pencarian kami."

    # feature loop
    - title: "Edit tanda tangan dengan gampang"
      content: "Hampir semua tanda tangan yang telah diterapkan sebelumnya dapat dimodifikasi. Dengan nyaman, perbarui teks, sesuaikan posisi, atau ubah warna sesuai kebutuhan Anda."

    # feature loop
    - title: "Penghapusan tanda tangan yang efisien"
      content: "Pendekatan kami sepenuhnya mendukung operasi CRUD untuk tanda tangan, memungkinkan penghapusan cepat dari tanda tangan yang tidak diinginkan atau kadaluarsa dari dokumen Anda."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cara menghasilkan tanda tangan kode batang"
      content: |
        Contoh ini menunjukkan cara menyematkan kode batang yang dikustomisasi pada halaman dokumen JPEG.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          using (Signature signature = new Signature("input.jpeg"))
          {
              // Rumuskan opsi tanda tangan dengan teks yang diinginkan
              BarcodeSignOptions options = new BarcodeSignOptions("Accepted")
              {
                  EncodeType = BarcodeTypes.Code39FullASCII,

                  // Tentukan posisi relatif kode batang di halaman
                  VerticalAlignment = Domain.VerticalAlignment.Top,
                  HorizontalAlignment = Domain.HorizontalAlignment.Left,

                  // Tentukan jarak kode batang dari tepi halaman
                  Margin = new Padding() { Top = 180, Right = 20 },

                  // Tentukan warna batang
                  ForeColor = Color.Red,

                  // Pilih gaya font untuk pesan
                  Font = new SignatureFont { Size = 12, FamilyName = "Arial" },

                  // Tentukan posisi pesan
                  CodeTextAlignment = CodeTextAlignment.Above
              };

              // Tandatangani dan simpan dokumen
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
            link: "/examples/signature/formats/signature_barcode.jpeg"
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
    title: "Temukan fitur utama kami"
    exclude: "barcode"
    description: "Kami menawarkan pilihan dan operasi tanda tangan yang mengesankan"
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
    title: "Tandatangani dokumen dalam berbagai format"
    exclude: "JPEG"
    description: "API .NET kami mendukung penandatanganan lebih dari 60 format berbeda. Dengan mudah tempatkan berbagai jenis tanda tangan pada setiap halaman atau di posisi yang diinginkan dalam dokumen Anda."
    items: 
          
        # format loop 1
        - name: "Tambahkan barcode ke PDF"
          format: "PDF"
          link: "/signature/net/barcode/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Tambahkan barcode ke DOCX"
          format: "DOCX"
          link: "/signature/net/barcode/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Tambahkan barcode ke JPEG"
          format: "JPEG"
          link: "/signature/net/barcode/jpeg/"
          description: "Gambar JPEG"
          
        # format loop 4
        - name: "Tambahkan barcode ke PPTX"
          format: "PPTX"
          link: "/signature/net/barcode/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 5
        - name: "Tambahkan barcode ke XLSX"
          format: "XLSX"
          link: "/signature/net/barcode/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---