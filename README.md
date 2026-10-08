# Minha Finança — APK Android 10+

Projeto Android da primeira versão funcional do **Minha Finança**.

## Compatibilidade
- Android 10 (API 29) ou superior
- `minSdk 29`
- `targetSdk 35`
- Java 17

## Gerar o APK sem Android Studio

O projeto já possui GitHub Actions. Você só precisa colocar esta pasta em um repositório GitHub.

1. Entre em https://github.com e faça login.
2. Crie um repositório novo, por exemplo `MinhaFinanca`.
3. No repositório, use **Add file → Upload files**.
4. Envie **todos os arquivos e pastas que estão dentro desta pasta `MinhaFinancaAndroid`**.
5. Faça o commit na branch `main`.
6. Abra a aba **Actions**.
7. Selecione **Build APK**.
8. Clique em **Run workflow**.
9. Quando terminar, abra a execução concluída.
10. Em **Artifacts**, baixe `MinhaFinanca-Android10-plus`.
11. Extraia o ZIP e instale `app-debug.apk` no celular.

O workflow instala automaticamente o Android SDK 35 e compila o APK.

## Teste pelo celular

O APK é uma versão de teste (`debug`). Ao instalar, o Android pode solicitar autorização para instalar aplicativos dessa fonte. Isso é normal para um APK fora da Play Store.

## Estrutura
- `app/src/main/assets/index.html`: interface e lógica do aplicativo.
- `MainActivity.java`: tela Android que abre o aplicativo.
- `.github/workflows/build-apk.yml`: compilação automática.
- `minSdk 29`: Android 10+.
