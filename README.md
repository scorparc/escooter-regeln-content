# E-Scooter Regeln – Content

Versionierter Regel-Content für die App **E-Scooter Regeln** („Darf ich hier fahren?").
Die App lädt Updates von diesem Repo (raw.githubusercontent.com) – Änderungen hier
erreichen alle installierten Apps **ohne App-Release**.

- `index.json` – Manifest: `contentVersion` (Apps übernehmen nur höhere Versionen) + Länderliste
- `countries/<code>.json` – ein Datensatz pro Land, Schema: `schema/escooter-rules.schema.json`
- Alle Texte mehrsprachig (de + en Pflicht)

**Pflege-Workflow:** siehe `docs/CONTENT_GUIDE.md` im (privaten) Projekt-Repo.
Kurzfassung: Länderdatei ändern → `lastUpdated` setzen → `contentVersion` in
`index.json` erhöhen → `tools/publish-content.ps1` ausführen.

**Hinweis:** Inhalte mit `"verified": false` sind redaktionelle Entwürfe und noch
nicht fachlich geprüft. Alle Angaben ohne Gewähr, keine Rechtsberatung.
