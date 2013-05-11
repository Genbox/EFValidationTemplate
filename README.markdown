# EF 5 Validation Template with DataAnnotations

An Entity Framework T4 template for auto-generating EF DataAnnotation validation code for entities
based on metadata from the database.

### Features

* Puts [Required] on not null fields
* Detects datetime, int and floating point numbers and inserts datatype range values
* Guesses the kind of data and applies the appropriate regular expression for validation

### Usage

Just drag and drop it into your Visual Studio project and change "MyModel.edmx" in the .tt file to match the name of your datamodel.
It will create a metadata class which you should copy to another file, and then you can remove the .tt template.