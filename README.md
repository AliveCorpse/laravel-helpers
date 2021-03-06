# Laravel Helpers

- [Arrays](#arrays)
- [Database](#database)
- [Dev](#dev)
- [Forms](#forms)
- [Generic](#generic)
- [Math](#math)
- [Server](#server)
- [Strings](#strings)
- [Class](#class)

## Arrays

#### `array_has_wildcard()`

The `array_has_wildcard` is analogue of function `array_has` with ability to search with wildcard. Also it can search keys with dots (i.e. when you want to get some data from multiple field when validation is failed)

### `array_get_random()`

The `array_get_random` function returns random value instead key, how it makes the `array_rand`.

## Database

#### `compile_sql_query()`

The `compile_sql_query` function replaces all placeholders given bindings.

#### `get_all_tables()`

The `get_all_tables` function returns the list all tables with their columns.

#### `search_entire_database()`

The `search_entire_database` function searches entire database.

## Dev

#### `ddq()`

The `ddq` is analogue of function `dd`, but uses only for database queries.

#### `dump()`

The `dump` is analogue of function `dd`, but without stopping php executing script.

## Forms

#### `transform_form_element_key()`

The `transform_form_element_key` function for get the right name for the form element name. ["laravelcollective/html"](https://laravelcollective.com/docs/master/html) uses similar method called "transformKey". It helpful for `Illuminate\Support\MessageBag` when you want to get error from the multiple field, for example from multiple phones.

## Generic

#### `is_production_environment()`

The `is_production_environment` function checks whether the production environment is using.

#### `is_local_environment()`

The `is_local_environment` function checks whether the production local is using.

#### `get_size_types()`

The `get_size_types` function returns the list all available size types.

## Math

#### `calculate_percentage()`

The `calculate_percentage` function calculates percentages.

#### `float_has_remainder()`

The `float_has_remainder` function checks whether the remainder of the float is not zero.

#### `convert_bytes()`

The `convert_bytes` function converts bytes between any sizes.

## Server

#### `is_request_method_update()`

The `is_request_method_update` function checks whether the current request method is for updating.

#### `long_processes()`

The `long_processes` function sets the maximum value of the optimal configuration for the server to perform long operations.

#### `get_upload_max_filesize()`

The `get_upload_max_filesize` function returns the value of the `upload_max_filesize` from `php.ini` in any of the formats.

#### `get_post_max_size()`

The `get_post_max_size` function returns the value of the `post_max_size` from `php.ini` in any of the formats.

#### `is_max_post_size_exceeded()`

The `is_max_post_size_exceeded` function checks whether is the permissible size of the value `post_max_size` exceeded.

## Strings

#### `str_lower()`

The `str_lower` is function wrapper over `Str::lower`.

#### `str_ucwords()`

The `str_ucwords` function converts a value to studly caps case with spaces.

#### `strpos_array()`

The `strpos_array` is function wrapper over `strpos`. Added ability to pass `$needle` as an array.

## Class

### `get_class_constants()`

The `get_class_constants` function returns an array with all class constants.

### `get_class_constants_start_with()`

The `get_class_constants_start_with` function returns an array with constants which start with passed string.
