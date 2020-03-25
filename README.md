zz-curl
=======

> ZZ bindings for libcurl

## Status

> **WIP**

## Installation

> [Still trying to figure that out](https://github.com/aep/zz/issues/34)

## Usage

```c++
using zz_curl as curl

fn main() -> int {
  new request = curl::easy::init();

  request.setopt(curl::options::URL, "https://github.com");

  if curl::OK != request.perform() {
    printf("%s\n", request.error_string());
  }

  request.cleanup();
  return 0;
}
```

## License

MIT
