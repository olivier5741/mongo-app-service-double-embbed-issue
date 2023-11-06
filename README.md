
https://github.com/olivier5741/mongo-app-service-double-embbed-issue/assets/3897291/07bcdb9a-b84d-4fdb-88af-d1e0738ff4c7


## GraphQL query

```graphql
{
  counters {
    _id
    description {
      short {
        markdown
      }
    }
    translations {
      en {
        name
      }
    }
    catalog {
      _id
      description {
        short {
          markdown
        }
      }
      translations {
        en {
          name
        }
      }
    }
  }
}
```

## Counter document

```json
{
  "_id": {
    "$oid": "653a6cba5be8146fac9ada3c"
  },
  "catalog": {
    "$oid": "653a6cde5be8146fac9ada40"
  },
  "translations": {
    "en": {
      "name": "The swamp counter"
    }
  },
  "description": {
    "short": {
      "markdown": "Un magasin *très* particulier"
    }
  }
}
```

## Catalog document

```json
{
  "_id": {
    "$oid": "653a6cde5be8146fac9ada40"
  },
  "translations": {
    "en": {
      "name": "Delicious vegetables and fruits"
    }
  },
  "description": {
    "short": {
      "markdown": "De délicieux fruits et légumes"
    }
  }
}
```

