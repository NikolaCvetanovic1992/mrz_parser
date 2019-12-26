# mrz_parser (Dart/Flutter) 
[![Build Status](https://travis-ci.org/olexale/mrz_parser.svg?branch=master)](https://travis-ci.org/olexale/mrz_parser) [![Coverage Status](https://coveralls.io/repos/github/olexale/mrz_parser/badge.svg?branch=master)](https://coveralls.io/github/olexale/mrz_parser?branch=master)

Parse MRZ (Machine Readable Zone) from identity documents. Heavily insipred by [QKMRZParser](https://github.com/Mattijah/QKMRZParser).

### Supported formats:
* TD1
* TD2
* TD3
* MRV-A
* MRV-B

## Usage

### Import the package
Add to `pubspec.yaml`
```yaml
dependencies:
    mrz_parser: ^1.0.0
```

### Parse MRZ
```dart
final mrz = <String>[
  'P<UTOERIKSSON<<ANNA<MARIA<<<<<<<<<<<<<<<<<<<',
  'L898902C36UTO7408122F1204159ZE184226B<<<<<10'
];

final result = MRZParser.parse(mrz);
```

For help getting started with Flutter, view our 
[online documentation](https://flutter.dev/docs), which offers tutorials, 
samples, guidance on mobile development, and a full API reference.

## Authors
* [Anna Domashych](https://github.com/foxanna/)
* [Oleksandr Leuschenko](https://github.com/olexale/)

## License
`mrz_parser` is released under a [MIT License](https://opensource.org/licenses/MIT). See `LICENSE` for details.