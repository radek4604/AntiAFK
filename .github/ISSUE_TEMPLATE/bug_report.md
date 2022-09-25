name: Zgłaszanie błędu | radziuDevelopment
description: Zgłoś nam twój błąd dotyczący programu AntiAFK
labels: ["BŁĄD"]
body:
  - type: checkboxes
    id: searched
    attributes:
      label: Zasady
      options:
        - label: "Używam najnowszej wersji programu i nie ma żadnej dostępnej aktualizacji."
          required: true
  - type: input
    id: discord_tag
    attributes:
      label: Twój discord tag (opcjonalne)
      description: Jak możemy się z Tobą skontaktować?
      placeholder: np. DiscordTag#0001
    validations:
      required: false
  - type: textarea
    id: what-happened
    attributes:
      label: Co się stało?
      description: Krótki opis co się stało podczas używania programu.
      placeholder: Powiedz nam co widzisz!
      placeholder: "np. Przy uruchamianiu AntiAFK program zcrashował!"
    validations:
      required: true
  - type: textarea
    id: steps
    attributes:
      label: Co trzeba zrobić aby wygenerować ten sam błąd
      description: Opisz nam, jak możemy uzyskać ten sam błąd?
      placeholder: |
        1. Wejdź w '...'
        2. Kliknij w '....'
        3. Zjedź w dół na '....'
        4. Zobacz błąd
    validations:
      required: true
  - type: dropdown
    id: server_version
    attributes:
      label: Wersja klienta
      description: "Wybierz wersja swojego klienta"
      options:
        - 1.0
  - type: dropdown
    id: game_name
    attributes:
      label: Gra
      description: "Wybierz w której grze występuję błąd."
      options:
        - VALORANT
        - CS:GO
        - Roblox
  - type: dropdown
    id: isThatProb
    attributes:
      label: Czy ten problem występuje tylko w tej grze?
      description: "Potrzebujemy tej informacji w celu zweryfikowania czy to błąd gry czy może błąd po naszej stronie."
      options:
        - Tak, błąd występuje tylko w tej grze!
        - Nie, niestety ale błąd występuję w każdej grze.
  - type: textarea
    id: screenshots
    attributes:
      label: Screenshoty / Filmy
      description: Wklej screenshot aby pomóc nam w rozwiązaniu Twojego problemu.
  - type: markdown
    attributes:
      value: |
        ## Dziękujemy za wypełnienie formularza błędu.
