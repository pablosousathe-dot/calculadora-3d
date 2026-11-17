# Filtro de Corridas — controle de versões

Este ramo (`filtro-controle`) é lido pelo app para avisar sobre atualizações.

## Como lançar uma versão nova
1. Gere o APK novo (com `versionCode` maior) e substitua `apk/FiltroCorridas.apk`.
2. Em `controle.json`:
   - `versaoAtual`: número da versão nova → quem tiver versão menor recebe o aviso "Nova versão disponível".
   - `versaoMinima`: se aumentar, **todas as versões abaixo TRAVAM** até atualizar.
   - `mensagem`: texto que aparece no aviso.
   - `link`: onde baixar (já aponta para `apk/FiltroCorridas.apk` deste ramo).

Dá para editar o `controle.json` pelo próprio site do GitHub (ícone de lápis), até pelo celular.
