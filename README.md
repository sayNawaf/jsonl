# jsonl

The JSONL Converter Library is a Python library designed to facilitate the conversion of various file formats to the JSON Lines (JSONL) format. JSONL is a format where each line of the file represents a valid JSON object, making it easy to read, write, and process large datasets.

Supported File Formats:

1.CSV
2.JSONL
3.Pandas DataFrame
4.Excel (xls, xlsx)
5.Avro
6.Parquet
7.ORC
8.Feather
9.XML
10.YAML
11.JSON
12.Msgpack
13.SQLite
14.HDF5

# Sample Code

from jsonl import jsonl

csv_file = "input.csv"
jsonl_obj = jsonl.csv_to_jsonl(csv_file) \# Convert CSV to JSONL

jsonl_obj.save_jsonl("output.jsonl") \# Save JSONL to file



# Conversion to jsonl object

| Function                                         | Purpose                                              | Supported Formats        |
| ------------------------------------------------ | ---------------------------------------------------- | ------------------------ |
| `csv_to_jsonl(input_csv_file) -> jsonl_object`    | Convert CSV to JSONL                                 | CSV                      |
| `read_jsonl(input_file_name) -> jsonl_object`     | Read JSONL file and return JSONL object              | JSONL                    |
| `dataframe_to_jsonl(df) -> jsonl_object`          | Convert Pandas DataFrame to JSONL object             | Pandas DataFrame         |
| `xl_to_jsonl(input_excel_file, sheet_name=0) -> jsonl_object` | Convert Excel to JSONL                | Excel (xls, xlsx)        |
| `avro_to_jsonl(input_avro_file) -> jsonl_object`  | Convert Avro to JSONL                                | Avro                     |
| `parquet_to_jsonl(input_parquet_file) -> jsonl_object` | Convert Parquet to JSONL                       | Parquet                  |
| `orc_to_jsonl(input_orc_file) -> jsonl_object`    | Convert ORC to JSONL                                 | ORC                      |
| `feather_to_jsonl(input_feather_file) -> jsonl_object` | Convert Feather to JSONL                       | Feather                  |
| `xml_to_jsonl(input_xml_file) -> jsonl_object`    | Convert XML to JSONL                                 | XML                      |
| `yaml_to_jsonl(input_yaml_file) -> jsonl_object`  | Convert YAML to JSONL                                | YAML                     |
| `json_to_jsonl(input_json_file) -> jsonl_object`  | Convert JSON to JSONL                                | JSON                     |
| `msgpack_to_jsonl(input_msgpack_file) -> jsonl_object` | Convert Msgpack to JSONL               | Msgpack                  |
| `sqlite_to_jsonl(input_sqlite_file, table_name='data') -> jsonl_object` | Convert SQLite to JSONL        | SQLite                   |
| `hdf5_to_jsonl(input_hdf5_file, key='data') -> jsonl_object` | Convert HDF5 to JSONL                          | HDF5                     |



# jsonl object to other file format

| Function                                                  | Purpose                                               | Supported Formats          |
| --------------------------------------------------------- | ----------------------------------------------------- | -------------------------- |
| `jsonl_object.save_jsonl(output_file_name)`                | Saves the JSONL object to a JSONL file.              | JSONL                      |
| `jsonl_object.to_csv(output_csv_file)`                     | Converts the JSONL object to a CSV file.             | CSV                        |
| `jsonl_object.to_xl(output_xlsx_file)`                     | Converts the JSONL object to an Excel file.          | Excel (xls, xlsx)          |
| `jsonl_object.to_dataframe()`                               | Returns a Pandas DataFrame from the JSONL object.    | Pandas DataFrame           |
| `jsonl_object.to_orc(output_orc_file)`                     | Converts the JSONL object to an ORC file.            | ORC                        |
| `jsonl_object.to_hdf5(output_hdf5_file)`                   | Converts the JSONL object to an HDF5 file.           | HDF5                       |
| `jsonl_object.to_parquet(output_parquet_file)`             | Converts the JSONL object to a Parquet file.         | Parquet                    |
| `jsonl_object.to_avro(output_avro_file)`                   | Converts the JSONL object to an Avro file.           | Avro                       |
| `jsonl_object.to_xml(output_xml_file)`                     | Converts the JSONL object to an XML file.            | XML                        |
| `jsonl_object.to_yaml(output_yaml_file)`                   | Converts the JSONL object to a YAML file.           | YAML                       |
| `jsonl_object.to_json(output_json_file)`                   | Converts the JSONL object to a JSON file.           | JSON                       |
| `jsonl_object.to_feather(output_feather_file)`             | Converts the JSONL object to a Feather file.        | Feather                    |
| `jsonl_object.to_sqlite(output_sqlite_file, table_name='data')` | Converts the JSONL object to a SQLite file.   | SQLite                     |
| `jsonl_object.to_msgpack(output_msgpack_file)`             | Converts the JSONL object to a Msgpack file.         | Msgpack                    |


