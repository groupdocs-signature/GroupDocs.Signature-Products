



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:20
draft: false
lang: id
format: Pptx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Buat kode QR untuk PPTX dengan Java"
head_description: "API GroupDocs.Signature memungkinkan pembuatan kode QR untuk file PPTX. Buat kode QR dari konten Anda dan tempatkan di halaman mana pun."

############################# Header ############################
title: "Buat kode QR untuk PPTX" 
description: "Buat kode batang 2D dengan data teks dan numerik dan tempatkan di halaman mana pun dari berbagai dokumen menggunakan GroupDocs.Signature for Java."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Uji coba gratis"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "Pelajari lebih lanjut tentang GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) menawarkan berbagai fitur untuk menghasilkan dan menyisipkan berbagai jenis tanda tangan dalam semua format dokumen utama. Ini mendukung PDF, dokumen Word, spreadsheet Excel, presentasi PowerPoint, dan gambar. Tingkatkan dokumen Anda dengan tanda tangan Teks, Gambar, Barcode, Kode QR, Metadata, Digital, dan Stempel.

############################# Steps ############################
steps:
    enable: true
    title: "Langkah-langkah untuk menghasilkan dan menempatkan kode QR di lokasi mana pun dalam PPTX"
    content: |
      [GroupDocs.Signature](/signature/java/) dapat menghasilkan kode QR dalam banyak format populer dan menempatkannya di halaman PPTX. Lebih dari 10 jenis kode QR didukung dan dapat dengan cepat diintegrasikan ke dalam aplikasi Java. Gunakan produk kami untuk menandatangani dokumen dengan kode QR yang dihasilkan.
      
      1. Dapatkan file atau aliran PPTX yang akan ditandatangani dengan kode QR.
      2. Sediakan teks untuk QrCodeSignOptions.
      3. Sesuaikan opsi visual seperti warna, posisi, ukuran, dll.
      4. Simpan file dengan kode QR.
   
    code:
      platform: "java"
      copy_title: "Salin"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Contoh tanda tangan"
      install:
        command_title: "Maven XML"
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-signature</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "klik untuk menyalin"
        copy_done: "disalin"
      links:
        #  loop
        - title: "Lebih banyak contoh"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
        #  loop
        - title: "Dokumentasi"
          link: "https://docs.groupdocs.com/signature/java/"
          
      content: |
        ```java {style=abap}
        // Serahkan dokumen ke instance Signature baru
        Signature signature = new Signature("input.pptx");

        // Gunakan QrCodeSignOptions untuk menambahkan kode QR ke dokumen
        QrCodeSignOptions options = new QrCodeSignOptions("Text Content");

        // Tentukan tipe tanda tangan dan posisinya di halaman
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(50);
        options.setTop(150);

        // Simpan file dengan kode QR yang ditambahkan
        signature.sign("output.pptx", options);

        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Tambahkan tanda tangan ke dokumen Anda"
  description: "API GroupDocs.Signature for Java mendukung penandatanganan semua format file populer. Hasilkan, modifikasi, cari, verifikasi, dan hapus berbagai jenis tanda tangan."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "Fitur Utama GroupDocs.Signature"
  features:
    # feature loop
    - title: "Tanda tangani dokumen"
      content: "GroupDocs.Signature mendukung penandatanganan dengan tanda tangan Teks, Gambar, Barcode, Kode QR, dan Stempel. Tempatkan mereka di halaman mana pun dari format dokumen yang didukung. Kelola metadata dokumen dengan tanda tangan metadata, dan lindungi konten dari perubahan yang tidak sah menggunakan sertifikat digital."

    # feature loop
    - title: "Pencarian dan verifikasi"
      content: "Pastikan semua tanda tangan dalam dokumen valid melalui prosedur verifikasi. Ambil daftar lengkap tanda tangan dalam dokumen menggunakan fitur pencarian bawaan."

    # feature loop
    - title: "Modifikasi tanda tangan"
      content: "Modifikasi sifat tanda tangan setelah tanda tangan dengan mudah. Sesuaikan konten, posisi, warna, ukuran, dan atribut lainnya sesuai kebutuhan."

    # feature loop
    - title: "Hapus tanda tangan"
      content: "Hapus tanda tangan yang tidak diinginkan dengan mudah. Berbagai jenis tanda tangan, termasuk sertifikat digital, dapat dihapus secara programatis dari dokumen."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cara menyesuaikan kode QR yang dihasilkan"
      content: |
        Gunakan contoh ini untuk belajar cara menempatkan kode QR baru di halaman PPTX.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Ambil dokumen yang perlu ditandatangani dan serahkan ke Signature
          Signature signature = new Signature("input.pptx");

          // Gunakan opsi kode QR untuk memberikan teks dengan informasi yang diperlukan
          QrCodeSignOptions signOptions = new QrCodeSignOptions("Archived on July 11, 2019");

          // Tentukan posisi relatif kode QR di halaman
          signOptions.setVerticalAlignment(VerticalAlignment.Top);
          signOptions.setHorizontalAlignment(HorizontalAlignment.Right);

          // Tentukan padding tanda tangan
          Padding padding = new Padding();
          padding.setRight(20);
          padding.setTop(20);
          signOptions.setMargin(padding);

          // Tentukan warna kode QR
          signOptions.setForeColor(Color.RED);

          // Tentukan opsi font untuk pesan
          SignatureFont font = new SignatureFont();
          font.setSize(12);
          font.setFamilyName("Comic Sans MS");
          signOptions.setFont(font);

          // Sesuaikan warna latar belakang dan kuas kode QR
          Background background = new Background();
          background.setColor(Color.GREEN);
          background.setTransparency(0.5);
          background.setBrush(new LinearGradientBrush(Color.GREEN, Color.DARK_GRAY, 0));
          signOptions.setBackground(background);

          // Tambahkan kode QR ke dokumen
          SignResult signResult = signature.sign("output.pptx", signOptions);
          ```
        platform: "java"
        copy_title: "Salin"
        install:
          command_title: "Maven XML"
          command: |
            <dependencies>
              <dependency>
                <groupId>com.groupdocs</groupId>
                <artifactId>groupdocs-signature</artifactId>
                <version>{0}</version>
              </dependency>
            </dependencies>
            <repositories>
              <repository>
                <id>repository.groupdocs.com</id>
                <name>GroupDocs Repository</name>
                <url>https://repository.groupdocs.com/repo/</url>
              </repository>
            </repositories>
          copy_tip: "klik untuk menyalin"
          copy_done: "disalin"
        top_links:
          #  loop
          - title: "Unduh hasil"
            icon: "download"
            link: "/examples/signature/formats/signature_qrcode.pptx"
        links:
          #  loop
          - title: "Lebih banyak contoh"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
          #  loop
          - title: "Dokumentasi"
            link: "https://docs.groupdocs.com/signature/java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Siap untuk memulai?"
  description: "Coba fitur GroupDocs.Signature secara gratis atau minta lisensi"
  items:
    #  loop
    - title: "Unduhan Maven"
      link: "https://releases.groupdocs.com/signature/java/"
      color: "red"
        #  loop
    - title: "Lisensi"
      link: "https://purchase.groupdocs.com/pricing/signature/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Periksa penawaran utama kami"
    exclude: "qrcode"
    description: "Kami menawarkan berbagai pilihan fitur tanda tangan dan operasi lanjutan."
    items: 
          
        # operation loop 1
        - name: "Tanda Tangan Elektronik"
          operation: "esign"
          link: "/signature/java/esign/pptx/"
          description: "Tambahkan berbagai jenis tanda tangan ke format file yang didukung"

        # operation loop 2
        - name: "Tambahkan teks ke dokumen"
          operation: "text"
          link: "/signature/java/text/pptx/"
          description: "Tingkatkan konten dokumen dengan tanda tangan teks yang dapat disesuaikan"

        # operation loop 3
        - name: "Tanda Tangan Gambar"
          operation: "image"
          link: "/signature/java/image/pptx/"
          description: "Tempatkan gambar di posisi mana pun dalam dokumen"

        # operation loop 4
        - name: "Hasilkan barcode"
          operation: "barcode"
          link: "/signature/java/barcode/pptx/"
          description: "Buat dan sisipkan berbagai barcode ke dalam dokumen yang didukung"

        # operation loop 5
        - name: "Hasilkan QR code"
          operation: "qrcode"
          link: "/signature/java/qrcode/pptx/"
          description: "Buat dan QR Code, termasuk QR code, untuk penandatanganan dokumen"
          
        # operation loop 6
        - name: "Sertifikat Digital"
          operation: "digital"
          link: "/signature/java/digital/pptx/"
          description: "Amankan bisnis dan tanda tangani dokumen dengan sertifikat digital"

        # operation loop 7
        - name: "Tanda Tangan Stempel"
          operation: "stamp"
          link: "/signature/java/stamp/pptx/"
          description: "Gunakan Konstruksi Stempel untuk membuat stempel bulat atau persegi yang kustom"
          
        # operation loop 8
        - name: "Cari tanda tangan"
          operation: "search"
          link: "/signature/java/search/pptx/"
          description: "Temukan tanda tangan yang ditambahkan sebelumnya dalam dokumen"
          
        # operation loop 9
        - name: "Verifikasi tanda tangan"
          operation: "verify"
          link: "/signature/java/verify/pptx/"
          description: "Verifikasi keaslian tanda tangan setelah diterapkan"
          
        # operation loop 10
        - name: "Modifikasi tanda tangan"
          operation: "modify"
          link: "/signature/java/modify/pptx/"
          description: "Edit berbagai tanda tangan dalam dokumen"
          
        # operation loop 11
        - name: "Hapus tanda tangan"
          operation: "delete"
          link: "/signature/java/delete/pptx/"
          description: "Hapus berbagai tanda tangan yang diterapkan sebelumnya"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Hasilkan kode QR untuk format file tambahan"
    exclude: "PPTX"
    description: "Tingkatkan semua format file populer dengan kode QR yang dihasilkan menggunakan API Java. Tambahkan data barcode 2D untuk pemindaian dan pemrosesan yang mudah."
    items: 
          
        # format loop 1
        - name: "QR-Code untuk PDF"
          format: "PDF"
          link: "/signature/java/qrcode/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "QR-Code untuk DOCX"
          format: "DOCX"
          link: "/signature/java/qrcode/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "QR-Code untuk JPEG"
          format: "JPEG"
          link: "/signature/java/qrcode/jpeg/"
          description: "Gambar JPEG"
          
        # format loop 4
        - name: "QR-Code untuk PPTX"
          format: "PPTX"
          link: "/signature/java/qrcode/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 5
        - name: "QR-Code untuk XLSX"
          format: "XLSX"
          link: "/signature/java/qrcode/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---