--------------------------------
[Version]
--------------------------------
v1

■ Change logs
-----------


--------------------------------
[Overview]
--------------------------------
These code samples describe how to use PHP to call APIs.

--------------------------------
[Contents]
--------------------------------
conf/
  - api_config.ini      : Config files to specify IDs.

src/jp/co/yahoo/adsdisplayapi
  - sample/             : Examples of Report services.

--------------------------------
[Development environment]
--------------------------------
To construct PHP environment, install followings.

1. PHP 7.1.x or above
2. Composer 1.9.3 or above
3. OpenAPI generator 4.2.3 or above
4. Write Ids in conf/api_config.ini like this.
  - accountId          : API account ID (required)
  - accessToken        : API accessToken (required)

--------------------------------
[How to execute Sample Code]
--------------------------------
Move to the directory where you stored the cloned sample program, and execute OpenAPI Generator to generate a PHP client.
```
openapi-generator generate -i https://yahoojp-marketing.github.io/ads-display-api-documents/design/v1/Route.yaml -g php -o ./
```

Then, composer.json is generated immediately below, so execute client install.
```
composer install
```

Execution example
```
php ./src/jp/co/yahoo/adsdisplayapi/sample/ReportDefinitionServiceSample.php
```

--------------------------------
NOTICE：　Yahoo! Ads Display Ads API - For use of sample code
--------------------------------


The sample code of Yahoo! Ads API is provided to API users only who concluded the contract of "Application to Use Yahoo! Promotional Ads API" with Yahoo Japan Corporation.

Additionally, please note that Yahoo Japan Corporation may change the contents and the specification of the sample code, and may discontinue providing the sample code without any notice.
