marketo_gem
===========

More information about this gem can be found at [Rapleaf](https://www.rapleaf.com/developers/rapleaf-labs/marketo-gem-documentation/).

Note that you probably need to specify your API endpoint as well as your API key and secret.  It's also possible to specify the API version you'd like to use.

Your own key, secret and subdomain are found within Marketo > Admin > Integration > SOAP API.

For example:

```ruby

access_key = "your_access_key"    # Marketo UI calls this User ID
secret = "your_secret"            # Marketo UI calls this Encryption Key
your_subdomain = "na-l"           # Look for this in what Marketo UI calls 'SOAP endpoint'

client = Rapleaf::Marketo.new_client(access_key, secret, api_subdomain = your_subdomain, api_version = '1_5', document_version = '1_4')
```
