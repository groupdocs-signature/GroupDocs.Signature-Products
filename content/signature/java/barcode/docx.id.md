



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:05
draft: false
lang: id
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Tambahkan kode batang ke file DOCX dengan Java"
head_description: "Buat dan masukkan tanda tangan kode batang ke dokumen DOCX dalam Java. GroupDocs.Signature memungkinkan integrasi tanda tangan yang beragam untuk berbagai format."

############################# Header ############################
title: "Hasilkan kode batang untuk DOCX" 
description: "Tambahkan kode batang dari format populer ke posisi mana pun dalam dokumen bisnis Anda dengan GroupDocs.Signature for Java. Solusi kami menyediakan berbagai opsi untuk menyesuaikan tanda tangan kode batang."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Unduh Gratis"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "Tentang GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) adalah solusi tanda tangan lanjutan yang mendukung berbagai jenis tanda tangan. Anda dapat menandatangani dokumen dengan teks, gambar, kode batang, sertifikat digital, cap, dan lainnya dalam lebih dari 60 format file, termasuk PDF, MS Office, gambar, file ZIP, dan format bisnis populer lainnya. Selain itu, tanda tangan dalam dokumen yang ditandatangani dapat dicari, diverifikasi, dimodifikasi, atau dihapus kapan saja.

############################# Steps ############################
steps:
    enable: true
    title: "Langkah untuk menghasilkan dan menambahkan kode batang ke file DOCX"
    content: |
      [GroupDocs.Signature](/signature/java/) dapat menghasilkan kode batang dalam berbagai format populer dan menempatkannya di halaman DOCX. Dengan dukungan untuk lebih dari 60 jenis kode batang, aplikasi Java dapat dengan mudah ditingkatkan dengan kemampuan tanda tangan kode batang dengan mengintegrasikan pustaka kami.
      
      1. Sediakan file DOCX atau aliran untuk diproses.
      2. Serahkan teks kode batang ke instansi BarcodeSignOptions.
      3. Sesuaikan opsi kode batang seperti posisi, ukuran, dll.
      4. Simpan file dengan kode batang yang baru ditambahkan.
   
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
        // Buat instansi Signature baru dengan jalur dokumen
        Signature signature = new Signature("input.docx");

        // Gunakan BarcodeSignOptions untuk menambahkan kode batang ke dokumen
        BarcodeSignOptions options = new BarcodeSignOptions("Business data");

        // Siapkan jenis kode batang dan properti lainnya
        options.setEncodeType(BarcodeTypes.Code128);
        options.setLeft(100);
        options.setTop(100);

        // Simpan file yang ditandatangani
        signature.sign("output.docx", options);

        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Tingkatkan atau lindungi konten dokumen dengan tanda tangan"
  description: "Pustaka GroupDocs.Signature for Java dirancang untuk menandatangani dan memproses lebih lanjut format file populer. Tambahkan, ubah, verifikasi, atau hapus berbagai jenis tanda tangan dengan cepat dan efisien."
  image: "/img/signature/features_barcode.webp" # 500x500 px
  image_description: "Fitur dari GroupDocs.Signature"
  features:
    # feature loop
    - title: "Penandatanganan dokumen"
      content: "Tandatangani halaman mana pun dari dokumen yang didukung dengan teks, gambar, kode batang, kode QR, atau cap. Tambahkan metadata tersembunyi seperti EXIF dalam gambar atau lindungi konten dokumen dari perubahan yang tidak sah menggunakan sertifikat digital."

    # feature loop
    - title: "Pencarian dan verifikasi tanda tangan"
      content: "Ada banyak hal yang dapat Anda lakukan dengan dokumen yang ditandatangani. Kami menawarkan verifikasi tanda tangan untuk memastikan semuanya dalam keadaan baik. Selain itu, Anda dapat mengambil daftar semua tanda tangan dokumen melalui pencarian."

    # feature loop
    - title: "Modifikasi tanda tangan"
      content: "Sebagian besar tanda tangan yang ditambahkan sebelumnya dapat dimodifikasi. Sesuaikan teks, ubah posisi, atau ubah warna dengan mudah."

    # feature loop
    - title: "Hapus tanda tangan"
      content: "Solusi kami mendukung operasi CRUD penuh untuk tanda tangan. Banyak jenis tanda tangan dapat dihapus dari dokumen jika diperlukan."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cara membuat tanda tangan kode batang"
      content: |
        Contoh ini menunjukkan cara menempatkan kode batang yang disesuaikan pada halaman dokumen DOCX.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Sediakan dokumen yang akan ditandatangani
          Signature signature = new Signature("input.docx");

          // Buat opsi tanda tangan dengan teks yang diinginkan
          BarcodeSignOptions signOptions = new BarcodeSignOptions("Accepted");
          signOptions.setEncodeType(BarcodeTypes.Code39FullASCII);

          // Atur posisi kode batang relatif pada halaman
          signOptions.setVerticalAlignment(VerticalAlignment.Bottom);
          signOptions.setHorizontalAlignment(HorizontalAlignment.Left);

          // Atur padding kode batang dari tepi halaman
          Padding padding = new Padding();
          padding.setLeft(20);
          padding.setTop(180);
          signOptions.setMargin(padding);

          // Atur warna batang
          signOptions.setForeColor(Color.RED);

          // Tentukan gaya font pesan
          SignatureFont font = new SignatureFont();
          font.setSize(12);
          font.setFamilyName("Arial");
          signOptions.setFont(font);

          // Tentukan posisi pesan
          signOptions.setCodeTextAlignment(CodeTextAlignment.Above);

          // Tandatangani dan simpan dokumen
          SignResult signResult = signature.sign("output.docx", signOptions);

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
            link: "/examples/signature/formats/signature_barcode.docx"
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
    title: "Temukan kemampuan inti kami"
    exclude: "barcode"
    description: "Kami bangga mempersembahkan berbagai jenis tanda tangan dan fungsi yang didukung."
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
    title: "Tandatangani dokumen dalam format lainnya"
    exclude: "DOCX"
    description: "Lebih dari 60 format dapat ditandatangani menggunakan API Java kami. Terapkan berbagai tanda tangan pada halaman atau posisi mana pun dalam dokumen."
    items: 
          
        # format loop 1
        - name: "Tambahkan barcode ke PDF"
          format: "PDF"
          link: "/signature/java/barcode/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Tambahkan barcode ke DOCX"
          format: "DOCX"
          link: "/signature/java/barcode/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Tambahkan barcode ke JPEG"
          format: "JPEG"
          link: "/signature/java/barcode/jpeg/"
          description: "Gambar JPEG"
          
        # format loop 4
        - name: "Tambahkan barcode ke PPTX"
          format: "PPTX"
          link: "/signature/java/barcode/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 5
        - name: "Tambahkan barcode ke XLSX"
          format: "XLSX"
          link: "/signature/java/barcode/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---