
        // Set up input <% get "FILEFORMAT" %> file
        string filePath = "input.<% lower (get "FILEFORMAT") %>";
        // Set up output file
        string outputFilePath = "output.<% lower (get "FILEFORMAT") %>";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(BarcodeTypes.<% get "Codetype" %>);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign <% get "FILEFORMAT" %> document
        SignResult result = signature.sign(outputFilePath, options);
