
        // Set up input <% get "Fileformat" %> file
        string filePath = "input.<% lower (get "Fileformat") %>";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Create search options
        BarcodeSearchOptions options = new BarcodeSearchOptions();

        // specify special pages to search on 
        options.setAllPages(false);
        // single page number
        options.setPageNumber(1);
        // specify text match type
        options.setMatchType(TextMatchType.Contains);
        // specify text pattern to search
        options.setText("Text signature");
        // return  <% get "Signaturetype" %> images for processing
        options.setReturnContent(true);
        // set up type of returned  <% get "Signaturetype" %> images
        options.setReturnContentType(FileType.PNG);
                            
        // search for <% get "Signaturetype" %> signatures in <% get "Fileformat" %> document
        List<BarcodeSignature> signatures = signature.Search<BarcodeSignature>(options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println("..."));
