# API V2.0 Endpoints

## Autenticate

~~~
https://theomx.com/api/2.0/authenticate
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
    <td>abc123</td>
    <td>Mandatory</td>
  </tr>
  <tr>
    <td>format</td>
    <td>json or xml</td>
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
    <td>abc123</td>
    <td></td>
  </tr>
  <tr>
    <td>format</td>
    <td>json</td>
    <td></td>
  </tr>
  <tr>
    <td>result.token</td>
    <td>abc123</td>
    <td></td>
  </tr>
    <tr>
    <td>result.expires_on</td>
    <td>2021-01-01T00:00:00.000-04:00</td>
    <td>One hour from time of query. GMT.</td>
  </tr>
</table>