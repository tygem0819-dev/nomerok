# nomerOK — сборка APK и EXE

1. Создай пустой репозиторий на github.com (например, nomerok).
2. В папке с этим проектом выполни:
   git init
   git add .
   git commit -m "nomerOK"
   git branch -M main
   git remote add origin https://github.com/ТВОЙ_НИК/nomerok.git
   git push -u origin main
   (скрытая папка .github должна попасть в репозиторий)
3. На GitHub открой вкладку Actions → Build nomerOK → Run workflow.
4. Через 5–10 минут внутри запуска, внизу, в Artifacts появятся:
   - nomerOK-windows-exe (portable .exe для ПК)
   - nomerOK-android-apk (nomerOK.apk для телефона)
5. Чтобы файлы были доступны всем по ссылке: создай тег, и сборка сама прикрепит их к Release:
   git tag v1.0.0 && git push origin v1.0.0
   Скачать можно будет на странице Releases.

Локально: npm install, затем npm start (окно игры) или npm run dist:win (на Windows).
