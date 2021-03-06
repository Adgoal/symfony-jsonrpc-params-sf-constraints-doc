# Symfony JSON-RPC params documentation
[![License](https://img.shields.io/github/license/adgoal/symfony-jsonrpc-params-sf-constraints-doc.svg)](https://github.com/adgoal/symfony-jsonrpc-params-sf-constraints-doc) [![Code size](https://img.shields.io/github/languages/code-size/adgoal/symfony-jsonrpc-params-sf-constraints-doc.svg)](https://github.com/adgoal/symfony-jsonrpc-params-sf-constraints-doc) [![Dependabot Status](https://api.dependabot.com/badges/status?host=github&repo=adgoal/symfony-jsonrpc-params-sf-constraints-doc)](https://dependabot.com)

[![Scrutinizer Build Status](https://img.shields.io/scrutinizer/build/g/adgoal/symfony-jsonrpc-params-sf-constraints-doc.svg?label=Scrutinizer&logo=scrutinizer)](https://scrutinizer-ci.com/g/adgoal/symfony-jsonrpc-params-sf-constraints-doc/build-status/master) [![Scrutinizer Code Quality](https://img.shields.io/scrutinizer/g/adgoal/symfony-jsonrpc-params-sf-constraints-doc/master.svg?logo=scrutinizer)](https://scrutinizer-ci.com/g/adgoal/symfony-jsonrpc-params-sf-constraints-doc/?branch=master) [![Code Coverage](https://img.shields.io/scrutinizer/coverage/g/adgoal/symfony-jsonrpc-params-sf-constraints-doc/master.svg?logo=scrutinizer)](https://scrutinizer-ci.com/g/adgoal/symfony-jsonrpc-params-sf-constraints-doc/?branch=master)

[![Travis Build Status](https://img.shields.io/travis/com/adgoal/symfony-jsonrpc-params-sf-constraints-doc/master.svg?label=Travis&logo=travis)](https://travis-ci.com/adgoal/symfony-jsonrpc-params-sf-constraints-doc) <!-- NOT WORKING WITH travis-ci.com [![Travis PHP versions](https://img.shields.io/travis/php-v/adgoal/symfony-jsonrpc-params-sf-constraints-doc.svg?logo=travis)](https://php.net/) --> [![Travis Symfony Versions](https://img.shields.io/badge/Symfony-v3%20%2F%20v4-8892BF.svg?logo=travis)](https://symfony.com/)

[![Latest Stable Version](https://img.shields.io/packagist/v/adgoal/symfony-jsonrpc-params-sf-constraints-doc.svg)](https://packagist.org/packages/adgoal/symfony-jsonrpc-params-sf-constraints-doc) [![Packagist PHP version](https://img.shields.io/packagist/php-v/adgoal/symfony-jsonrpc-params-sf-constraints-doc.svg)](https://packagist.org/packages/adgoal/symfony-jsonrpc-params-sf-constraints-doc)

Symfony bundle for easy Symfony constraints to JSON-RPC documentation transformation

Symfony bundle for [adgoal/jsonrpc-params-symfony-constraint-doc-sdk](https://github.com/adgoal/php-jsonrpc-params-symfony-constraint-doc-sdk)

## How to use

Once configured, your project will automatically create documentation for JSON-RPC params

See below how to configure it.

## Configuration

[Behat demo app configuration folders](./features/demo_app) can be used as examples.

 - Add the bundles in your config/bundles.php file:
   ```php
   // config/bundles.php
   return [
       ...
       Symfony\Bundle\FrameworkBundle\FrameworkBundle::class => ['all' => true],
       Yoanm\SymfonyJsonRpcHttpServer\JsonRpcHttpServerBundle::class => ['all' => true],
       Yoanm\SymfonyJsonRpcHttpServerDoc\JsonRpcHttpServerDocBundle::class => ['all' => true],
       Yoanm\SymfonyJsonRpcParamsSfConstraintsDoc\JsonRpcParamsSfConstraintsDocBundle::class => ['all' => true],
       ...
   ];
   ```
   
 - Configure `adgoal/symfony-jsonrpc-http-server` as described on [adgoal/symfony-jsonrpc-http-server](https://github.com/adgoal/symfony-jsonrpc-http-server) documentation.
 
 - Configure `adgoal/symfony-jsonrpc-http-server-doc` as described on [adgoal/symfony-jsonrpc-http-server-doc](https://github.com/adgoal/symfony-jsonrpc-http-server-doc) documentation.
 
 - Query your project at documentation endpoint and you should see JSON-RPC params documentation for each methods

   

## Contributing
See [contributing note](./CONTRIBUTING.md)
