



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:14
draft: false
lang: id
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Verifikasi tanda tangan elektronik DOCX menggunakan Java"
head_description: "GroupDocs.Signature for Java memungkinkan verifikasi tanda tangan yang diletakkan dalam file DOCX. Validasi tanda tangan dalam PDF, dokumen Word, lembar Excel, Presentasi, Gambar, atau arsip ZIP."

############################# Header ############################
title: "Verifikasi e-Signature untuk DOCX" 
description: "Verifikasi semua tanda tangan elektronik yang didukung dalam file PDF, Word, Excel, Presentasi, Gambar, atau ZIP dengan GroupDocs.Signature for Java."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Unduh versi gratis"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "Aplikasi GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) mendukung operasi CRUD lengkap untuk penandatanganan dokumen dan lebih banyak lagi. Tandatangani lebih dari 60 format dokumen, termasuk PDF, file MS Office, Gambar, dan arsip ZIP, dengan teks, gambar, kode batang, sertifikat digital, metadata, dan cap. Operasi tambahan seperti mencari, memverifikasi, memodifikasi, atau menghapus tanda tangan juga tersedia.

############################# Steps ############################
steps:
    enable: true
    title: "Langkah-langkah untuk memverifikasi tanda tangan dalam DOCX menggunakan Java"
    content: |
      [GroupDocs.Signature](/signature/java/) dapat memverifikasi keberadaan tanda tangan tertentu dalam dokumen DOCX. Pengembang Java dapat meningkatkan aplikasi mereka dengan menambahkan fitur yang disediakan oleh solusi kami.
      
      1. Muat file DOCX ke dalam instansi Signature.
      2. Instansiasi dan konfigurasi VerifyOptions untuk mencapai hasil yang diinginkan.
      3. Inisiasi proses verifikasi.
      4. Tinjau hasil verifikasi.
   
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
        // Instansiasi Signature dengan dokumen
        Signature signature = new Signature("input.docx");

        // Buat TextVerifyOptions untuk memverifikasi tanda tangan yang mengandung teks tertentu
        TextVerifyOptions options = new TextVerifyOptions();
        options.setText("signature");
        options.setMatchType(TextMatchType.Contains);

        // Verifikasi tanda tangan dalam dokumen
        VerificationResult result = signature.verify(options);

        // Proses hasil verifikasi
        if (result.isValid())
        {
            System.out.print("\nDocument was verified successfully!");
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Solusi penandatanganan dokumen yang komprehensif"
  description: "GroupDocs.Signature meningkatkan format dokumen kantor populer dengan 7 jenis tanda tangan dan operasi CRUD lengkap, menawarkan perlindungan yang kuat untuk konten dokumen Anda."
  image: "/img/signature/features_verify.webp" # 500x500 px
  image_description: "Verifikasi tanda tangan"
  features:
    # feature loop
    - title: "Tandatangani dokumen korporat"
      content: "Tambahkan tanda tangan digital profesional ke dokumen manapun. Solusi kami mendukung berbagai jenis tanda tangan, termasuk teks, gambar, kode batang, metadata, cap, dan sertifikat digital."

    # feature loop
    - title: "Operasi CRUD tanda tangan"
      content: "Dalam banyak kasus, dokumen yang telah ditandatangani memerlukan pemrosesan lebih lanjut. Ambil daftar semua tanda tangan dalam dokumen, verifikasi, modifikasi propertinya, atau hapus saat diperlukan."

    # feature loop
    - title: "Lindungi konten dokumen"
      content: "Lindungi dokumen korporat dengan sertifikat digital untuk mencegah perubahan yang tidak sah. Sisipkan metadata tersembunyi untuk melindungi lebih jauh konten dokumen."

    # feature loop
    - title: "Tanda tangan asli"
      content: "Gunakan tanda tangan teks yang spesifik untuk dokumen, seperti cap PDF atau watermark Word, untuk membuat dokumen yang disesuaikan dan profesional untuk penggunaan korporat."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Verifikasi tanda tangan kode batang"
      content: |
        Contoh ini menunjukkan cara untuk memverifikasi tanda tangan kode batang dalam dokumen.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Sediakan dokumen yang berisi tanda tangan kode batang
          final Signature signature = new Signature("input.docx");

          // Konfigurasi opsi untuk memverifikasi kode batang terhadap teks tertentu
          BarcodeVerifyOptions options = new BarcodeVerifyOptions();
          options.setText("12345");
          options.setMatchType(TextMatchType.StartsWith);

          // Verifikasi tanda tangan yang diterapkan pada dokumen
          VerificationResult result = signature.verify(options);

          // Tampilkan hasil verifikasi
          if (result.isValid())
          {
              System.out.print("\nDocument was verified successfully!");
          }
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
    title: "Operasi dan tipe tanda tangan yang didukung"
    exclude: "verify"
    description: "Jelajahi berbagai fitur dan operasi tanda tangan yang didukung oleh GroupDocs.Signature."
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
          
############################# More Formats #####################
more_formats:
    enable: true
    title: "Verifikasi tanda tangan di berbagai format file"
    exclude: "DOCX"
    description: "GroupDocs.Signature for Java menyederhanakan proses verifikasi semua tanda tangan dalam dokumen. Atur parameter verifikasi kustom untuk memastikan integritas dokumen yang ditandatangani."
    items: 
          
        # format loop 1
        - name: "Verifikasi tanda tangan PDF"
          format: "PDF"
          link: "/signature/java/verify/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Verifikasi tanda tangan DOCX"
          format: "DOCX"
          link: "/signature/java/verify/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Verifikasi tanda tangan PPTX"
          format: "PPTX"
          link: "/signature/java/verify/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 4
        - name: "Validasi tanda tangan XLSX"
          format: "XLSX"
          link: "/signature/java/verify/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---