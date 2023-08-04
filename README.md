Correios Rastreio é uma biblioteca pra facilitar o rastreamento de pacotes nos correios, ela utiliza o site https://suareceita.net/

## Usage

Simples exemplo:

```dart
import 'package:rastrear_correios/rastrear_correios.dart';

void main() async {
  var correios = CorreiosRastreio();
  final events = await correios.rastrearEncomenda('AB12345678912BR');
  print(events[0].data);
  print(events[0].hora);
  print(events[0].destino);
  print(events[0].status);
  print(events[0].origem);
  print(events[0].local);
}

```

## Features

Quaisquer dúvidas ou erro criar issue no github.
