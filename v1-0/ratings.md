# Ratings API v1.0 Endpoints

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
    <td>ABC123</td>
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
    <td>ABC123</td>
    <td></td>
  </tr>
  <tr>
    <td>expires_on</td>
    <td>2018-01-01 12:00:00</td>
    <td>One hour from time of query. GMT.</td>
  </tr>
</table>

## Match Organizations

~~~
https://theomx.com/api/1.0/organizations/match
~~~

### Input Parameters

<table>
  <tr>
    <td><b>Parameter</b></td>
    <td><b>Example</b></td>
    <td><b><b>Notes</b></b></td>
  </tr>
  <tr>
    <td>token</td>
    <td>ABC123</td>
    <td>Mandatory</td>
  </tr>
  <tr>
    <td>format</td>
    <td>json</td>
    <td>Must be json. Defaults to json if not present.</td>
  </tr>
  <tr>
    <td>company_name</td>
    <td>'ACME Corp'</td>
    <td>Mandatory</td>
  </tr>
  <tr>
    <td>country</td>
    <td>CA</td>
    <td>Mandatory</td>
  </tr>
  <tr>
    <td>province</td>
    <td>ON</td>
    <td>Mandatory</td>
  </tr>
  <tr>
    <td>city</td>
    <td>'Toronto'</td>
    <td>Mandatory</td>
  </tr>
  <tr>
    <td>zipcode</td>
    <td>'A1B2C3'</td>
    <td>Mandatory</td>
  </tr>
  <tr>
    <td>street_name</td>
    <td>'Unnamed Rd.'</td>
    <td>Mandatory</td>
  </tr>
  <tr>
    <td>street_number</td>
    <td>123</td>
    <td></td>
  </tr>
  <tr>
    <td>complement</td>
    <td>'unit 123'</td>
    <td></td>
  </tr>
  <tr>
    <td>telephone</td>
    <td>'+1 (123) 456 7890'</td>
    <td>Mandatory</td>
  </tr>
  <tr>
    <td>extension</td>
    <td>'123'</td>
    <td></td>
  </tr>
  <tr>
    <td>website</td>
    <td>'https://www.example.com/company_website'</td>
    <td>Mandatory</td>
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
    <td>id</td>
    <td>32344</td>
    <td></td>
  </tr>
</table>

## Ratings

~~~
https://theomx.com/api/1.0/ratings
~~~

### Input Parameters

<table>
  <tr>
    <td><b>Parameter</b></td>
    <td><b>Example</b></td>
    <td><b><b>Notes</b></b></td>
  </tr>
  <tr>
    <td>token</td>
    <td>ABC123</td>
    <td>Mandatory</td>
  </tr>
  <tr>
    <td>format</td>
    <td>json</td>
    <td>Must be json, xml or csv. Defaults to json if not present.</td>
  </tr>
  <tr>
    <td>sust_id</td>
    <td>'100012345'</td>
    <td>Mandatory</td>
  </tr>
  <tr>
    <td>omx_id</td>
    <td>'12345'</td>
    <td>Mandatory</td>
  </tr>
  <tr>
    <td>rating</td>
    <td>{ complex JSON structure with ratings data }</td>
    <td>Mandatory</td>
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
    <td>success</td>
    <td>true</td>
    <td></td>
  </tr>
</table>