# Stripe Country Specs in JSON Format

Have you ever wanted to implement Stripe's 
[Required Verification Information](https://stripe.com/docs/connect/required-verification-information) guidelines for
Stripe Connect Custom? Sure, we've all been there at some point in our life.

This repository is a direct dump of the country spec for all supported countries, in JSON format.



Each folder in this repository represents a new update and is named by date.

Description of files:

File | Description
------------ | -------------
[default.json](2017-11-22/default.json) | A direct dump of all Country Spec objects in JSON format, untouched and pure.
[default-labeled.json](2017-11-22/default-labeled.json) | A direct dump of all Country Spec objects, plus an extra `label` attribute which indicates country name.
[required-fields.json](2017-11-22/required-fields.json) | A dump of only requirements - useful for building frontend components based on country requirements.

Each file has a `.min` version, in which the JSON has been minified but otherwise unchanged.

**Tip:** These JSON files are large. If you intend on serving them client-side, consider removing as much data as possible
to lower the total download size.

## Prefer a CSV File Dump?

The requirements page lists out the requirements in a nice table, and also offers a 
[CSV file](https://stripe.com/files/connect/Stripe_Connect_Custom_Identity_Verification.csv) as well.

## Prefer API Access?

The JSON dumps in this repository are grabbed directly from the Stripe API. You can do it too if you try hard enough:

[Country Specs API Docs](https://stripe.com/docs/api#country_specs)

## License

This repository is public domain, except for any license Stripe imposes on their data. Please refer to Stripe's terms if you
are concerned with licensing.