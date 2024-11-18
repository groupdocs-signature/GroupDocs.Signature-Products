



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:50
draft: false
lang: id
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Menambahkan Tanda Tangan Gambar ke file JPEG dengan Java"
head_description: "Tempatkan tanda tangan gambar di file JPEG untuk Java dengan beberapa baris kode. Gunakan API GroupDocs.Signature for Java untuk menambahkan gambar."

############################# Header ############################
title: "Tanda tangani file JPEG dengan tanda tangan gambar" 
description: "Gunakan GroupDocs.Signature for Java untuk menyisipkan gambar ke dalam berbagai format dokumen kantor, termasuk PDF, Word, Excel, dan file gambar. Gambar dengan tanda tangan atasan dapat menambah kesan yang mengesankan!"
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Unduh gratis"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "Temukan GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) menawarkan kemampuan untuk menambahkan tanda tangan gambar ke setiap halaman dan posisi dalam dokumen bisnis. Permudah alur kerja Anda dengan menambahkan gambar ke PDF, dokumen Word, spreadsheet Excel, presentasi PowerPoint, dan format gambar populer.

############################# Steps ############################
steps:
    enable: true
    title: "Langkah-langkah untuk menambahkan gambar ke mana saja dalam JPEG melalui Java"
    content: |
      [GroupDocs.Signature](/signature/java/) memperkaya aplikasi Java dengan kemampuan untuk menambahkan tanda tangan ke halaman mana saja dari dokumen JPEG secara tepat. Tingkatkan fungsionalitas produk Anda dengan mengintegrasikan pustaka kami.
      
      1. Buat instance Signature dengan dokumen JPEG.
      2. Gunakan ImageSignOptions untuk menentukan gambar tanda tangan.
      3. Tempatkan gambar di lokasi mana saja di halaman mana saja.
      4. Simpan dokumen yang ditandatangani ke lokasi baru.
   
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
        // Instansiasi Signature dengan jalur dokumen
        Signature signature = new Signature("input.jpeg");

        // Buat ImageSignOptions menggunakan gambar untuk tanda tangan
        ImageSignOptions options = new ImageSignOptions("company_logo.jpg");

        // Posisikan gambar di sudut kiri atas semua halaman
        options.setAllPages(true);
        options.setLeft(100);
        options.setTop(200);

        // Simpan dokumen yang ditandatangani
        SignResult result = signature.sign("output.jpeg", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Solusi tanda tangan dokumen yang komprehensif"
  description: "API kami mendukung berbagai fitur tanda tangan, memungkinkan Anda untuk menambah, memodifikasi, menghapus, mencari, dan memverifikasi berbagai jenis tanda tangan, termasuk tanda tangan gambar."
  image: "/img/signature/features_image.webp" # 500x500 px
  image_description: "Tanda tangan gambar"
  features:
    # feature loop
    - title: "Sisipkan gambar ke dokumen kantor"
      content: "Tempatkan tanda tangan gambar dengan mudah di posisi mana pun di halaman dokumen. Perkaya konten Anda dengan teks, gambar, barcode, metadata, dan sertifikat digital."

    # feature loop
    - title: "Pencarian dan verifikasi tanda tangan"
      content: "Verifikasi validitas tanda tangan di dokumen yang ditandatangani. Ambil daftar semua tanda tangan dalam sebuah dokumen dan periksa informasi mendetail tentang masing-masing."

    # feature loop
    - title: "Modifikasi tanda tangan"
      content: "Perbarui konten, penampilan, ukuran, atau posisi tanda tangan yang pernah ditambahkan ke dokumen. API kami membuat modifikasi tanda tangan menjadi sederhana dan efisien."

    # feature loop
    - title: "Hapus tanda tangan yang tidak diperlukan"
      content: "API kami mendukung operasi CRUD penuh untuk sebagian besar jenis tanda tangan. Anda dapat dengan mudah menghapus tanda tangan dari hampir semua jenis dokumen yang didukung jika diperlukan."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Tingkatkan konten dokumen dengan tanda tangan gambar"
      content: |
        Pelajari cara menambahkan gambar ke dokumen bisnis untuk memberikan informasi tambahan.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Pilih dokumen yang akan ditandatangani
          Signature signature = new Signature("input.jpeg");

          // Buat opsi gambar dengan jalur ke gambar
          ImageSignOptions options = new ImageSignOptions("manager_signature.jpg");

          // Tentukan ukuran tanda tangan gambar
          options.setWidth(100);
          options.setHeight(100);

          // Tempatkan gambar di sudut kanan bawah
          options.setVerticalAlignment(VerticalAlignment.Bottom);
          options.setHorizontalAlignment(HorizontalAlignment.Right);

          // Terapkan padding dari sudut halaman jika perlu
          Padding padding = new Padding();
          padding.setRight(120);
          padding.setBottom(120);
          options.setMargin(padding);

          // Tambahkan tepi kustom ke gambar jika diinginkan
          Border border = new Border();
          border.setColor(Color.RED);
          border.setDashStyle(DashStyle.DashDotDot);
          border.setWeight(5);
          border.setVisible(true);
          options.setBorder(border);

          // Putar tanda tangan untuk penyesuaian yang lebih baik
          options.setRotationAngle(45);

          // Simpan dokumen yang diperbarui ke lokasi mana saja
          SignResult result = signature.sign("output.jpeg", options);

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
            link: "/examples/signature/formats/signature_image.jpeg"
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
    title: "Lihat fitur unggulan kami"
    exclude: "image"
    description: "Kami dengan senang hati mempresentasikan berbagai alat dan operasi tanda tangan."
    items: 
          
        # operation loop 1
        - name: "Tanda Tangan Elektronik"
          operation: "esign"
          link: "/signature/java/esign/jpeg/"
          description: "Tambahkan berbagai jenis tanda tangan ke format file yang didukung"

        # operation loop 2
        - name: "Tambahkan teks ke dokumen"
          operation: "text"
          link: "/signature/java/text/jpeg/"
          description: "Tingkatkan konten dokumen dengan tanda tangan teks yang dapat disesuaikan"

        # operation loop 3
        - name: "Tanda Tangan Gambar"
          operation: "image"
          link: "/signature/java/image/jpeg/"
          description: "Tempatkan gambar di posisi mana pun dalam dokumen"

        # operation loop 4
        - name: "Hasilkan barcode"
          operation: "barcode"
          link: "/signature/java/barcode/jpeg/"
          description: "Buat dan sisipkan berbagai barcode ke dalam dokumen yang didukung"

        # operation loop 5
        - name: "Hasilkan QR code"
          operation: "qrcode"
          link: "/signature/java/qrcode/jpeg/"
          description: "Buat dan QR Code, termasuk QR code, untuk penandatanganan dokumen"
          
        # operation loop 6
        - name: "Sertifikat Digital"
          operation: "digital"
          link: "/signature/java/digital/pdf/"
          description: "Amankan bisnis dan tanda tangani dokumen dengan sertifikat digital"

        # operation loop 7
        - name: "Tanda Tangan Stempel"
          operation: "stamp"
          link: "/signature/java/stamp/jpeg/"
          description: "Gunakan Konstruksi Stempel untuk membuat stempel bulat atau persegi yang kustom"
          
        # operation loop 8
        - name: "Cari tanda tangan"
          operation: "search"
          link: "/signature/java/search/pdf/"
          description: "Temukan tanda tangan yang ditambahkan sebelumnya dalam dokumen"
          
        # operation loop 9
        - name: "Verifikasi tanda tangan"
          operation: "verify"
          link: "/signature/java/verify/pdf/"
          description: "Verifikasi keaslian tanda tangan setelah diterapkan"
          
        # operation loop 10
        - name: "Modifikasi tanda tangan"
          operation: "modify"
          link: "/signature/java/modify/pdf/"
          description: "Edit berbagai tanda tangan dalam dokumen"
          
        # operation loop 11
        - name: "Hapus tanda tangan"
          operation: "delete"
          link: "/signature/java/delete/pdf/"
          description: "Hapus berbagai tanda tangan yang diterapkan sebelumnya"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Tambahkan gambar ke format file lainnya"
    exclude: "JPEG"
    description: "Dengan API Java, Anda dapat menyisipkan format gambar yang didukung ke dalam berbagai dokumen. Sesuaikan ukuran, pilih posisi, dan tambahkan tanda tangan gambar ke dokumen Anda."
    items: 
          
        # format loop 1
        - name: "Tanda Tangan PDF dengan Gambar"
          format: "PDF"
          link: "/signature/java/image/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Tanda Tangan DOCX dengan Gambar"
          format: "DOCX"
          link: "/signature/java/image/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Tanda Tangan JPEG dengan Gambar"
          format: "JPEG"
          link: "/signature/java/image/jpeg/"
          description: "Gambar JPEG"
          
        # format loop 4
        - name: "Tanda Tangan PPTX dengan Gambar"
          format: "PPTX"
          link: "/signature/java/image/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 5
        - name: "Tanda Tangan XLSX dengan Gambar"
          format: "XLSX"
          link: "/signature/java/image/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---