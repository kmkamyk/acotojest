Krótkie wyjaśnienie każdego z algorytmów i rozszerzeń protokołów używanych w SSH:

**Ciphers (algorytmy szyfrowania)**:
Szyfrują dane przesyłane przez sieć w celu ochrony przed nieautoryzowanym dostępem.

* **AES-256-GCM** to algorytm szyfrowania symetrycznego, który jest uważany za bardzo bezpieczny.
* **ChaCha20-Poly1305** to algorytm szyfrowania symetrycznego, który jest uważany za szybszy niż AES-256-GCM.
* **ECDH-ECDSA-AES256-GCM-SHA512** to zestaw algorytmów, które są używane do szyfrowania, uwierzytelniania i kompresji danych w SSH.

**Compression formats (formaty kompresji)**:

* **ZLIB** to popularny format kompresji danych, który jest używany w wielu aplikacjach.
* **LZ4** to nowszy format kompresji danych, który jest uważany za szybszy niż ZLIB.

**Hostkey formats (formaty kluczy hosta)**:

* **RSA** to algorytm szyfrowania asymetrycznego, który jest używany do uwierzytelniania serwerów.
* **DSA** to algorytm szyfrowania asymetrycznego, który jest uważany za mniej bezpieczny niż RSA.
* **ECDSA** to algorytm szyfrowania asymetrycznego, który jest uważany za bezpieczniejszy niż RSA i DSA.

**Key exchange protocols (protokoły wymiany kluczy)**:

* **Diffie-Hellman** to protokół wymiany kluczy, który jest używany do wymiany kluczy szyfrowania między dwoma stronami.
* **ECDH** to nowszy protokół wymiany kluczy, który jest uważany za bezpieczniejszy niż Diffie-Hellman.

**Message authentication codes (MACs)** (kody uwierzytelniania wiadomości):

* **HMAC-SHA256** to kod uwierzytelniania wiadomości, który jest używany do weryfikacji integralności danych.
* **HMAC-SHA512** to kod uwierzytelniania wiadomości, który jest uważany za bardziej bezpieczny niż HMAC-SHA256.

**User authentication methods (metody uwierzytelniania użytkowników)**:

* **gssapi-keyex** to metoda uwierzytelniania, która wykorzystuje GSSAPI (Generic Security Services Application Program Interface) do wymiany kluczy szyfrowania między klientem i serwerem.
* **gssapi-with-mic** to metoda uwierzytelniania, która wykorzystuje GSSAPI do wymiany kluczy szyfrowania i generowania kodu uwierzytelniania wiadomości (MAC).
* **hostbased** to metoda uwierzytelniania, która wykorzystuje nazwę hosta klienta do uwierzytelnienia klienta.
* **keyboard-interactive** to metoda uwierzytelniania, która wymaga od użytkownika podania dodatkowych informacji, takich jak hasła jednorazowe (TOTP) lub odpowiedzi na pytania bezpieczeństwa.
* **password** to metoda uwierzytelniania, która wymaga od użytkownika podania hasła.
* **publickey** to metoda uwierzytelniania, która wykorzystuje parę kluczy SSH (klucz publiczny i klucz prywatny) do uwierzytelnienia klienta.

**Protocol extensions (rozszerzenia protokołów)**:

* **delay-compression** to rozszerzenie protokołu, które umożliwia opóźnienie kompresji danych przesyłanych przez SSH.
* **elevation** to rozszerzenie protokołu, które umożliwia klientowi żądanie podniesienia uprawnień na serwerze.
* **ext-auth-info** to rozszerzenie protokołu, które umożliwia serwerowi przekazywanie dodatkowych informacji o uwierzytelnianiu do klienta.
* **global-requests-ok** to rozszerzenie protokołu, które umożliwia klientowi wysyłanie żądań globalnych do serwera.
* **no-flow-control** to rozszerzenie protokołu, które wyłącza kontrolę przepływu danych między klientem i serwerem.
* **server-sig-algs** to rozszerzenie protokołu, które umożliwia klientowi negocjować algorytmy podpisu serwera z serwerem.
