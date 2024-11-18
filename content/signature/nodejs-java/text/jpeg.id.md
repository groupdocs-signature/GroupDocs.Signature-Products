



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:56
draft: false
lang: id
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Tambahkan tanda tangan teks ke JPEG melalui JavaScript"
head_description: "Manfaatkan API JavaScript untuk mengintegrasikan tanda tangan teks ke dalam dokumen JPEG secara mulus. API kami mendukung berbagai format, termasuk PDF, Word, Excel, Presentasi, Gambar, dan file ZIP."

############################# Header ############################
title: "Tambahkan tanda tangan teks ke JPEG" 
description: "Gabungkan tanda tangan teks yang dipersonalisasi ke dalam file bisnis Anda dengan GroupDocs.Signature for Node.js via Java. Kendalikan alur kerja dokumen Anda dengan meningkatkan keamanan dan opsi tanda tangan yang dapat disesuaikan."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Mulai uji coba gratis"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Memperkenalkan GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) adalah solusi inovatif yang dirancang untuk memudahkan penambahan tanda tangan teks ke dokumen. Sesuaikan dan tempatkan tanda tangan di halaman mana saja, meningkatkan efisiensi dalam penanganan dokumen. Permudah alur kerja organisasi Anda dengan mengintegrasikan tanda tulisan teks yang dipersonalisasi yang meningkatkan fungsi dan profesionalisme.

############################# Steps ############################
steps:
    enable: true
    title: "Panduan untuk membuat tanda tangan teks untuk JPEG menggunakan JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) memungkinkan penambahan tanda tangan teks ke dokumen JPEG dalam aplikasi Node.js via Java. Segera tingkatkan kemampuan produk Anda dengan solusi robust kami.
      
      1. Berikan dokumen JPEG sebagai argumen untuk kelas Signature.
      2. Instansikan TextSignOptions dengan teks yang diperlukan.
      3. Tetapkan properti visual dari tanda tangan teks.
      4. Tambahkan tanda tangan teks ke halaman yang diinginkan dari dokumen.
   
    code:
      platform: "nodejs-java"
      copy_title: "Salin"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Contoh tanda tangan"
      install:
        command: "npm i @groupdocs/groupdocs.signature"
        copy_tip: "klik untuk menyalin"
        copy_done: "disalin"
      links:
        #  loop
        - title: "Lebih banyak contoh"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
        #  loop
        - title: "Dokumentasi"
          link: "https://docs.groupdocs.com/signature/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')

        // Inisialisasi kelas Signature dengan jalur dokumen
        const signature = new signatureLib.Signature('input.jpeg');

        // Buat TextSignOptions dengan teks tanda tangan yang diperlukan
        const options = new signatureLib.TextSignOptions('Approved');

        // Tetapkan warna teks dan properti font
        options.setForeColor(new signatureLib.Color(255, 0, 0));
        const signatureFont = new signatureLib.SignatureFont();
        signatureFont.setSize(12);
        signatureFont.setFamilyName('Comic Sans MS');
        options.setFont(signatureFont);
        
        // Tambahkan tanda tangan teks ke dokumen
        const result = signature.sign('output.jpeg', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Kontrol tanda tangan teks yang ditingkatkan"
  description: "Dengan GroupDocs.Signature for Node.js via Java, Anda dapat sangat meningkatkan pengelolaan tanda tangan berbasis teks dalam format dokumen kunci. Alat ini memungkinkan Anda mengkonfigurasi gaya, penempatan, dan konten tanda tangan dengan sangat baik, memungkinkan bisnis menyesuaikan proses dokumen mereka."
  image: "/img/signature/features_text.webp" # 500x500 px
  image_description: "Fitur utama GroupDocs.Signature"
  features:
    # feature loop
    - title: "Tanda tangan dokumen dinamis"
      content: "Sisipkan berbagai jenis tanda tangan—seperti teks, gambar, barcode, kode QR, atau cap—di halaman mana pun dari dokumen yang didukung. Sisipkan metadata untuk menyimpan informasi tersembunyi atau terapkan sertifikat digital untuk langkah-langkah keamanan lanjutan."

    # feature loop
    - title: "Pencarian dan validasi tanda tangan"
      content: "Verifikasi keaslian tanda tangan yang tertanam dalam dokumen Anda. Lakukan pencarian yang efisien untuk menemukan semua instance tanda tangan, memastikan pelacakan dan pengelolaan dokumen yang menyeluruh."

    # feature loop
    - title: "Edit atau hapus tanda tangan"
      content: "Ubah atau hapus tanda tangan yang telah ditambahkan sebelumnya sesuai kebutuhan. Anda dapat menyesuaikan penampilan, posisi, atau konten tanda tangan mana pun untuk memenuhi kebutuhan yang terus berkembang, memastikan fleksibilitas dalam penanganan dokumen."

    # feature loop
    - title: "Kustomisasi tanda tangan asli"
      content: "Untuk jenis file tertentu, sesuaikan penempatan tanda tangan dengan fitur dokumen bawaan, seperti menambahkan watermark ke file Word atau cap yang disesuaikan ke PDF, meningkatkan uniknya dokumen Anda."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Terapkan tanda tangan teks dalam dokumen"
      content: |
        Pelajari cara menyisipkan tanda tangan teks ke dalam dokumen bisnis untuk mengoptimalkan proses.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // Pilih dokumen yang akan ditandatangani
          const signature = new signatureLib.Signature('input.jpeg');

          // Tentukan opsi teks dengan konten yang ditentukan
          const options = new signatureLib.TextSignOptions('Rescheduled to 03/04/2025');

          // Tetapkan ukuran dan posisi tanda tangan di halaman
          options.setLeft(100);
          options.setTop(180);
          options.setWidth(230);
          options.setHeight(30);

          // Terapkan padding untuk tanda tangan dari tepi halaman
          const padding = new signatureLib.Padding();
          padding.setBottom(20);
          padding.setRight(20);
          options.setMargin(padding);

          // Sesuaikan warna teks dan gaya font
          options.setForeColor(signatureLib.Color.RED);
          const signatureFont = new signatureLib.SignatureFont();
          signatureFont.setSize(12);
          signatureFont.setFamilyName('Comic Sans MS');
          options.setFont(signatureFont);

          // Tambahkan garis batas pada tanda tangan teks jika diinginkan
          const border = new signatureLib.Border();
          border.setColor(signatureLib.Color.RED);
          border.setDashStyle(signatureLib.DashStyle.Dash);
          border.setTransparency(0.5);
          border.setVisible(true);
          border.setWeight(2);
          options.setBorder(border);

          // Konfigurasi latar belakang tanda tangan
          const background = new signatureLib.Background();
          background.setColor(signatureLib.Color.YELLOW);
          background.setTransparency(0.8);
          options.setBackground(background);

          // Jika perlu, simpan teks sebagai gambar untuk kompatibilitas
          options.setSignatureImplementation(signatureLib.TextSignatureImplementation.Image);
          
          // Simpan dokumen dengan tanda tangan teks yang ditambahkan
          const result = signature.sign('output.jpeg', options);
          ```
        platform: "nodejs-java"
        copy_title: "Salin"
        install:
          command: "npm i @groupdocs/groupdocs.signature"
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
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
          #  loop
          - title: "Dokumentasi"
            link: "https://docs.groupdocs.com/signature/nodejs-java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Siap untuk memulai?"
  description: "Coba fitur GroupDocs.Signature secara gratis atau minta lisensi"
  items:
    #  loop
    - title: "Unduhan NPM"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      color: "red"
        #  loop
    - title: "Lisensi"
      link: "https://purchase.groupdocs.com/pricing/signature/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Fitur pengelolaan tanda tangan yang komprehensif"
    exclude: "text"
    description: "Platform kami menawarkan operasi CRUD penuh dan fitur canggih untuk pengelolaan tujuh jenis tanda tangan yang berbeda, memungkinkan Anda mengelola tanda tangan dokumen dengan presisi dan efisiensi."
    items: 
          
        # operation loop 1
        - name: "Tanda Tangan Elektronik"
          operation: "esign"
          link: "/signature/nodejs-java/esign/jpeg/"
          description: "Tambahkan berbagai jenis tanda tangan ke format file yang didukung"

        # operation loop 2
        - name: "Tambahkan teks ke dokumen"
          operation: "text"
          link: "/signature/nodejs-java/text/jpeg/"
          description: "Tingkatkan konten dokumen dengan tanda tangan teks yang dapat disesuaikan"

        # operation loop 3
        - name: "Tanda Tangan Gambar"
          operation: "image"
          link: "/signature/nodejs-java/image/jpeg/"
          description: "Tempatkan gambar di posisi mana pun dalam dokumen"

        # operation loop 4
        - name: "Hasilkan barcode"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/jpeg/"
          description: "Buat dan sisipkan berbagai barcode ke dalam dokumen yang didukung"

        # operation loop 5
        - name: "Hasilkan QR code"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/jpeg/"
          description: "Buat dan QR Code, termasuk QR code, untuk penandatanganan dokumen"
          
        # operation loop 6
        - name: "Sertifikat Digital"
          operation: "digital"
          link: "/signature/nodejs-java/digital/pdf/"
          description: "Amankan bisnis dan tanda tangani dokumen dengan sertifikat digital"

        # operation loop 7
        - name: "Tanda Tangan Stempel"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/jpeg/"
          description: "Gunakan Konstruksi Stempel untuk membuat stempel bulat atau persegi yang kustom"
          
        # operation loop 8
        - name: "Cari tanda tangan"
          operation: "search"
          link: "/signature/nodejs-java/search/pdf/"
          description: "Temukan tanda tangan yang ditambahkan sebelumnya dalam dokumen"
          
        # operation loop 9
        - name: "Verifikasi tanda tangan"
          operation: "verify"
          link: "/signature/nodejs-java/verify/pdf/"
          description: "Verifikasi keaslian tanda tangan setelah diterapkan"
          
        # operation loop 10
        - name: "Modifikasi tanda tangan"
          operation: "modify"
          link: "/signature/nodejs-java/modify/pdf/"
          description: "Edit berbagai tanda tangan dalam dokumen"
          
        # operation loop 11
        - name: "Hapus tanda tangan"
          operation: "delete"
          link: "/signature/nodejs-java/delete/pdf/"
          description: "Hapus berbagai tanda tangan yang diterapkan sebelumnya"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Terapkan tanda tangan teks di berbagai format"
    exclude: "JPEG"
    description: "Manfaatkan kemampuan API Node.js via Java untuk mengintegrasikan tanda tangan berbasis teks ke berbagai format Office. Kendalikan aliran informasi di setiap tahap siklus hidup dokumen Anda dengan menambahkan tanda tulisan teks yang sangat dapat disesuaikan."
    items: 
          
        # format loop 1
        - name: "Tanda Tangan Teks PDF"
          format: "PDF"
          link: "/signature/nodejs-java/text/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Tanda Tangan Teks DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/text/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Tanda Tangan Teks JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/text/jpeg/"
          description: "Gambar JPEG"
          
        # format loop 4
        - name: "Tanda Tangan Teks PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/text/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 5
        - name: "Tanda Tangan Teks XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/text/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---