        
        // Set up input <% get "Fileformat" %> file
        String filePath = "input.<% lower (get "Fileformat") %>";
        // Set up output file
        String outputFilePath = "output.<% lower (get "Fileformat") %>";
        // Provide image file
        String imageFilePath = "image.png";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        ImageSignOptions options = new ImageSignOptions(imageFilePath);

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign <% get "Fileformat" %> document
        SignResult result = signature.sign(outputFilePath, options);