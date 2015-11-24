QuoteTool
==============
2015-11-24



Main utility to manipulate quotes.



There are two types of quotes:

 - single quote
 - double quote
 
A quoted string is a string wrapped with the same type of quote.
Those quotes must be non escaped.
The wrapped content must not contain non escaped quote of the same type.

We use [quote escaping modes](https://github.com/lingtalfi/universe/blob/master/planets/ConventionGuy/convention.quotesEscapingModes.eng.md)

All methods here use [php multi-bytes functions](http://php.net/manual/en/ref.mbstring.php) (mb_)
 
 



isQuotedString
-----------
2015-11-24


```php
bool        isQuotedString ( str:string, str:quoteType=null, bool:escapedRecursiveMode=true ) 
```

If quoteType is null (the default), both types of quotes are tested.



