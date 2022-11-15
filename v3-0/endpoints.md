# API V3.0 Endpoints

## Autenticate

~~~
https://esgperformance.sustainalytics.com/api/3.0/authenticate
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
    <td>"abc123"</td>
    <td>Mandatory</td>
  </tr>
  <tr>
    <td>format</td>
    <td>"json"</td>
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
    <td>datetime</td>
    <td>"2021-01-01T00:00:00.000-04:00"</td>
    <td></td>
  </tr>
  <tr>
    <td>format</td>
    <td>"json"</td>
    <td></td>
  </tr>
  <tr>
    <td>result</td>
    <td>{"token": "a4603ebbe8f819cf0f12386bc7ee359c","expires_on": "2021-01-01T00:00:00.000-04:00"}</td>
    <td></td>
  </tr>
</table>

## Organizations

~~~
https://esgperformance.sustainalytics.com/api/3.0/organizations
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
    <td>"abc123"</td>
    <td>Mandatory</td>
  </tr>
  <tr>
    <td>format</td>
    <td>"json"</td>
    <td>Must be json, xml or csv. Defaults to json if not present.</td>
  </tr>
  <tr>
    <td>page</td>
    <td>1</td>
    <td>Defaults to 1 if not present.</td>
  </tr>
  <tr>
    <td>keywords</td>
    <td>"cloud,infrastructure"</td>
    <td>A comma-separated list of keywords to search by. Returns companies that match given list.</td>
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
    <td>"OMX"</td>
    <td></td>
  </tr>
  <tr>
    <td>description</td>
    <td>"Supplier of premium widgets"</td>
    <td>First 100 characters</td>
  </tr>
  <tr>
    <td>country</td>
    <td>"CA"</td>
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
    <td>"abc123"</td>
    <td>Mandatory</td>
  </tr>
    <tr>
    <td>page</td>
    <td>1</td>
    <td>Defaults to 1 if not present.</td>
  </tr>
  <tr>
    <td>format</td>
    <td>"json"</td>
    <td>Must be json, xml or csv. Defaults to json if not present.</td>
  </tr>
  <tr>
    <td>is_pinned</td>
    <td>true</td>
    <td>Returns pinned companies if true. Otherwise, unpinned companies.</td>
  </tr>
    <tr>
    <td>tags</td>
    <td>"EGB Supplier,Service Provider"</td>
    <td>A comma-separated list of tags. Returns companies that are tagged with the given tags. </td>
  </tr>
  <tr>
    <td>esg_risk_rating_category</td>
    <td>"negligible"</td>
    <td>A comma-separated list of rating categories. Returns companies that match given list.</td>
  </tr>
  <tr>
    <td>nace_codes</td>
    <td>"A01.11"</td>
    <td>A comma-separated list of NACE codes. Returns companies that match given list.</td>
  </tr>
  <tr>
    <td>unspsc_codes</td>
    <td>"10000000,11000000"</td>
    <td>A comma-separated list of UNSPSC codes. Returns companies that match given list.</td>
  </tr>
  <tr>
    <td>naics_codes</td>
    <td>"111110,121110"</td>
    <td>A comma-separated list of NAICS codes. Returns companies that match given list.</td>
  </tr>
  <tr>
    <td>is_claimed</td>
    <td>true</td>
    <td>Returns claimed companies if true. Otherwise, unclaimed companies.</td>
  </tr>
  <tr>
    <td>is_verified</td>
    <td>true</td>
    <td>Returns verified companies if true. Otherwise, unverified companies.</td>
  </tr>
  <tr>
    <td>aboriginal_owned</td>
    <td>true</td>
    <td>Returns aboriginal owned companies if true. Otherwise, not aboriginal owned companies.</td>
  </tr>
  <tr>
    <td>veteran_owned</td>
    <td>true</td>
    <td>Returns veteran owned companies if true. Otherwise, not veteran owned companies.</td>
  </tr>
  <tr>
    <td>women_owned</td>
    <td>true</td>
    <td>Returns women owned companies if true. Otherwise, not women owned companies.</td>
  </tr>
  <tr>
    <td>certifications</td>
    <td>"ISO 9001,ISO 9002"</td>
    <td>A comma-separated list of certifications. Returns companies that match given list.</td>
  </tr>
  <tr>
    <td>organization_type</td>
    <td>"Corporation,Association"</td>
    <td>A comma-separated list of organization types. Returns companies that match given list.</td>
  </tr>
    <tr>
    <td>countries_exported_to</td>
    <td>"CA,US"</td>
    <td>A comma-separated list of countries. Returns companies that match given list.</td>
  </tr>
  <tr>
    <td>keywords</td>
    <td>"aircraft,helicopters"</td>
    <td>A comma-separated list of keywords to search by. Returns companies that match given list.</td>
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
    <td>1</td>
    <td></td>
  </tr>
  <tr>
    <td>description</td>
    <td>"All colors, all sizes"</td>
    <td>First 100 characters</td>
  </tr>
  <tr>
    <td>organization_name</td>
    <td>"OMX"</td>
    <td></td>
  </tr>
  <tr>
    <td>country</td>
    <td>"CA"</td>
    <td></td>
  </tr>
    <tr>
    <td>website</td>
    <td>"https://esgperformance.sustainalytics.com/"</td>
    <td></td>
  </tr>
  <tr>
    <td>email</td>
    <td>"info@theomx.com"</td>
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
    <td>languages</td>
    <td>["eng","fre"]</td>
    <td></td>
  </tr>
  <tr>
    <td>key_industrial_capabilities</td>
    <td>"IT Security Architectures"</td>
    <td></td>
  </tr>
  <tr>
    <td>year_established</td>
    <td>2020</td>
    <td></td>
  </tr>
  <tr>
    <td>telephone</td>
    <td>4379179288</td>
    <td></td>
  </tr>
  <tr>
    <td>ext</td>
    <td>4</td>
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
    <td>organization_types</td>
    <td>["Corporation","Government"]</td>
    <td></td>
  </tr>
  <tr>
    <td>countries_exported_to</td>
    <td>["CA","US"]</td>
    <td></td>
  </tr> 
  <tr>
    <td>annual_sales</td>
    <td>1000000</td>
    <td></td>
  </tr>
  <tr>
    <td>annual_exports</td>
    <td>2100000</td>
    <td></td>
  </tr>
  <tr>
    <td>total_employees</td>
    <td>3100</td>
    <td></td>
  </tr>
  <tr>
    <td>major_clients</td>
    <td>"OMX"</td>
    <td></td>
  </tr>
  <tr>
    <td>unspsc_codes</td>
    <td>"84111700"</td>
    <td></td>
  </tr>
  <tr>
    <td>naics_codes</td>
    <td>["523110","522110"]</td>
    <td></td>
  </tr>
  <tr>
    <td>nace_codes</td>
    <td>["K64.1","K64.11"]</td>
    <td></td>
  </tr>
  <tr>
    <td>nace_codes</td>
    <td>["K64.1","K64.11"]</td>
    <td></td>
  </tr>
  <tr>
    <td>lei_codes</td>
    <td>["959800NEP6XY8CHS8G76","549300QE1RU34T50MR69"]</td>
    <td></td>
  </tr>
  <tr>
    <td>duns</td>
    <td>12345678</td>
    <td></td>
  </tr>
  <tr>
    <td>certifications</td>
    <td>["ISO 9001","ISO 9002"]</td>
    <td></td>
  </tr>
  <tr>
    <td>alliances</td>
    <td>["Aerospace PEI","Aerospace Alberta"]</td>
    <td></td>
  </tr>
  <tr>
    <td>product_and_services</td>
    <td>["Private Banking","Investment Banking"]</td>
    <td></td>
  </tr>
  <tr>
    <td>is_pinned</td>
    <td>true</td>
    <td></td>
  </tr>
  <tr>
    <td>esg_risk_rating_score</td>
    <td>0.8</td>
    <td></td>
  </tr>
  <tr>
    <td>esg_risk_rating_category</td>
    <td>"negligible"</td>
    <td></td>
  </tr>
  <tr>
    <td>esg_risk_rating_class</td>
    <td>"1"</td>
    <td></td>
  </tr>
  <tr>
    <td>esg_risk_exposure_score</td>
    <td>0.8</td>
    <td></td>
  </tr>
  <tr>
    <td>esg_risk_exposure_category</td>
    <td>"negligible"</td>
    <td></td>
  </tr>
  <tr>
    <td>esg_risk_management_score</td>
    <td>0.8</td>
    <td></td>
  </tr>
  <tr>
    <td>esg_risk_management_category</td>
    <td>"negligible"</td>
    <td></td>
  </tr>
</table>

