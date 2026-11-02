MINDHACK ANDROID — PROGETTO APK
================================

Questa è una vera struttura di progetto Android Studio (Java + WebView locale).
Include 50 livelli didattici:
- 1–10 BASE
- 11–20 MEDIUM
- 21–30 HARD
- 31–50 EXPERT (molto difficili, non impossibili)

La progressione salva livelli completati e XP nel localStorage della WebView.
Il terminale e i target sono simulati e non attaccano reti reali.

COME OTTENERE L'APK CON ANDROID STUDIO
1. Su un PC installa Android Studio.
2. Estrai questo ZIP.
3. Android Studio > Open > seleziona la cartella MINDHACK_Android.
4. Attendi la sincronizzazione Gradle e l'installazione dei componenti Android richiesti.
5. Menu Build > Build Bundle(s) / APK(s) > Build APK(s).
6. Il file sarà in app/build/outputs/apk/debug/app-debug.apk.
7. Copialo sul telefono Android e aprilo. Se richiesto, autorizza l'installazione da quella sorgente.

BUILD AUTOMATICO CON GITHUB ACTIONS
È incluso .github/workflows/build-apk.yml.
1. Crea un repository GitHub e carica il contenuto di questa cartella.
2. Apri la scheda Actions.
3. Avvia "Build MINDHACK APK" con Run workflow (oppure fai push su main).
4. Quando termina, scarica l'artifact "MINDHACK-APK".
5. Estrai l'artifact: contiene app-debug.apk.

IMPORTANTE
Non è stato possibile compilare qui il binario APK perché in questo ambiente non è installato l'Android SDK/Gradle.
Quindi questo ZIP è il progetto Android pronto per essere compilato, NON un APK già installabile.
L'APK debug è firmato automaticamente per installazione e test; per pubblicarlo su Play Store serve una release firmata con chiave dedicata.
