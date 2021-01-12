# Reason-ReScript-Cheatsheet

## Convert Script

```bash
./node_modules/.bin/bsc -format <path_to_reason_file>/<name>.re > <path_to_rescript_file>/<name>.res
```

## PPX

### Single-line String

#### Reason
```re
[%tw "w-full text-sm"]
```

#### ReScript
```res
%tw("w-full text-sm")
```

### Multi-line String
#### Reason
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

#### ReScript
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