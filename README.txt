Huschel Speichermodul V1.0 – Pilot

1. In Supabase > Edge Functions > github-app-storage > Code den kompletten Inhalt von index.ts einsetzen und Deploy updates ausführen.
   Einstellung "Verify JWT with legacy secret" eingeschaltet lassen.
   Das Secret GITHUB_TOKEN bleibt unverändert in Supabase gespeichert.
2. index.html als separate Pilotseite über GitHub Pages (HTTPS) bereitstellen; bestehende Apps nicht ändern.
3. Supabase Publishable Key (sb_publishable_...) eingeben, mit huschka@eventdesign.com und bestehendem Passwort anmelden.
4. Zuerst "GitHub laden", dann Daten bearbeiten und "GitHub speichern".
5. Bei Speicherkonflikten zuerst JSON-Backup erstellen und erst dann neue GitHub-Daten laden.

Sicherheit: serverseitige App-Pfad-Whitelist, UID-Prüfung, kein Token im Browser, GitHub-SHA-Abgleich.
Grenzen: echte App-Datenintegration ist noch nicht erfolgt; dies ist eine separate, funktionsfähige Pilot-Oberfläche.
GitHub-Versionen/Commits sind kein unabhängiges Backup. JSON-Backup weiter verwenden.

Wichtig: Vor erstem GitHub-Laden kein Speichern möglich. Der erste erfolgreiche Schreibvorgang erstellt den App-Unterordner automatisch.
