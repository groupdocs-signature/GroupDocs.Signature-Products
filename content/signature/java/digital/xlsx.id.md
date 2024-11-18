



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:57
draft: false
lang: id
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Menambahkan tanda tangan elektronik digital ke file XLSX dengan Java"
head_description: "Letakkan tanda tangan digital di file XLSX menggunakan Java dengan hanya beberapa baris kode. Gunakan GroupDocs.Signature for Java untuk menandatangani berbagai format file."

############################# Header ############################
title: "Tandatangani XLSX dengan tanda tangan digital" 
description: "Lindungi konten dokumen bisnis Anda dengan menyegel mereka menggunakan sertifikat digital menggunakan fitur dari GroupDocs.Signature for Java. Kami menyediakan berbagai cara untuk menandai dan mengamankan dokumen Anda."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Unduh secara gratis"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "Tentang GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) adalah solusi penandatanganan komprehensif yang mendukung berbagai jenis pemrosesan dokumen. Anda dapat menambahkan teks, gambar, sertifikat digital, dan cap ke file dalam lebih dari 60 format, termasuk PDF, MS Office, gambar, file ZIP, dan format bisnis populer lainnya. Selain itu, dokumen yang ditandatangani dapat dicari, diverifikasi, dimodifikasi, atau dihapus secara otomatis dengan cara yang nyaman.

############################# Steps ############################
steps:
    enable: true
    title: "Langkah-langkah untuk melindungi XLSX dengan sertifikat digital di Java"
    content: |
      [GroupDocs.Signature](/signature/java/) memungkinkan pengembang Java untuk mencegah perubahan pada dokumen XLSX menggunakan tanda tangan digital. Perkuat aplikasi bisnis Anda dengan kemampuan untuk mengamankan data penting.
      
      1. Berikan dokumen XLSX ke konstruktor kelas Signature.
      2. Gunakan sertifikat digital dan kata sandinya untuk melindungi dokumen.
      3. Opsional, tambahkan representasi visual dari tanda tangan digital di halaman dokumen.
      4. Tandatangani dokumen untuk mencegah perubahan di masa mendatang.
   
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
        // Gunakan Signature dengan dokumen untuk tanda tangan digital
        Signature signature = new Signature("input.xlsx");

        // Sediakan sertifikat digital dan kata sandi
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");
        options.setPassword("1234567890");

        // Atur representasi visual jika diperlukan
        options.setPageNumber(1);
        options.setLeft(100);
        options.setTop(100);

        // Lindungi dokumen dengan sertifikat digital
        SignResult result = signature.sign("output.xlsx", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Tingkatkan atau lindungi konten dokumen dengan tanda tangan"
  description: "Perpustakaan GroupDocs.Signature for Java mampu menandatangani semua format file populer. Tambahkan, ubah, verifikasi, atau hapus berbagai jenis tanda tangan secara otomatis untuk memperlancar proses bisnis Anda."
  image: "/img/signature/features_digital.webp" # 500x500 px
  image_description: "Fitur-fitur dari GroupDocs.Signature"
  features:
    # feature loop
    - title: "Tambahkan tanda tangan ke dokumen"
      content: "Tanda tangan Teks, Gambar, Barcode, QR-Code, atau Cap dapat ditambahkan dengan tepat ke halaman mana pun dari dokumen yang didukung. Metadata tersembunyi seperti EXIF dapat ditambahkan atau diedit dalam gambar dan sebagian besar jenis file. Lindungi konten dokumen dari perubahan yang tidak sah menggunakan tanda tangan digital."

    # feature loop
    - title: "Pencarian dan verifikasi tanda tangan"
      content: "Dokumen dapat diproses dengan berbagai cara setelah ditandatangani. Verifikasi dokumen yang ditandatangani untuk memastikan bahwa mereka telah diproses dengan benar. Jika Anda memerlukan kontrol lebih, ambil daftar semua tanda tangan melalui pencarian."

    # feature loop
    - title: "Edit tanda tangan"
      content: "Sebagian besar jenis tanda tangan mendukung modifikasi lebih lanjut. Anda bebas untuk memperbaiki teks, mengubah posisi, warna, ukuran, dan lainnya."

    # feature loop
    - title: "Hapus tanda tangan yang tidak perlu"
      content: "Solusi kami mendukung operasi CRUD penuh untuk tanda tangan. Banyak jenis tanda tangan, termasuk sertifikat digital, dapat dihapus dari dokumen jika diperlukan."
      
  code_samples:
    # code sample loop
    - title: "Lindungi dokumen dengan tanda tangan digital"
      content: |
        Pelajari cara mengamankan dokumen dari perubahan menggunakan tanda tangan digital.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        // Sediakan dokumen untuk ditandatangani
        Signature signature = new Signature("input.xlsx");

        // Gunakan sertifikat digital yang valid dengan kata sandi
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");
        options.setPassword("1234567890");

        // Tentukan data teks tambahan
        options.setReason("Security issue");
        options.setContact("John Smith");
        options.setLocation("Office D.W.");

        // Gunakan gambar dan opsi lain untuk representasi visual
        options.setImageFilePath("image.png");

        options.setAllPages(true);
        options.setVerticalAlignment(VerticalAlignment.Bottom);
        options.setHorizontalAlignment(HorizontalAlignment.Right);
        options.setWidth(80);
        options.setHeight(60);

        Padding padding = new Padding();
        padding.setBottom(10);
        padding.setRight(10);
        options.setMargin(padding);

        // Simpan dokumen yang dilindungi ke lokasi yang berbeda
        SignResult result = signature.sign("output.xlsx", options);
        ```
        {{< /landing/code >}}


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
    title: "Periksa set fitur komprehensif kami"
    exclude: "digital"
    description: "Kami bangga dengan fungsionalitas luas dan dukungan tanda tangan yang ditawarkan oleh platform kami."
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
    title: "Tandatangani dokumen dalam format lainnya"
    exclude: "XLSX"
    description: "API Java memungkinkan Anda untuk memproses lebih dari 60 format. Buat dan tambahkan berbagai tanda tangan ke halaman mana pun, segel konten dengan sertifikat digital, dan kelola serta edit tanda tangan yang sudah ada dalam dokumen."
    items: 
          
        # format loop 1
        - name: "Lindungi PDF"
          format: "PDF"
          link: "/signature/java/digital/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Lindungi DOCX"
          format: "DOCX"
          link: "/signature/java/digital/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Lindungi PPTX"
          format: "PPTX"
          link: "/signature/java/digital/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 4
        - name: "Lindungi XLSX"
          format: "XLSX"
          link: "/signature/java/digital/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---