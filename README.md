# FlagbitCurrencyBundle [![Build Status](https://travis-ci.org/Flagbit/FlagbitCurrencyBundle.svg?branch=master)](https://travis-ci.org/Flagbit/FlagbitCurrencyBundle)

## About

The FlagbitCurrencyBundle provides basic functions to display currency symbols and names.

## Configuration

You can set your default currency:

```yaml
fagbit_currency:
    default_currency: CHF
```

The bundle defaults to EUR.

## Services

```php
$container->get('flagbit_currency')->getDefaultCurrency(); // EUR
```

## Twig Functions

### currency_name

```twig
{{ currency_name() }} {# example output: Euro #}
{{ currency_name('EUR') }} {# example output: Euro #}
{{ currency_name('CHF') }} {# example output: Schweizer Franken #}
```

### curreny_symbol

```twig
{{ currency_symbol() }} {# example output: € #}
{{ currency_symbol('CHF') }} {# example output: CHF #}
{{ currency_symbol('EUR') }} {# example output: € #}
```
