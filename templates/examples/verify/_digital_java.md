        
        // Set up input <% get "Fileformat" %> file
        string filePath = "input.<% lower (get "Fileformat") %>";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide verification options
        DigitalVerifyOptions options = new DigitalVerifyOptions();

        // Digital signature comment
        options.setComments("Approved");

        // specify period of signatures
        options.setSignDateTimeFrom(LocalDate.of(2020, 12, 12));
        options.setSignDateTimeTo(LocalDate.of(2022, 12, 12));
                            
        // Verify document signatures
        VerificationResult result = signature.Verify(options);

        //process result
        if (result.IsValid)
        {
            //..
        }