        // Instantiate Signature for <% get "FILEFORMAT" %> file
        string filePath = "input.<% lower (get "FILEFORMAT") %>";
        // Set up output <% get "FILEFORMAT" %> file
        string outputFilePath = "output.<% lower (get "FILEFORMAT") %>";

        Signature signature = new Signature(filePath);

        //Provide sign options
        TextSignOptions options = new TextSignOptions("John Smith");

        // set signature position
        options.setLeft(50);
        options.setTop(50);

        // sign <% get "FILEFORMAT" %> document
        SignResult result = signature.sign(outputFilePath, options);
