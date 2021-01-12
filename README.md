# Reason-ReScript-Cheatsheet

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