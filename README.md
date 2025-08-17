# JSON File Viewer

### Objective
This project aims to test your knowledge of data structures and algorithms and use it to solve real-life problems.

### Problem
A software development company needs a tool to help visualize the structure of JSON files. This project requires checking and showing a JSON file, and then displaying two separate views:
- All unique keys found in the file,
- All values are found in the file.

### Features

- Read a JSON file.
- Validate that the file contains valid JSON.
- Extract and display:
  - All unique keys found in the JSON.
  - All values found in the JSON.
- If the file is invalid or the structure is not as expected, display a clear error message.

### Implementation

* Implement a function named `readFile` that reads the file and parses it as JSON.
* Implement a function named `extractKeys` that recursively traverses the JSON and returns a list of all unique keys.
* Implement a function named `extractValues` that recursively traverses the JSON and returns a list of all values.
* Display two views:
  - One for keys,
  - One for values.
* Show an error message if the file cannot be parsed or is not valid JSON.

### Test Case

1.
```json
{
  "user": {
    "name": "Alice",
    "age": 30
  },
  "active": true
}
```
Output
```
Keys: {user, name, age, active}
Values: {Alice, 30, true}
```

2.
```json
[
  { "id": 1, "score": 10 },
  { "id": 2, "score": 15 }
]
```
Output
```
Keys: {id, score}
Values: {1, 10, 2, 15}
```

3.
```json
{ "a": [1, {"b": 2}], "c": null }
```
Output
```
Keys: {a, b, c}
Values: {1, 2, null}
```

4.
```
`{"a": 1}`
```
Output
```
Error: Invalid JSON file.
```

### Qualification to pass
- [ ] The code should run successfully.
- [ ] Write all required functions for reading, validating, and extracting keys and values correctly.

