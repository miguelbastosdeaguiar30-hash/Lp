LAST PATTERN — projeto Android pronto para abrir no Android Studio

O que foi preparado:
- O seu index.html original foi colocado em app/src/main/assets/index.html.
- O projeto usa uma WebView Android para abrir o jogo localmente, sem precisar hospedar o HTML.
- JavaScript e armazenamento local estão habilitados para o jogo e seu progresso.
- A tela fica em modo paisagem e tela cheia.

COMO GERAR O APK
1. Extraia o ZIP em uma pasta.
2. Instale o Android Studio (versão recente) e o Android SDK Platform 35.
3. No Android Studio, escolha Open e selecione a pasta LAST_PATTERN.
4. Aguarde a sincronização do Gradle. Se pedir para instalar componentes do SDK, aceite.
5. Para testar, conecte um celular com depuração USB ativada ou use um emulador e clique em Run.
6. Para gerar o APK: menu Build > Build Bundle(s) / APK(s) > Build APK(s).
7. Quando terminar, clique em Locate. Normalmente o APK fica em app/build/outputs/apk/debug/app-debug.apk.

PARA GERAR APK DE LANÇAMENTO
Use Build > Generate Signed Bundle / APK e siga o assistente para criar uma chave de assinatura. Guarde essa chave com segurança.

OBSERVAÇÕES
- Este pacote contém o projeto-fonte para compilar; o APK binário não foi compilado aqui.
- O HTML original foi mantido, sem reescrever a lógica do jogo.
- O projeto está configurado para orientação horizontal. Se quiser jogar em pé, altere android:screenOrientation="landscape" no AndroidManifest.xml para "portrait".
- Se algum recurso do HTML tentar carregar conteúdo externo, ele dependerá da conexão e das permissões correspondentes. Os recursos embutidos no HTML continuam locais.
