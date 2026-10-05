# Nota Clara

Protótipo Flutter para fotografar ou selecionar uma nota fiscal e visualizar um resumo estruturado da análise.

## Executar no Android Studio

1. Instale o Android Studio com `Android SDK`, `Android SDK Platform-Tools` e uma imagem de sistema pelo SDK Manager.
2. Abra `Device Manager`, crie um dispositivo virtual e inicie-o.
3. Na raiz do projeto, execute:

```bash
flutter doctor --android-licenses
flutter devices
flutter run
```

O fluxo permite escolher uma imagem da galeria ou abrir a câmera. O serviço em `lib/main.dart` usa uma resposta simulada de IA para o protótipo; a classe `InvoiceAiService` é o ponto de troca para uma API própria, Gemini, OpenAI ou outro provedor. A chave deve ficar em um backend, nunca no APK.

## Validação

```bash
flutter analyze
flutter test
```
