# Reason-ReScript-Cheatsheet

## Convert Script

```bash
./node_modules/.bin/bsc -format <path_to_reason_file>/<name>.re > <path_to_rescript_file>/<name>.res
```

## PPX

### Single-line String

```re
[%tw "w-full text-sm"]
```


```res
%tw("w-full text-sm")
```

### Multi-line String
```re
[%graphql {|
  query UserQuery {
    user {
      id
      name
    }
  }
|}];
```

```res
%graphql(`
  query UserQuery {
    user {
      id
      name
    }
  }
`)
```