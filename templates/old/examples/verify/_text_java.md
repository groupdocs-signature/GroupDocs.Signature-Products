        
        // Set up input <% get "Fileformat" %> file
        String filePath = "input.<% lower (get "Fileformat") %>";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide verification options
        TextVerifyOptions options = new TextVerifyOptions();

        // Process all pages
        options.setAllPages(true);
        // specify text match type
        options.setMatchType(TextMatchType.Exact);
        // specify text pattern to search
        options.setText("Very important signature");
                            
        // Verify document signatures
        VerificationResult result = signature.verify(options);

        //process result
        if (result.isValid())
        {
            //..
        }
