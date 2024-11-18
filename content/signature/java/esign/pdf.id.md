



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:09
draft: false
lang: id
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Tanda tangan e-Sign berkas PDF dengan aplikasi Java"
head_description: "Gunakan API Java untuk memproses berkas PDF dan menerapkan berbagai jenis tanda tangan, termasuk PDF, Word, Excel, Presentasi, dan Gambar."

############################# Header ############################
title: "Tanda tangan elektronik untuk PDF" 
description: "Tambahkan berbagai tanda tangan elektronik menggunakan GroupDocs.Signature for Java ke semua format bisnis populer, termasuk PDF, Word, Excel, Presentasi, dan Gambar."
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
    title: "Tentang API GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) menawarkan fitur tanda tangan elektronik yang canggih. Gunakan untuk menambah, mencari, memverifikasi, memodifikasi, dan menghapus berbagai jenis tanda tangan elektronik dalam dokumen dan gambar tanpa memerlukan perangkat lunak eksternal. Tandai PDF, dokumen Word, spreadsheet Excel, presentasi PowerPoint, dan format gambar populer dengan mudah.

############################# Steps ############################
steps:
    enable: true
    title: "Langkah-langkah untuk menandatangani PDF menggunakan Java"
    content: |
      [GroupDocs.Signature](/signature/java/) memungkinkan penambahan tanda tangan kustom ke berkas PDF. Pengembang Java dapat mengintegrasikan fungsionalitas tanda tangan ke dalam aplikasi mereka menggunakan perangkat lunak kami.
      
      1. Berikan berkas PDF yang akan ditandatangani ke instance Signature.
      2. Gunakan SignOptions untuk mendefinisikan rincian tanda tangan.
      3. Sesuaikan berbagai properti seperti ukuran, warna, dan konten.
      4. Simpan berkas yang ditandatangani ke lokasi yang diinginkan.
   
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
        // Muat dokumen ke dalam instance Signature
        Signature signature = new Signature("input.pdf");

        // Buat objek QrCodeSignOptions
        QrCodeSignOptions options = new QrCodeSignOptions("QR code text");

        // Konfigurasikan semua opsi yang diinginkan
        options.setLeft(100);
        options.setTop(100);
        options.setForeColor(Color.RED);

        // Simpan berkas dengan kode QR yang ditambahkan ke disk lokal
        signature.sign("output.pdf", options);
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Tanda tangan elektronik dokumen"
  description: "API tanda tangan elektronik kami mempermudah proses bisnis. Tandai, cari, perbarui, hapus, dan verifikasi berbagai tanda tangan secara programatis."
  image: "/img/signature/features_esign.webp" # 500x500 px
  image_description: "Tanda tangan elektronik"
  features:
    # feature loop
    - title: "Tanda tangan dokumen kantor"
      content: "Tempatkan tanda tangan elektronik di posisi manapun di halaman dokumen. Tingkatkan konten dokumen dengan teks, gambar, kode batang, metadata, atau sertifikat digital."

    # feature loop
    - title: "Manajemen tanda tangan"
      content: "Setelah menandatangani, dokumen dapat diproses lebih lanjut. Ambil daftar semua tanda tangan yang ada, modifikasi, atau hapus sesuai kebutuhan."

    # feature loop
    - title: "Kontrol konten yang canggih"
      content: "Lindungi dokumen bisnis dari perubahan yang tidak sah dengan sertifikat digital perusahaan. Tambahkan atau ekstrak entri metadata tersembunyi yang tersedia di semua jenis dokumen."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cara menambahkan tanda tangan gambar ke dokumen"
      content: |
        Contoh ini menunjukkan cara menempatkan tanda tangan gambar pada halaman tertentu dari dokumen.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Berikan dokumen sumber sebagai parameter
          Signature signature = new Signature("input.pdf");

          // Tentukan jalur gambar dalam opsi tanda tangan
          ImageSignOptions options = new ImageSignOptions("image.jpg");

          // Atur ukuran dan halaman target untuk tanda tangan
          options.setVerticalAlignment(VerticalAlignment.Bottom);
          options.setHorizontalAlignment(HorizontalAlignment.Right);
          options.setHeight(150);
          options.setWidth(200);
          Padding padding = new Padding(50);
          options.setMargin(padding);
          options.setAllPages(true);

          // Terapkan tanda tangan ke dokumen
          signature.sign("output.pdf", options);

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
            link: "/examples/signature/formats/signature_esign.pdf"
        links:
          #  loop
          - title: "Lebih banyak contoh"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
          #  loop
          - title: "Dokumentasi"
            link: "https://docs.groupdocs.com/signature/java/"
            

            


############################## Actions ############################

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
    title: "Jelajahi fitur kunci kami"
    exclude: "esign"
    description: "Kami bangga menawarkan berbagai tanda tangan dan operasi yang didukung."
    items: 
          
        # operation loop 1
        - name: "Tanda Tangan Elektronik"
          operation: "esign"
          link: "/signature/java/esign/pdf/"
          description: "Tambahkan berbagai jenis tanda tangan ke format file yang didukung"

        # operation loop 2
        - name: "Tambahkan teks ke dokumen"
          operation: "text"
          link: "/signature/java/text/pdf/"
          description: "Tingkatkan konten dokumen dengan tanda tangan teks yang dapat disesuaikan"

        # operation loop 3
        - name: "Tanda Tangan Gambar"
          operation: "image"
          link: "/signature/java/image/pdf/"
          description: "Tempatkan gambar di posisi mana pun dalam dokumen"

        # operation loop 4
        - name: "Hasilkan barcode"
          operation: "barcode"
          link: "/signature/java/barcode/pdf/"
          description: "Buat dan sisipkan berbagai barcode ke dalam dokumen yang didukung"

        # operation loop 5
        - name: "Hasilkan QR code"
          operation: "qrcode"
          link: "/signature/java/qrcode/pdf/"
          description: "Buat dan QR Code, termasuk QR code, untuk penandatanganan dokumen"
          
        # operation loop 6
        - name: "Sertifikat Digital"
          operation: "digital"
          link: "/signature/java/digital/pdf/"
          description: "Amankan bisnis dan tanda tangani dokumen dengan sertifikat digital"

        # operation loop 7
        - name: "Tanda Tangan Stempel"
          operation: "stamp"
          link: "/signature/java/stamp/pdf/"
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
    title: "Tandai format berkas populer dengan tanda tangan elektronik"
    exclude: "PDF"
    description: "API tanda tangan elektronik untuk Java memungkinkan pemrosesan semua format berkas dan dokumen bisnis modern."
    items: 
          
        # format loop 1
        - name: "Tanda Tangan Elektronik PDF"
          format: "PDF"
          link: "/signature/java/esign/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Tanda Tangan Elektronik DOCX"
          format: "DOCX"
          link: "/signature/java/esign/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Tanda Tangan Elektronik JPEG"
          format: "JPEG"
          link: "/signature/java/esign/jpeg/"
          description: "Gambar JPEG"
          
        # format loop 4
        - name: "Tanda Tangan Elektronik PPTX"
          format: "PPTX"
          link: "/signature/java/esign/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 5
        - name: "Tanda Tangan Elektronik XLSX"
          format: "XLSX"
          link: "/signature/java/esign/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---