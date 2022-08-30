        
        // Set up input <% get "Fileformat" %> file
        string filePath = "input.<% lower (get "Fileformat") %>";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be updated
        // such Id might be get as result of search operation
        string id = "07f83369-318b-41ad-a843-732417b912c2";

        // provide signature features to update
        BarcodeSignature signatureToUpdate = new BarcodeSignature();

        // set up particular signature id
        signatureToUpdate.setSignatureId(id);
        // specify signature width
        signatureToUpdate.setWidth(300);
        // specify signature height
        signatureToUpdate.setHeight(50);
        // set left position
        signatureToUpdate.setLeft(80);
        // set top position
        signatureToUpdate.setTop(100);

        // update signature
        bool updateResult = signature.Update(signatureToUpdate);

        // process updation result
        if (updateResult)
        {
                System.out.println("Signature was updated successfully!");
        }