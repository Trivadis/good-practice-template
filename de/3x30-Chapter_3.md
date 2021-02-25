# Good Practice Chapter 2

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem
Ipsum has been the industry's standard dummy text ever since the 1500s, when an
unknown printer took a galley of type and scrambled it to make a type specimen
book. It has survived not only five centuries, but also the leap into electronic
typesetting, remaining essentially unchanged. It was popularised in the 1960s
with the release of Letraset sheets containing Lorem Ipsum passages, and more
recently with desktop publishing software like Aldus PageMaker including
versions of Lorem Ipsum.

## G-1010: Never XYZ

### Reason

dd

### Justification

Reason for this is:

1. because 1=1
2. becasue 2=2

### Example (bad)

This is an SQL code block

```SQL
SELECT file_name FROM dba_data_files;
```

### Example (good)

This is an BASH code block

```BASH
if [ -z $TEST ]; then
    echo "\$TEST is empty"
else
    echo "\$TEST is defined"
fi
```

### Rating

| Priority | ​Impact  |
|----------|--------|
| high     | medium |
