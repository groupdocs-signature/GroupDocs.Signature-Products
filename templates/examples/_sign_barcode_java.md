        // Instantiate Signature for <% get "FILEFORMAT" %> file
        string filePath = "input.<% lower (get "FILEFORMAT") %>";
        // Set up output <% get "FILEFORMAT" %> file
        string outputFilePath = "output.<% lower (get "FILEFORMAT") %>";

        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(BarcodeTypes.<% get "BARCODETYPE" %>);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign <% get "FILEFORMAT" %> document
        SignResult result = signature.sign(outputFilePath, options);
