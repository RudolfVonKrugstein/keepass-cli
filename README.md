# keepass-cli

Cli interface for keepass writing in python and based on [libkeepas](https://github.com/phpwutz/libkeepass).

The following commands are available (the password can always aso be passed through the KEEPASS_PASSWORD environment variable):

* show-entry -f <filename> -p <password> -e <path-to-entry> -f <field-to-retrieve>
  Return the given field from the given entry. If no field is given, it defaults to "Password"
  
* list-entries: -f <filename> -p <password> -e <path-to-group>
  List all entries in the given group
  
* to-json: -f <filename> -p <password> -e <path-to-group> -f <field-names>
  Prints an json object with everything found below the given group. Only the fields in <field-names> (which is a comma sperated list) are included.
