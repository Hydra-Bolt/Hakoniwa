
# Hakoniwa Class

The `Hakoniwa` class is a Python class designed to handle JSON data stored in a file. It provides methods to parse JSON, search for specific records, insert new records, and update existing records.

## Usage

To use the `Hakoniwa` class, follow these steps:

1. Import the `Hakoniwa` class into your Python script:

```python
from hakoniwa import Hakoniwa
```

2. Create an instance of the `Hakoniwa` class by providing the filename of the JSON file:

```python
hakoniwa = Hakoniwa("data.json")
```

3. Parse the JSON file using the `parseJSON` method:

```python
hakoniwa.parseJSON("data.json")
```

4. Find records that match specific criteria using the `find` method:

```python
matching_records = hakoniwa.find({"key": "value"})
```

5. Insert a new record using the `insert` method:

```python
hakoniwa.insert({"key": "value"})
```

6. Update existing records that match specific criteria using the `update_insert` method:

```python
hakoniwa.update_insert({"key": "value"}, {"new_key": "new_value"})
```

## Class Methods

### `parseJSON(file)`

Static method that parses a JSON file and returns the parsed data as a list of dictionaries.

Parameters:
- `file` (str): The path to the JSON file.

### `find(dict_find)`

Finds records in the parsed JSON data that match the specified criteria.

Parameters:
- `dict_find` (dict): A dictionary containing key-value pairs to match against the records.

Returns:
- A list of dictionaries representing the matched records.

### `insert(dict_update)`

Inserts a new record into the parsed JSON data.

Parameters:
- `dict_update` (dict): A dictionary representing the new record to be inserted.

### `updateDB()`

Updates the JSON file with the current data records.

### `update_insert(dict_find, dict_insert)`

Updates existing records that match the specified criteria with the new values provided.

Parameters:
- `dict_find` (dict): A dictionary containing key-value pairs to match against the records.
- `dict_insert` (dict): A dictionary representing the new values to be inserted into the matching records.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! If you encounter any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request.

## Authors

- [Muneeb Ahmed](https://github.com/Hydra-Bolt/) - Creator

## Acknowledgements

- [PyMongo](https://github.com/mongodb/mongo-python-driver) - Inspiration or code snippets


```

Make sure to replace `"data.json"` with the actual filename of your JSON data file.


<details>
<summary>Click to Reveal Easter Egg</summary>

Hakoniwa means Box-Garden it is known as pocket dimension for storage

</details>
