# JSON-LD cheat sheet

## Different attribute, same URI

The first JSON-LD uses `name` as attribute, while the second JSON-LD uses `test`.
Semantically, they mean the same because the URIs of `name` and `test` are the same.

```json
{
  "@context": {
    "@vocab": "http://schema.org/",
    "name": "http://example.com/name"
  },
  "@type": "Person",
  "name": "Jane Doe"
}
```
```json
{
  "@context": {
    "@vocab": "http://schema.org/",
    "test": "http://example.com/name"
  },
  "@type": "Person",
  "test": "Jane Doe"
}
```

## Order in array doesn't change semantics

The order in the array of `jobTitle` is different between the first and second JSON-LD.
Semantically, they mean the same because the order in an array has no meaning.

```json
{
  "@context": {
    "@vocab": "http://schema.org/"
  },
  "@type": "Person",
  "name": "Jane Doe",
  "jobTitle": ["Professor", "Dr."]
}
```

```json
{
  "@context": {
    "@vocab": "http://schema.org/"
  },
  "@type": "Person",
  "name": "Jane Doe",
  "jobTitle": ["Dr.","Professor"]
}
```

## Array with one element is same as just that element

The first JSON-LD has an array with one element `"Professor"` for the attribute `jobTitle`.
The second JSON-LD has no array but directly the element.
Semantically, they mean the same.

```json
{
  "@context": {
    "@vocab": "http://schema.org/"
  },
  "@type": "Person",
  "name": "Jane Doe",
  "jobTitle": ["Professor"]
}
```

```json
{
  "@context": {
    "@vocab": "http://schema.org/"
  },
  "@type": "Person",
  "name": "Jane Doe",
  "jobTitle": "Professor"
}
```
