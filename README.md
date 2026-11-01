# Era UUID (`github.com/era-lang-official/uuid`)

RFC 4122 UUID v4 (random) and UUID v7 (time-ordered) generators and validators for Era.

## Features
- **UUID v4**: Cryptographically-seeded pseudo-random UUID generator.
- **UUID v7**: Time-ordered 48-bit millisecond timestamp + random payload.
- **Validation**: Strict RFC 4122 string format checker.

## Usage
```era
import "github.com/era-lang-official/uuid";

fn main() {
    let id = uuid_v4();
    println(id); // "xxxxxxxx-xxxx-4xxx-yxxx-xxxxxxxxxxxx"
    assert(is_valid_uuid(id));
}
```

