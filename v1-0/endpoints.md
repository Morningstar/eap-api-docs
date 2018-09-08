# API v1.0 Endpoints

## Authenticate

~~~
https://theomx.com/api/1.0/authenticate
~~~

### Input Parameters

<table>
  <tr>
    <td><b>Parameter</b></td>
    <td><b>Example</b></td>
    <td><b><b>Notes</b></b></td>
  </tr>
  <tr>
    <td>api_key</td>
    <td>fsd8hos8d7fh8s7dfhsfg7fgs7gf</td>
    <td>Mandatory</td>
  </tr>
  <tr>
    <td>format</td>
    <td>json</td>
    <td>Must be json or xml. Defaults to json if not present.</td>
  </tr>
</table>

### Resultset

<table>
  <tr>
    <td><b>Field</b></td>
    <td><b>Value</b></td>
    <td><b><b>Notes</b></b></td>
  </tr>
  <tr>
    <td>token</td>
    <td>fsd8hos8d7fh8s7dfhsfg7fgs7gf</td>
    <td></td>
  </tr>
  <tr>
    <td>expires_on</td>
    <td>2018-01-01 12:00:00</td>
    <td>One hour from time of query. GMT.</td>
  </tr>
</table>

## Organizations

~~~
https://theomx.com/api/1.0/organizations
~~~

### Input Parameters (truncated)

<table>
  <tr>
    <td><b>Parameter</b></td>
    <td><b>Example</b></td>
    <td><b><b>Notes</b></b></td>
  </tr>
  <tr>
    <td>token</td>
    <td>fsd8hos8d7fh8s7dfhsfg7fgs7gf</td>
    <td>Mandatory</td>
  </tr>
  <tr>
    <td>format</td>
    <td>json</td>
    <td>Must be json, xml or csv. Defaults to json if not present.</td>
  </tr>
  <tr>
    <td>page</td>
    <td>1</td>
    <td>Defaults to 1 if not present.</td>
  </tr>
  <tr>
    <td>keywords</td>
    <td>{'aircraft', 'helicopters'}</td>
    <td></td>
  </tr>
  <tr>
    <td>country</td>
    <td>CA</td>
    <td></td>
  </tr>
</table>

### Resultset (truncated)

<table>
  <tr>
    <td><b>Field</b></td>
    <td><b>Value</b></td>
    <td><b><b>Notes</b></b></td>
  </tr>
  <tr>
    <td>id</td>
    <td>32344</td>
    <td></td>
  </tr>
  <tr>
    <td>organization_name</td>
    <td>Acme Corporation</td>
    <td></td>
  </tr>
  <tr>
    <td>description</td>
    <td>Supplier of premium widgets</td>
    <td>First 100 characters</td>
  </tr>
  <tr>
    <td>country</td>
    <td>CA</td>
    <td></td>
  </tr>
</table>

### Input Parameters (robust)

<table>
  <tr>
    <td><b>Parameter</b></td>
    <td><b>Example</b></td>
    <td><b><b>Notes</b></b></td>
  </tr>
  <tr>
    <td>token</td>
    <td>fsd8hos8d7fh8s7dfhsfg7fgs7gf</td>
    <td>Mandatory</td>
  </tr>
  <tr>
    <td>format</td>
    <td>json</td>
    <td>Must be json, xml or csv. Defaults to json if not present.</td>
  </tr>
  <tr>
    <td>page</td>
    <td>1</td>
    <td>Defaults to 1 if not present.</td>
  </tr>
  <tr>
    <td>keywords</td>
    <td>{'aircraft', 'helicopters'}</td>
    <td></td>
  </tr>
  <tr>
    <td>country</td>
    <td>CA</td>
    <td></td>
  </tr>
  <tr>
    <td>is_claimed</td>
    <td>true</td>
    <td></td>
  </tr>
  <tr>
    <td>is_verified</td>
    <td>true</td>
    <td></td>
  </tr>
  <tr>
    <td>aboriginal_owned</td>
    <td>true</td>
    <td></td>
  </tr>
  <tr>
    <td>veteran_owned</td>
    <td>true</td>
    <td></td>
  </tr>
  <tr>
    <td>women_owned</td>
    <td>true</td>
    <td></td>
  </tr>
  <tr>
    <td>unspsc_codes</td>
    <td>{'10000000', '11000000'}</td>
    <td></td>
  </tr>
  <tr>
    <td>naics_codes</td>
    <td>{'111110', '121110'}</td>
    <td></td>
  </tr>
  <tr>
    <td>nsn_codes</td>
    <td>{'5110005709017', '2110005709017'}</td>
    <td></td>
  </tr>
  <tr>
    <td>fsc_codes</td>
    <td>{'1234', '5678'}</td>
    <td></td>
  </tr>
  <tr>
    <td>certifications</td>
    <td>{'ISO9001', 'ISO14001'}</td>
    <td></td>
  </tr>
  <tr>
    <td>organization_type</td>
    <td>Supplier</td>
    <td></td>
  </tr>
  <tr>
    <td>countries_exported_to</td>
    <td>{'CA', 'US'}</td>
    <td></td>
  </tr>
</table>

### Resultset (robust)

<table>
  <tr>
    <td><b>Field</b></td>
    <td><b>Value</b></td>
    <td><b><b>Notes</b></b></td>
  </tr>
  <tr>
    <td>id</td>
    <td>32344</td>
    <td></td>
  </tr>
  <tr>
    <td>organization_name</td>
    <td>Acme Corporation</td>
    <td></td>
  </tr>
  <tr>
    <td>description</td>
    <td>Supplier of premium widgets</td>
    <td></td>
  </tr>
  <tr>
    <td>country</td>
    <td>CA</td>
    <td></td>
  </tr>
  <tr>
    <td>website</td>
    <td>https://domain.com</td>
    <td></td>
  </tr>
  <tr>
    <td>telephone</td>
    <td>555-555-5555</td>
    <td>Format may vary</td>
  </tr>
  <tr>
    <td>ext</td>
    <td>123</td>
    <td></td>
  </tr>
  <tr>
    <td>email</td>
    <td>user@domain.com</td>
    <td></td>
  </tr>
  <tr>
    <td>is_claimed</td>
    <td>true</td>
    <td></td>
  </tr>
  <tr>
    <td>is_verified</td>
    <td>true</td>
    <td></td>
  </tr>
  <tr>
    <td>aboriginal_owned</td>
    <td>true</td>
    <td></td>
  </tr>
  <tr>
    <td>veteran_owned</td>
    <td>true</td>
    <td></td>
  </tr>
  <tr>
    <td>women_owned</td>
    <td>true</td>
    <td></td>
  </tr>
  <tr>
    <td>number_of_current_opportunities</td>
    <td>3</td>
    <td></td>
  </tr>
  <tr>
    <td>organization_types</td>
    <td>{'Supplier'}</td>
    <td></td>
  </tr>
  <tr>
    <td>countries_exported_to</td>
    <td>{'CA', 'US'}</td>
    <td></td>
  </tr>
  <tr>
    <td>key_industrial_capabilities</td>
    <td>Spot welding</td>
    <td></td>
  </tr>
  <tr>
    <td>annual_sales</td>
    <td>100000</td>
    <td></td>
  </tr>
  <tr>
    <td>annual_exports</td>
    <td>Spot welding</td>
    <td></td>
  </tr>
  <tr>
    <td>year_established</td>
    <td>1950</td>
    <td></td>
  </tr>
  <tr>
    <td>total_employees</td>
    <td>250</td>
    <td></td>
  </tr>
  <tr>
    <td>major_clients</td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>major_projects</td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>languages</td>
    <td>{'ENG', 'SPA'}</td>
    <td></td>
  </tr>
  <tr>
  <tr>
    <td>unspsc_codes</td>
    <td>{'10000000', '11000000'}</td>
    <td></td>
  </tr>
  <tr>
    <td>naics_codes</td>
    <td>{'111110', '121110'}</td>
    <td></td>
  </tr>
  <tr>
    <td>nsn_codes</td>
    <td>{'5110005709017', '2110005709017'}</td>
    <td></td>
  </tr>
  <tr>
    <td>fsc_codes</td>
    <td>{'1234', '5678'}</td>
    <td></td>
  </tr>
  <tr>
    <td>lei_codes</td>
    <td>{'1234567890123456789A'}</td>
    <td></td>
  </tr>
  <tr>
    <td>duns</td>
    <td>203848726</td>
    <td></td>
  </tr>
  <tr>
    <td>cage</td>
    <td>1234</td>
    <td></td>
  </tr>
  <tr>
    <td>jco</td>
    <td>123456789</td>
    <td></td>
  </tr>
  <tr>
    <td>certifications</td>
    <td>{'ISO9001', 'ISO14001'}</td>
    <td></td>
  </tr>
    <td>alliances</td>
    <td>{'CADSI', 'AIAC'}</td>
    <td></td>
  </tr>
  <tr>
    <td>products_and_services</td>
    <td>{'Product name 1', 'Service name 1'}</td>
    <td></td>
  </tr>
</table>
