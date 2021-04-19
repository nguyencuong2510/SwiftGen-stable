# YAML parser

## Input

The YAML parser accepts multiple files or directories (which it'll recursively search). Each file's content will be loaded into the context, but the parser will also generate metadata about the structure of the file.

YAML files can contain multiple documents, which is why each file can contain multiple `documents` in the structure below.

Note: The JSON, YAML and Plist parsers provide the same context structure, so you can easily switch input formats while keeping the same template.

### Filter

The default filter for this command is: `[^/]\\.(?i:ya?ml)$`. That means it'll accept any file with the extensions `yaml` or `yml`.

You can provide a custom filter using the `filter` option, it accepts any valid regular expression. See the [Config file documentation](../ConfigFile.md) for more information.


## Customization

This parser currently doesn't accept any options.

## Templates

* [See here](../templates/yaml) for a list of templates bundled with SwiftGen and their documentation.
* If you want to write custom templates, make sure to check the [stencil context documentation](../SwiftGenKit%20Contexts/yaml.md) to see what data is available after parsing.
