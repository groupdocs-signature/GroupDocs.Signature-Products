
        // Set up input <% get "Fileformat" %> file
        string filePath = "input.<% lower (get "Fileformat") %>";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // search for <% get "Signaturetype" %> signatures in <% get "Fileformat" %> document
        List<PdfMetadataSignature> signatures = signature.Search<PdfMetadataSignature>(SignatureType.Metadata);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println("..."));

