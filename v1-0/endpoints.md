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
