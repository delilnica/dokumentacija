# Dokumentacija za Delilnico

Storitev je trenutno v nastajanju, a so nekateri API klici že na voljo.


## APIv1

Vsem končnim točkam dodaj predpono `/v1`.

- `/add` (POST) - dodaj nov fragment

  Zahtevani parametri:

  * `title` - naslov
  * `author` - pisec
  * `text` - besedilna vsebina
  * `is_private` - logična vrednost, ki naznanja zasebnost fragmenta

  Vrnjene vrednosti:

  * `id` - enolična oznaka fragmenta

- `/fragment/id` (GET) - pridobi obstoječ fragment

  Zahtevan parameter:

  * `id` - enolična oznaka fragmenta, pridobljena po dodajanju

- `/author/author` (GET) - pridobi vse javne fragmente podanega pisca

  Zahtevan parameter:

  * `author` - ime pisca

- `/all_fragments` (GET) - pridobi vse javne fragmente
