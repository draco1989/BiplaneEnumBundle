Changelog
=========

1.2.x
-----

 * Support JMSSerializerBundle of version 1.0;
 * [BC break] For using the custom handler for the serializer you should manually register
   your types of enumerations in the config.

1.1.1
-----

 * Fixed support PHP of version 5.3.5 and old;
 * Enhancements in the implementation of FlaggedEnum
   * Fixed determine of bit flags. Now, the zero value is will not be determined as a flag;
   * Added a constant `NONE` for the zero value;
   * [BC break] Constant with the zero value should not be returned in result from the `getPossibleValues` method;
   * Now there is no need to override `getBitmask` method;
   * Method `getMaskOfPossibleValues` marked as deprecated;
   * Make configurable a separator of flags for `ReadableFor` and `Readable` methods. By defaults `; `.

1.1.0
-----

 * Added `addFlags` and `removeFlags` methods to the `FlaggedEnum`;
 * Added support the Symfony of version 2.1;
 * Refactored the data transformers.

1.0.0
-----

Initial release.