        
        // Set up input <% get "Fileformat" %> file
        string filePath = "input.<% lower (get "Fileformat") %>";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Create search options
        DigitalSearchOptions options = new DigitalSearchOptions();

        // specify special search criteria
        options.setComments("Approved");
        // specify period of signatures
        options.setSignDateTimeFrom(LocalDate.of(2021, 3, 5));
        options.setSignDateTimeTo(LocalDate.of(2022, 7, 16));
        
        // search for <% get "Signaturetype" %> signatures in <% get "Fileformat" %> document
        List<DigitalSignature> signatures = signature.Search<DigitalSignature>(options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println("..."));
