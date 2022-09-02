        
        // Set up input <% get "Fileformat" %> file
        String filePath = "input.<% lower (get "Fileformat") %>";
        // Set up output file
        String outputFilePath = "output.<% lower (get "Fileformat") %>";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(QrCodeTypes.<% get "Codetype" %>);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign <% get "Fileformat" %> document
        SignResult result = signature.sign(outputFilePath, options);
