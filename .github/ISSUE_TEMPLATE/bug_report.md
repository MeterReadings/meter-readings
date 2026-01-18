name: 🐞 Bug
title: "[BUG] Kurze Zusammenfassung"
description: Melde einen Fehler in der App „Zählerstände“
labels: ["bug", "to verify"]
assignees: []
body:
  - type: textarea
    id: description
    attributes:
      label: Beschreibung
      description: Beschreibe den Fehler möglichst genau. Du kannst auch Screenshots/Videos anhängen.
      placeholder: Was ist genau falsch?
    validations:
      required: true

  - type: textarea
    id: repro-steps
    attributes:
      label: Schritte zum Reproduzieren
      description: Liste alle Schritte auf, mit denen sich der Fehler nachstellen lässt.
      placeholder: |
        1. ...
        2. ...
        3. ...
    validations:
      required: true

  - type: dropdown
    id: platforms-affected
    attributes:
      label: Betroffene Plattform(en)
      description: Wähle alle Plattformen aus, auf denen der Fehler auftritt.
      multiple: true
      options:
        - Android
        - iOS
        - Konnte auf anderen Plattformen nicht testen
    validations:
      required: true

  - type: input
    id: app-version
    attributes:
      label: App-Version
      description: Zu finden in der App unter Einstellungen → App → Version (z. B. 3.2.209)
      placeholder: 3.2.209
    validations:
      required: true

  - type: input
    id: device
    attributes:
      label: Gerät / Modell
      description: z. B. „Pixel 7, Samsung S23, iPhone 14 …“
      placeholder: Gerät und Modell

  - type: textarea
    id: workaround
    attributes:
      label: Workaround
      description: Falls du einen vorübergehenden Workaround gefunden hast, beschreibe ihn hier.
      placeholder: Optional – falls vorhanden
