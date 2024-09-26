---
############################# Static ############################
layout: "family"
date:  2024-09-26T13:44:48
draft: false

product: "Signature"
product_tag: "signature"

lang: id

############################# Head ############################
head_title: "Aplikasi Tanda Tangan Digital C# .NET, Java, Node.js"
head_description: "Integrasikan tanda tangan elektronik di aplikasi .NET, Java, atau Node.js dengan GroupDocs.Signature. Tanda tangani format dokumen bisnis populer."

############################# Header ############################
title: "Solusi Penandatanganan Dokumen secara elektronik"
description:  |
  Tanda tangani dokumen dan gambar digital di platform apa pun menggunakan API fleksibel dan solusi berbasis aplikasi kami untuk pemrogram dan pengguna akhir.

  Cari dan ubah tanda tangan yang ditambahkan sebelumnya menggunakan metode lanjutan.

  Lindungi dokumen dari perubahan dengan sertifikat digital dan kendalikan metadata tersembunyi.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "Pilih platform Anda"
  title: "Independensi platform"
  description: "Pustaka GroupDocs.Signature mendukung sistem operasi dan kerangka kerja berikut:"
  details_link_title: "Belajarlah lagi"

  items:
    # items loop
    - title: ".NET"
      description: GroupDocs.Signature .NET 
      color: "blue"
      tag: "net"
      link: "/signature/net/"
      features_link: "https://docs.groupdocs.com/signature/net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    .NET Framework 4.6.2 or higher <br> .NET Core 3.0 or higher <br> .NET 6.0 or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS <br> Microsoft Azure
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio <br> JetBrains Rider <br> Microsoft Visual Code
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats
      

    # items loop
    - title: "Java"
      description: GroupDocs.Signature Java
      color: "red"
      tag: "java"
      link: "/signature/java/"
      features_link: "https://docs.groupdocs.com/signature/java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Java 8 or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    IntelliJ IDEA <br> Eclipse <br> NetBeans
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats

    # items loop
    - title: "Node.js"
      description: GroupDocs.Signature Node.js
      color: "green"
      tag: "nodejs-java"
      link: "/signature/nodejs-java/"
      features_link: "https://docs.groupdocs.com/signature/nodejs-java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Node.js 16+ and J2SE 8.0 (1.8)+
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Atom <br> Visual Studio Code <br> Editor teks lainnya
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats

    # items loop
    - title: "Python"
      description: GroupDocs.Signature Python
      color: "yellow"
      tag: "python-net"
      link: "/signature/python-net/"
      features_link: "https://docs.groupdocs.com/signature/python-net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Python 3.9+ and .Net 6+
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    IDLE <br> PyCharm <br> Visual Studio Code
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats

############################# Features ###############################
features:
  enable: true
  title: "GroupDocs.Signature fitur utama"
  description: "Solusi kami dirancang untuk menambahkan berbagai jenis tanda tangan ke format dokumen dan file populer. Perkaya proses bisnis Anda dengan mudah."

  items:
    # items loop
    - icon: "additional"
      title: "Perkaya data Anda dengan tanda tangan"
      content: "Tambahkan teks, gambar, tanda air, dll. ke dokumen bisnis Anda."

    # items loop
    - icon: "protect"
      title: "Lindungi konten dokumen"
      content: "Larang perubahan dokumen dengan menyegelnya dengan sertifikat digital."

    # items loop
    - icon: "search"
      title: "Tambahkan data dan kode batang tersembunyi"
      content: "Gunakan metadata untuk menyimpan informasi yang tidak terlihat atau memasang kode batang khusus di halaman."

    # items loop
    - icon: "manipulate"
      title: "Memanipulasi tanda tangan"
      content: "Cari, perbarui, atau hapus semua tanda tangan yang telah ditambahkan sebelumnya."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Lindungi file Anda menggunakan tanda tangan"
  description: "Contoh kode GroupDocs.Signature"
  items:
    # code sample loop
    - title: "Hasilkan dan tambahkan kode QR"
      content: |
       GroupDocs.Signature memungkinkan kami membuat dan menambahkan kode QR ke dokumen dengan format yang didukung. Berikan jalur ke dokumen yang harus ditandatangani dan atur opsi teks dan visual kode QR yang diinginkan. Anda dapat meletakkan gambar kode QR yang dihasilkan di area mana pun di halaman dokumen mana pun.
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // Tentukan dokumen yang akan ditandatangani
            using (Signature signature = new Signature("source.docx"))
            {
                // Buat opsi tanda kode QR
                QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith")
                {
                    // Atur opsi kode QR
                    EncodeType = QrCodeTypes.QR,
                    Left = 50,
                    Top = 150,
                };

                // Tanda tangani dan simpan file yang diproses
                SignResult result = signature.Sign("result.docx", options);
            }
            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // Tentukan dokumen yang akan ditandatangani
            Signature signature = new Signature("source.docx");

            // Buat opsi tanda kode QR
            QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith");

            // Atur opsi kode QR
            options.setEncodeType(QrCodeTypes.QR);
            options.setLeft(50);
            options.setTop(100);

            // Tanda tangani dan simpan file yang diproses
            signature.sign("result.docx", options);
            ```
        - language: "TypeScript"
          color: "green"
          content: |
            ```javascript {style=abap}  
            const signatureLib = require('@groupdocs/groupdocs.signature')

            // Tentukan dokumen yang akan ditandatangani
            const signature = new signatureLib.Signature('source.docx');

            // Buat opsi tanda kode QR
            const options = new signatureLib.QrCodeSignOptions('JohnSmith');

            // Atur opsi kode QR
            options.setEncodeType(signatureLib.QrCodeTypes.QR);
            options.setLeft(50);
            options.setTop(100);

            // Tanda tangani dan simpan file yang diproses
            signature.sign('result.docx', options);
            ```
        - language: "Python"
          color: "yellow"
          content: |
            ```python {style=abap}  
            import groupdocs.signature as sg

            def run():

                # Tentukan dokumen yang akan ditandatangani
                with sg.Signature('source.docx') as signature:

                    # Buat opsi tanda kode QR
                    options = sg.QrCodeSignOptions('JohnSmith')

                    # Atur opsi kode QR
                    options.setEncodeType(sg.QrCodeTypes.QR)
                    options.setLeft(50)
                    options.setTop(100)

                    # Tanda tangani dan simpan file yang diproses
                    signature.sign('result.docx', options)
            ```

############################# Supported Formats ###############################
formats:
  enable: true
  title: "60+ format file didukung"
  description: "GroupDocs.Signature mendukung hampir semua format file populer"

############################# Metrics ###############################
metrics:
  enable: true
  title: "Data statistik perpustakaan kami"
  description: "Periksa metrik produk utama, ungkapkan wawasan tentang pencapaian, dampak, dan pertumbuhan kami"

  items:
    # items loop
    - number: "50+"
      title: "Format yang didukung"
      content: "Menandatangani lebih dari 60 format file bisnis paling populer."

    # items loop
    - number: "500k"
      title: "Unduhan NuGet"
      content: "GroupDocs.Signature untuk .NET adalah perpustakaan populer dengan lebih dari 550.000 unduhan di NuGet."

    # items loop
    - number: "15k"
      title: "Unduhan Maven"
      content: "Pengembang Java telah mengunduh GroupDocs.Signature di Maven lebih dari 15 ribu kali."

    # items loop
    - number: "140+"
      title: "Pelanggan yang senang"
      content: "Pengembang individu dan perusahaan terkemuka di seluruh dunia menggunakan produk kami untuk membangun solusi inovatif."


############################# Customers ###############################
customers:
  enable: true
  title: "Pelanggan kami yang bahagia"
  description: "Perpustakaan GroupDocs digunakan oleh merek-merek terkenal dan terkemuka secara global di seluruh dunia"

  items:
    # items loop
    - title: "BenQ Corporation"
      logo: "benq"
      
    # items loop
    - title: "Nasdaq Stock Market"
      logo: "nasdaq"
      
    # items loop
    - title: "AT&T Inc."
      logo: "att"
      
    # items loop
    - title: "Customer logo AstraZeneca"
      logo: "astrazeneca"
      
    # items loop
    - title: "Central Bank of Argentina"
      logo: "argentinacentralbank"
      
    # items loop
    - title: "Roche Holding AG"
      logo: "roche"
      
    # items loop
    - title: "Capita"
      logo: "capita"
      
    # items loop
    - title: "Axa S.A."
      logo: "axa"
      
    # items loop
    - title: "Instructure Inc."
      logo: "instructure"
      
    # items loop
    - title: "Wipro"
      logo: "wipro"


############################# Actions ###############################
actions:
  enable: true
  title: "Siap untuk memulai?"
  description: "Coba fitur GroupDocs.Signature secara gratis di platform Anda"

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/signature/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/signature/java/"

    # items loop
    - title: "Node.js"
      color: "green"
      link: "/signature/nodejs-java/"      

############################# FAQ ###############################
faq:
  enable: true
  title: "Pertanyaan yang sering diajukan"
  description: "Jelajahi Pertanyaan Umum kami"

  items:
    # items loop
    - question: "Apakah GroupDocs.Signature memerlukan perpustakaan eksternal untuk penandatanganan dokumen?"
      answer: "Tidak, GroupDocs.Signature bekerja secara independen. Tidak ada ketergantungan pihak ketiga seperti Adobe Acrobat, Microsoft Office, dll."

    # items loop
    - question: "Apakah mungkin untuk menguji fitur GroupDocs.Signature sebelum membeli?"
      answer: "Sangat! GroupDocs.Signature menawarkan uji coba gratis. Instal dan jelajahi fitur-fiturnya. Perhatikan bahwa versi uji coba menambahkan 'lencana uji coba' ke dokumen Anda dan hanya memproses 3 halaman pertama. Untuk pengalaman penuh, dapatkan lisensi sementara gratis selama 30 hari untuk mengakses semua fungsi. Lihat detailnya di bawah [lisensi sementara](https://purchase.groupdocs.com/temporary-license/)."

    # items loop
    - question: "Jenis lisensi apa yang disediakan?"
      answer: "Mencari lisensi GroupDocs.Signature? Kami menawarkan berbagai pilihan yang disesuaikan dengan kebutuhan Anda. Pilih berdasarkan ukuran tim, lokasi penerapan (kantor tunggal atau tempat kerja jarak jauh), dan apakah distribusi pelanggan akhir memerlukan berbagi SDK/API dengan klien. Alternatifnya, pilihlah lisensi penggunaan bulanan dengan paket terukur—bayar hanya untuk apa yang Anda gunakan. Temukan yang paling cocok untuk Anda berdasarkan [harga](https://purchase.groupdocs.com/pricing/signature/net/)."

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "GroupDocs.Signature API kode rendah"
  description: "Tanda tangani file menggunakan aplikasi Anda melalui REST API berbasis cloud kami."
  
  items:
    # items loop
    - title: "GroupDocs.Signature Cloud for cURL"
      content: "Gunakan cURL RESTful API untuk memberi tanda tangan pada PDF, Word, Excel, PowerPoint, JPEG, dan banyak format file lainnya."
      icon: "groupdocs_signature-for-curl"
      link: "https://products.groupdocs.cloud/signature/curl"

    # items loop
    - title: "GroupDocs.Signature Cloud for .NET"
      content: "Perkaya aplikasi .NET Anda dengan penandatanganan dokumen melalui Cloud SDK. Lindungi dokumen bisnis dengan cara Anda sendiri."
      icon: "groupdocs_signature-for-net"
      link: "https://products.groupdocs.cloud/signature/net"

    # items loop
    - title: "GroupDocs.Signature Cloud for Java"
      content: "GroupDocs.Signature SDK memberikan akses ke berbagai kemungkinan bagi aplikasi Java Anda untuk menandatangani file apa pun."
      icon: "groupdocs_signature-for-java"
      link: "https://products.groupdocs.cloud/signature/java"

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Signature Aplikasi web"
  description: "GroupDocs.Signature menghadirkan aplikasi web gratis tempat Anda dapat menandatangani dokumen. Lebih dari 60 format file populer dapat ditandatangani melalui browser favorit Anda GRATIS."

  items:
    # items loop
    - title: "GroupDocs.Signature Total"
      content: "Alat online untuk memberi tanda tangan pada dokumen dari perangkat apa pun."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/signature/total"

    # items loop
    - title: "GroupDocs.Signature DOCX"
      content: "Tanda tangani MS Word DOCX online."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/signature/docx"

    # items loop
    - title: "GroupDocs.Signature PDF"
      content: "Lindungi dokumen PDF secara online."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/signature/pdf"


      


---