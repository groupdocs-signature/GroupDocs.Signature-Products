---
############################# Static ############################
layout: "landing"
date: 2024-03-05T08:14:01
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: el
#productCode: java
#otherformats: 
#breadcrumb: Put  signature on  for Java
product: "Signature"
product_tag: "signature"
platform: "Net"
platform_tag: "net"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: ".NET, Java, Cloud API & Online Document Signature Apps"
head_description: "Αποκτήστε ολοκληρωμένη λύση ηλεκτρονικής υπογραφής εγγράφων για .NET, Java και εφαρμογές που βασίζονται σε cloud. Υπογράψτε κοινές μορφές εγγράφων στο διαδίκτυο χρησιμοποιώντας την απλή λειτουργία μεταφοράς και απόθεσης"

############################# Header ############################
title: "Υπογράψτε έγγραφα<br>μέσω .NET API"
description: "Υπογράψτε ψηφιακά έγγραφα και εικόνες σε οποιαδήποτε πλατφόρμα χρησιμοποιώντας τα ευέλικτα API και τις λύσεις που βασίζονται σε εφαρμογές για προγραμματιστές και τελικούς χρήστες."
words:
  for: "Για"

actions:
  main: "Δωρεάν λήψη NuGet"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "Αδειοδότηση"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net"
  title: "Είστε έτοιμοι να ξεκινήσετε;"
  description: "Δοκιμάστε τις δυνατότητες GroupDocs.Signature δωρεάν ή ζητήστε άδεια"

release:
  title: "Κυκλοφόρησε η έκδοση {0}"
  notes: "Δείτε τι νέο υπάρχει"
  downloads: "Λήψεις"

code:
  title: "Υπογραφή αρχείων PDF σε C#"
  more: "Περισσότερα παραδείγματα"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // Επιλέξτε έγγραφο PDF
    using (Signature signature = new Signature("sample.pdf"))
    {
        // Δώστε κείμενο
        var options = new TextSignOptions("John Smith")
        {
            // Σετ χρώματος
            ForeColor = Color.Red
        };
        // Υπογράψτε το έγγραφο και αποθηκεύστε στο αρχείο
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Επισκόπηση GroupDocs.Signature"
  description: "API για την εκτέλεση υπογραφής εγγράφων και σχετικών λειτουργιών σε εφαρμογές .NET"
  features:
    # feature loop
    - title: "Προσθήκη υπογραφών σε επαγγελματικά έγγραφα σε C#"
      content: "Υπογραφή εγγράφων: Με το GroupDocs.Signature για .NET, μπορείτε να προσθέσετε διάφορους τύπους υπογραφών, όπως κείμενο, εικόνες, γραμμωτούς κώδικες και ψηφιακά πιστοποιητικά, σε έγγραφα PDF και Office. Αυτό το API σάς επιτρέπει να υπογράφετε τα έγγραφά σας με σχεδόν οποιονδήποτε τύπο δεδομένων, συμπεριλαμβανομένων των κρυφών μεταδεδομένων."

    # feature loop
    - title: "Επεξεργασία υπογεγραμμένων εγγράφων"
      content: "Πρόσθετη επεξεργασία: Μπορείτε να εκτελέσετε ισχυρές λειτουργίες σε υπογεγραμμένα έγγραφα χρησιμοποιώντας το GroupDocs.Signature. Αυτό περιλαμβάνει την αναζήτηση για υπάρχουσες υπογραφές εντός των επιχειρηματικών εγγράφων και την επαλήθευση τους χρησιμοποιώντας συγκεκριμένα κριτήρια. Επιπλέον, μπορείτε να ανακτήσετε πληροφορίες εγγράφων και να κάνετε προεπισκόπηση σελίδων μέσω αυτού του .NET API."

    # feature loop
    - title: "Προσαρμογή αποτελεσμάτων"
      content: "Το GroupDocs.Signature για .NET προσφέρει εκτενείς επιλογές προσαρμογής. Μπορείτε να τοποθετήσετε με ακρίβεια τις υπογραφές οπουδήποτε σε μια σελίδα εγγράφου και να προσαρμόσετε την εμφάνισή τους χρησιμοποιώντας μια ποικιλία ρυθμίσεων. Επιπλέον, αυτό το API υποστηρίζει την αποθήκευση επεξεργασμένων εγγράφων σε ένα ευρύ φάσμα υποστηριζόμενων μορφών."

############################# Platforms ############################
platforms:
  enable: true
  title: "Ανεξαρτησία πλατφόρμας"
  description: "Το GroupDocs.Signature για .NET υποστηρίζει τα ακόλουθα λειτουργικά συστήματα, πλαίσια και διαχειριστές πακέτων"
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "Υποστηριζόμενες μορφές αρχείων"
  description: |
    Το GroupDocs.Signature για .NET υποστηρίζει λειτουργίες με τις ακόλουθες [μορφές αρχείων](https://docs.groupdocs.com/signature/net/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Μορφές Microsoft Office
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Εικόνες & Άλλες Μορφές
        * **Φορητός:** PDF
        * **εικόνες:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Άλλες μορφές γραφείου:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Άλλες μορφές
        * **Ιστός:** HTML, MHTML
        * **Αρχεία:** ZIP, TAR, 7Z
        * **Πιστοποιητικά:** PFX

############################# Features ############################
features:
  enable: true
  title: "Λειτουργίες GroupDocs.Signature"
  description: "Υπογραφή αρχείων PDF, εγγράφων του Office και εικόνων γρήγορα και με ακρίβεια"

  items:
    # feature loop
    - icon: "sign"
      title: "Υπογραφή εγγράφου"
      content: "Προσθέστε έναν ή πολλούς υποστηριζόμενους τύπους υπογραφών με ακρίβεια σε οποιαδήποτε καθορισμένη θέση στα επαγγελματικά έγγραφα."

    # feature loop
    - icon: "custom"
      title: "Προσαρμόστε τις υπογραφές"
      content: "Χρησιμοποιήστε λειτουργίες όπως χρώμα, γραμματοσειρά, περίγραμμα, περιστροφή κ.λπ., για να διαμορφώσετε την εμφάνιση των υπογραφών."

    # feature loop
    - icon: "password"
      title: "Προστασία με κωδικό πρόσβασης εγγράφου"
      content: "Ασφαλίστε ορισμένους τύπους εγγράφων ορίζοντας έναν κωδικό πρόσβασης μετά την υπογραφή."

    # feature loop
    - icon: "protect"
      title: "Προστασία από αλλαγές"
      content: "Αποτρέψτε αλλαγές σε σημαντικά επιχειρηματικά έγγραφα μετά την προσάρτηση μιας υπογραφής με ψηφιακό πιστοποιητικό."

    # feature loop
    - icon: "convert"
      title: "Μετατροπή υπογεγραμμένων αρχείων σε άλλες μορφές"
      content: "Μετατρέψτε τα υπογεγραμμένα αρχεία σε επιθυμητές μορφές, όπως η αποθήκευση ενός εγγράφου του Word ως PDF."

    # feature loop
    - icon: "preview"
      title: "Εξαγωγή προεπισκοπήσεων σελίδων"
      content: "Εξαγωγή σελίδων από υπογεγραμμένα έγγραφα ως μεμονωμένες εικόνες για μελλοντική επεξεργασία."

    # feature loop
    - icon: "search"
      title: "Αναζήτηση υπογραφών σε έγγραφα"
      content: "Ανακτήστε πληροφορίες σχετικά με υπογραφές που προστέθηκαν προηγουμένως σε συγκεκριμένα έγγραφα."

    # feature loop
    - icon: "validate"
      title: "Επικύρωση υπογεγραμμένων εγγράφων"
      content: "Επαληθεύστε τη σωστή υπογραφή των εγγράφων χρησιμοποιώντας λειτουργίες επικύρωσης."

    # feature loop
    - icon: "update"
      title: "Ενημερώστε ή διαγράψτε τις υπογραφές"
      content: "Τοποθετήστε εύκολα συγκεκριμένες υπογραφές σε μια σελίδα, τροποποιήστε το κείμενό τους ή διαγράψτε τις χωρίς προβλήματα."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Δείγματα κωδικών"
  description: "Ορισμένες περιπτώσεις χρησιμοποιούν τυπικά GroupDocs.Signature για λειτουργίες .NET"
  items:
    # code sample loop
    - title: "Προσθήκη QR-code σε PDF"
      content: |
        Η προσθήκη [QR-codes](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) σε συγκεκριμένες σελίδες εγγράφων PDF μπορεί να βελτιώσει τις επιχειρηματικές διαδικασίες. Παρακάτω είναι ένα παράδειγμα για το πώς μπορείτε να προσθέσετε έναν κωδικό QR χρησιμοποιώντας το GroupDocs.Signature.
        {{< landing/code title="Πώς να τοποθετήσετε τον κωδικό QR σε PDF.">}}
        ```csharp {style=abap}
        // Φορτώστε το έγγραφο για υπογραφή
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Δημιουργήστε επιλογές κωδικού QR με προκαθορισμένο κείμενο
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // Διαμορφώστε τον τύπο και τη θέση κωδικοποίησης κώδικα QR στη σελίδα
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // Υπογράψτε το έγγραφο και αποθηκεύστε το ως αρχείο αποτελεσμάτων
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Προστασία ενός εγγράφου DOCX με χρήση ψηφιακού πιστοποιητικού"
      content: |
        Μπορείτε να [Προστασία εγγράφου](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/) χρησιμοποιώντας προσωπικές ή εταιρικές υπογραφές που είναι αποθηκευμένες ως ψηφιακά πιστοποιητικά. Τέτοια προστατευόμενα έγγραφα δεν μπορούν να τροποποιηθούν χωρίς να ακυρωθεί η υπογραφή.
        {{< landing/code title="Ακολουθεί ο τρόπος διασφάλισης της ακεραιότητας του εγγράφου.">}}
        ```csharp {style=abap}   
        // Φορτώστε το έγγραφο που πρόκειται να υπογραφεί ψηφιακά
        using (Signature signature = new Signature("file_to_sign.docx"))
        {
            // Καθορίστε τις επιλογές ψηφιακής υπογραφής και δώστε τη διαδρομή προς το αρχείο πιστοποιητικού
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // Ορίστε τον κωδικό πρόσβασης του πιστοποιητικού
                Password = "1234567890"
            };
            // Υπογράψτε το έγγραφο και αποθηκεύστε το στην επιθυμητή διαδρομή
            signature.Sign("digitally_signed.docx", options);
        }
        ```
        {{< /landing/code >}}

---
