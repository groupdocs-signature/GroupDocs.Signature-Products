



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:54
draft: false
lang: id
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Buat tanda tangan teks XLSX dengan Java"
head_description: "Manfaatkan API Java untuk menyisipkan tanda tangan teks ke dalam file XLSX. Proses berbagai format dokumen populer dengan lancar termasuk PDF, Word, Excel, Presentasi, Gambar, dan ZIP."

############################# Header ############################
title: "Buat tanda tangan teks untuk XLSX" 
description: "Tambahkan tanda tangan teks kustom pada dokumen bisnis Anda menggunakan GroupDocs.Signature for Java. Sempurnakan alur kerja organisasi dengan opsi kustomisasi tanda tangan."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Mulai secara gratis"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "Tentang solusi GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) menyediakan tanda tangan teks yang fleksibel dan dapat disesuaikan untuk menyederhanakan tugas manajemen dokumen Anda. Atur konten dan desain tanda tangan teks dan terapkan ke halaman mana pun, meningkatkan alur kerja dokumen organisasi Anda.

############################# Steps ############################
steps:
    enable: true
    title: "Langkah untuk menambahkan tanda tangan teks ke XLSX menggunakan Java"
    content: |
      [GroupDocs.Signature](/signature/java/) dapat diintegrasikan ke dalam aplikasi Java untuk menambahkan tanda tangan teks ke dokumen XLSX. Pengembang dapat dengan cepat meningkatkan fungsionalitas produk mereka dengan menggunakan solusi kami.
      
      1. Gunakan dokumen XLSX sebagai parameter untuk konstruktor kelas Signature.
      2. Instansiasi TextSignOptions dengan teks yang sesuai.
      3. Konfigurasi opsi visual untuk tanda tangan.
      4. Tambahkan tanda tangan teks ke halaman mana pun dari dokumen.
   
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
        // Lewati jalur dokumen ke konstruktor Signature
        Signature signature = new Signature("input.xlsx");

        // Instansiasi TextSignOptions dengan teks tanda tangan
        TextSignOptions options = new TextSignOptions("Approved");
        
        // Atur atribut warna dan font teks
        options.setForeColor(Color.RED);
        SignatureFont signatureFont = new SignatureFont();
        signatureFont.setSize(12);
        signatureFont.setFamilyName("Comic Sans MS");
        options.setFont(signatureFont);

        // Tambahkan tanda tangan teks ke dokumen
        SignResult result = signature.sign("output.xlsx", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Kelola tanda tangan teks dokumen"
  description: "Dengan GroupDocs.Signature for Java, Anda dapat memperlancar alur kerja dokumen perusahaan Anda dengan menambahkan tanda tangan teks ke format file populer. Sesuaikan tampilan dan konten tanda tangan dengan mudah."
  image: "/img/signature/features_text.webp" # 500x500 px
  image_description: "Fitur utama GroupDocs.Signature"
  features:
    # feature loop
    - title: "Tanda tangan dokumen"
      content: "Terapkan tanda tangan teks, gambar, kode batang, kode QR, atau stempel ke halaman mana pun dari dokumen yang didukung. Manfaatkan metadata untuk menyematkan konten tersembunyi dan mengamankan dokumen Anda dengan sertifikat digital."

    # feature loop
    - title: "Pencarian dan verifikasi tanda tangan"
      content: "Pastikan integritas dokumen yang telah ditandatangani dengan alat verifikasi tanda tangan kami. Anda juga dapat mengambil dan mencari semua tanda tangan yang disematkan dalam dokumen."

    # feature loop
    - title: "Ubah atau hapus tanda tangan"
      content: "Ubah konten, posisi, dan tampilan tanda tangan yang telah ditambahkan sebelumnya, atau hapus sepenuhnya dari dokumen."

    # feature loop
    - title: "Tanda tangan teks asli"
      content: "Tambahkan tanda tangan teks spesifik dokumen, seperti stiker di PDF atau watermark di dokumen Word, untuk kustomisasi yang lebih baik."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Tandai dokumen dengan tanda tangan teks"
      content: |
        Pelajari cara menambahkan informasi tekstual ke dokumen bisnis untuk meningkatkan proses bisnis.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Pilih dokumen yang akan ditandatangani
          Signature signature = new Signature("input.xlsx");

          // Buat opsi teks dengan teks yang diinginkan
          TextSignOptions options = new TextSignOptions("Rescheduled to 03/04/2025");

          // Tentukan ukuran dan posisi tanda tangan di halaman
          options.setLeft(100);
          options.setTop(180);
          options.setWidth(230);
          options.setHeight(30);

          // Tanda tangan mendukung padding dari sudut halaman
          Padding padding = new Padding();
          padding.setBottom(20);
          padding.setRight(20);
          options.setMargin(padding);

          // Warna teks dan gaya font dapat dikustomisasi
          options.setForeColor(Color.RED);
          SignatureFont signatureFont = new SignatureFont();
          signatureFont.setSize(12);
          signatureFont.setFamilyName("Comic Sans MS");
          options.setFont(signatureFont);

          // Tanda tangan teks dapat menyertakan batas
          Border border = new Border();
          border.setColor(Color.RED);
          border.setDashStyle(DashStyle.Dash);
          border.setTransparency(0.5);
          border.setVisible(true);
          border.setWeight(2);
          options.setBorder(border);

          // Kustomisasi latar belakang juga tersedia
          Background background = new Background();
          background.setColor(Color.YELLOW);
          background.setTransparency(0.8);
          options.setBackground(background);

          // Teks dapat disimpan sebagai gambar untuk kompatibilitas
          options.setSignatureImplementation(TextSignatureImplementation.Image);

          // Simpan dokumen dengan tambahan teks
          SignResult result = signature.sign("output.xlsx", options);
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
            link: "/examples/signature/formats/signature_text.xlsx"
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
    title: "Fitur utama dan opsi tanda tangan"
    exclude: "text"
    description: "Solusi kami mendukung operasi CRUD penuh dan lebih banyak lagi untuk tujuh jenis tanda tangan yang berbeda."
    items: 
          
        # operation loop 1
        - name: "Tanda Tangan Elektronik"
          operation: "esign"
          link: "/signature/java/esign/xlsx/"
          description: "Tambahkan berbagai jenis tanda tangan ke format file yang didukung"

        # operation loop 2
        - name: "Tambahkan teks ke dokumen"
          operation: "text"
          link: "/signature/java/text/xlsx/"
          description: "Tingkatkan konten dokumen dengan tanda tangan teks yang dapat disesuaikan"

        # operation loop 3
        - name: "Tanda Tangan Gambar"
          operation: "image"
          link: "/signature/java/image/xlsx/"
          description: "Tempatkan gambar di posisi mana pun dalam dokumen"

        # operation loop 4
        - name: "Hasilkan barcode"
          operation: "barcode"
          link: "/signature/java/barcode/xlsx/"
          description: "Buat dan sisipkan berbagai barcode ke dalam dokumen yang didukung"

        # operation loop 5
        - name: "Hasilkan QR code"
          operation: "qrcode"
          link: "/signature/java/qrcode/xlsx/"
          description: "Buat dan QR Code, termasuk QR code, untuk penandatanganan dokumen"
          
        # operation loop 6
        - name: "Sertifikat Digital"
          operation: "digital"
          link: "/signature/java/digital/xlsx/"
          description: "Amankan bisnis dan tanda tangani dokumen dengan sertifikat digital"

        # operation loop 7
        - name: "Tanda Tangan Stempel"
          operation: "stamp"
          link: "/signature/java/stamp/xlsx/"
          description: "Gunakan Konstruksi Stempel untuk membuat stempel bulat atau persegi yang kustom"
          
        # operation loop 8
        - name: "Cari tanda tangan"
          operation: "search"
          link: "/signature/java/search/xlsx/"
          description: "Temukan tanda tangan yang ditambahkan sebelumnya dalam dokumen"
          
        # operation loop 9
        - name: "Verifikasi tanda tangan"
          operation: "verify"
          link: "/signature/java/verify/xlsx/"
          description: "Verifikasi keaslian tanda tangan setelah diterapkan"
          
        # operation loop 10
        - name: "Modifikasi tanda tangan"
          operation: "modify"
          link: "/signature/java/modify/xlsx/"
          description: "Edit berbagai tanda tangan dalam dokumen"
          
        # operation loop 11
        - name: "Hapus tanda tangan"
          operation: "delete"
          link: "/signature/java/delete/xlsx/"
          description: "Hapus berbagai tanda tangan yang diterapkan sebelumnya"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Tambahkan tanda tangan teks ke berbagai format file"
    exclude: "XLSX"
    description: "Manfaatkan API Java untuk menyisipkan tanda tangan teks ke dalam dokumen Office, memastikan kontrol penuh atas konten di setiap tahap siklus hidup dokumen."
    items: 
          
        # format loop 1
        - name: "Tanda Tangan Teks PDF"
          format: "PDF"
          link: "/signature/java/text/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Tanda Tangan Teks DOCX"
          format: "DOCX"
          link: "/signature/java/text/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Tanda Tangan Teks JPEG"
          format: "JPEG"
          link: "/signature/java/text/jpeg/"
          description: "Gambar JPEG"
          
        # format loop 4
        - name: "Tanda Tangan Teks PPTX"
          format: "PPTX"
          link: "/signature/java/text/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 5
        - name: "Tanda Tangan Teks XLSX"
          format: "XLSX"
          link: "/signature/java/text/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---