        
        // Set up input <% get "Fileformat" %> file
        string filePath = "input.<% lower (get "Fileformat") %>";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be deleted
        // such Id may be obtained as result of search operation
        string id = "07f83369-318b-41ad-a843-732417b912c2";

        // provide signature features to delete
        BarcodeSignature signatureToDelete = new BarcodeSignature();

        // set up particular signature id
        signatureToDelete.setSignatureId(id);

        // delete signature
        bool deleteResult = signature.Delete(signatureToDelete);

        // process deletion result
        if (deleteResult)
        {
                System.out.println("Signature was deleted successfully!");
        }