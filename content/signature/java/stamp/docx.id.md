



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:46
draft: false
lang: id
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Tambahkan stempel ke DOCX menggunakan Java"
head_description: "Manfaatkan GroupDocs.Signature dan Java untuk membuat stempel kustom dan menempatkannya di halaman mana saja dalam dokumen DOCX."

############################# Header ############################
title: "Tambahkan stempel kustom ke DOCX" 
description: "Rancang dan terapkan stempel bulat atau persegi ke bagian mana pun dari dokumen Anda menggunakan GroupDocs.Signature for Java. Solusi kami menawarkan opsi kustomisasi yang luas untuk memenuhi semua kebutuhan bisnis Anda."
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
    title: "Tentang GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) adalah alat yang kuat yang memungkinkan Anda menambahkan berbagai tanda tangan stempel ke dokumen. Ini mendukung lebih dari 60 format file yang berbeda, termasuk PDF, Word, Excel, gambar, dan file ZIP. Anda dapat menerapkan teks, gambar, kode batang, metadata, sertifikat digital, dan tanda tangan stempel. Selain menambahkan tanda tangan, Anda dapat mencari, memverifikasi, memodifikasi, dan menghapusnya.

############################# Steps ############################
steps:
    enable: true
    title: "Langkah untuk menambahkan stempel ke DOCX menggunakan Java"
    content: |
      [GroupDocs.Signature](/signature/java/) menyediakan konstruktor stempel yang sangat bermanfaat untuk aplikasi Java. Manfaatkan untuk membuat stempel yang sangat disesuaikan untuk halaman dokumen Anda.
      
      1. Berikan dokumen DOCX yang akan distempel.
      2. Gunakan StampSignOptions untuk mengonfigurasi semua parameter yang diperlukan.
      3. Tambahkan sebanyak mungkin garis yang diperlukan.
      4. Terapkan stempel dan simpan dokumen.
   
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
        // Gunakan jalur dokumen dengan objek Signature
        Signature signature = new Signature("input.docx");

        // Instansikan StampSignOptions dengan teks tanda tangan yang diinginkan
        StampSignOptions options = new StampSignOptions();
        options.Height = 180;
        options.Width = 180;

        // Tambahkan satu atau lebih garis stempel
        StampLine outerLine = new StampLine();
        outerLine.setText("* The Best Company *");
        outerLine.setTextRepeatType(StampTextRepeatType.FullTextRepeat);
        outerLine.getFont().setSize(12);
        outerLine.setHeight(22);
        outerLine.setTextBottomIntent(6);
        outerLine.setTextColor(Color.WHITE);
        outerLine.setBackgroundColor(Color.BLUE);
        options.getOuterLines().add(outerLine);

        // Simpan dokumen yang telah distempel
        SignResult result = signature.sign("output.docx", options);
        ```        

############################# More features ############################
more_features:
  enable: true
  title: "Lindungi konten dokumen Anda dengan tanda tangan"
  description: "Perpustakaan GroupDocs.Signature for Java dirancang untuk menandatangani dan mengelola tanda tangan di berbagai format file populer. Tambahkan, modifikasi, verifikasi, atau hapus stempel dan jenis tanda tangan lainnya dengan mudah."
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "Tanda Tangan Stempel dengan GroupDocs.Signature"
  features:
    # feature loop
    - title: "Tanda tangani dokumen Anda"
      content: "Terapkan tanda tangan yang dapat disesuaikan ke bagian mana saja dari dokumen Anda. Pilih dari berbagai jenis tanda tangan, termasuk teks, gambar, kode batang, kode QR, dan stempel. Selain itu, metadata yang tersembunyi dapat ditambahkan atau dimodifikasi untuk meningkatkan keamanan dokumen."

    # feature loop
    - title: "Cari dan validasi tanda tangan"
      content: "Setelah dokumen ditandatangani, gunakan alat verifikasi kami untuk memastikan bahwa konten tanda tangan valid. Cari dan ambil daftar semua tanda tangan untuk pemrosesan lebih lanjut."

    # feature loop
    - title: "Perbarui tanda tangan sesuai kebutuhan"
      content: "Modifikasi berbagai tanda tangan yang diterapkan pada dokumen dengan mudah. Perbarui properti seperti ukuran, warna, posisi, konten, dan banyak lagi."

    # feature loop
    - title: "Hapus tanda tangan"
      content: "Perlu menghapus tanda tangan dari dokumen? API kami sepenuhnya mendukung penghapusan tanda tangan, sehingga Anda dapat mengelola dokumen Anda dengan efektif."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Tambahkan stempel kustom ke dokumen menggunakan tanda tangan khusus"
      content: |
        Pelajari cara menghasilkan dan menambahkan stempel kustom dengan informasi teks penting ke dokumen Anda.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Berikan dokumen yang akan distempel
          Signature signature = new Signature("input.docx");

          // Instansikan objek opsi stempel
          StampSignOptions options = new StampSignOptions();

          // Tetapkan ukuran dan posisi di halaman
          options.setHeight(200);
          options.setWidth(200);
          options.setVerticalAlignment(VerticalAlignment.Bottom);
          options.setHorizontalAlignment(HorizontalAlignment.Right);
          options.setAllPages(true);

          // Tambahkan satu atau lebih garis luar bulat dengan teks
          StampLine outerLine1 = new StampLine();
          outerLine1.setText("* The best  choice *");
          outerLine1.setTextRepeatType(StampTextRepeatType.FullTextRepeat);
          SignatureFont signatureFont1 = new SignatureFont();
          signatureFont1.setSize(12);
          signatureFont1.setFamilyName("Arial");
          outerLine1.setFont(signatureFont1);
          outerLine1.setHeight(30);
          outerLine1.setTextBottomIntent(6);
          outerLine1.setTextColor(Color.WHITE);
          outerLine1.setBackgroundColor(Color.BLUE);
          options.getOuterLines().add(outerLine1);

          // Tambahkan satu atau lebih garis dalam kotak
          StampLine innerLine1 = new StampLine();
          innerLine1.setText("Company #1");
          innerLine1.setTextColor(Color.RED);
          SignatureFont signFont1 = new SignatureFont();
          signFont1.setSize(20);
          signFont1.setBold(true);
          innerLine1.setFont(signFont1);
          innerLine1.setHeight(40);
          options.getInnerLines().add(innerLine1);

          // Simpan dokumen yang telah distempel
          SignResult result = signature.sign("output.docx", options);
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
            link: "/examples/signature/formats/signature_stamp.docx"
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
    title: "Jelajahi fitur inti kami"
    exclude: "stamp"
    description: "Manfaatkan berbagai opsi untuk menambahkan, mengelola, dan menghapus tanda tangan."
    items: 
          
        # operation loop 1
        - name: "Tanda Tangan Elektronik"
          operation: "esign"
          link: "/signature/java/esign/docx/"
          description: "Tambahkan berbagai jenis tanda tangan ke format file yang didukung"

        # operation loop 2
        - name: "Tambahkan teks ke dokumen"
          operation: "text"
          link: "/signature/java/text/docx/"
          description: "Tingkatkan konten dokumen dengan tanda tangan teks yang dapat disesuaikan"

        # operation loop 3
        - name: "Tanda Tangan Gambar"
          operation: "image"
          link: "/signature/java/image/docx/"
          description: "Tempatkan gambar di posisi mana pun dalam dokumen"

        # operation loop 4
        - name: "Hasilkan barcode"
          operation: "barcode"
          link: "/signature/java/barcode/docx/"
          description: "Buat dan sisipkan berbagai barcode ke dalam dokumen yang didukung"

        # operation loop 5
        - name: "Hasilkan QR code"
          operation: "qrcode"
          link: "/signature/java/qrcode/docx/"
          description: "Buat dan QR Code, termasuk QR code, untuk penandatanganan dokumen"
          
        # operation loop 6
        - name: "Sertifikat Digital"
          operation: "digital"
          link: "/signature/java/digital/docx/"
          description: "Amankan bisnis dan tanda tangani dokumen dengan sertifikat digital"

        # operation loop 7
        - name: "Tanda Tangan Stempel"
          operation: "stamp"
          link: "/signature/java/stamp/docx/"
          description: "Gunakan Konstruksi Stempel untuk membuat stempel bulat atau persegi yang kustom"
          
        # operation loop 8
        - name: "Cari tanda tangan"
          operation: "search"
          link: "/signature/java/search/docx/"
          description: "Temukan tanda tangan yang ditambahkan sebelumnya dalam dokumen"
          
        # operation loop 9
        - name: "Verifikasi tanda tangan"
          operation: "verify"
          link: "/signature/java/verify/docx/"
          description: "Verifikasi keaslian tanda tangan setelah diterapkan"
          
        # operation loop 10
        - name: "Modifikasi tanda tangan"
          operation: "modify"
          link: "/signature/java/modify/docx/"
          description: "Edit berbagai tanda tangan dalam dokumen"
          
        # operation loop 11
        - name: "Hapus tanda tangan"
          operation: "delete"
          link: "/signature/java/delete/docx/"
          description: "Hapus berbagai tanda tangan yang diterapkan sebelumnya"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Tambahkan stempel di berbagai format file"
    exclude: "DOCX"
    description: "API GroupDocs.Signature mendukung penempelan dokumen dalam lebih dari 60 format. Tempatkan stempel di halaman atau area mana saja untuk meningkatkan pengelolaan dan kustomisasi dokumen."
    items: 
          
        # format loop 1
        - name: "Stempel PDF"
          format: "PDF"
          link: "/signature/java/stamp/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Stempel DOCX"
          format: "DOCX"
          link: "/signature/java/stamp/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Stempel JPEG"
          format: "JPEG"
          link: "/signature/java/stamp/jpeg/"
          description: "Gambar JPEG"
          
        # format loop 4
        - name: "Stempel PPTX"
          format: "PPTX"
          link: "/signature/java/stamp/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 5
        - name: "Stempel XLSX"
          format: "XLSX"
          link: "/signature/java/stamp/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---