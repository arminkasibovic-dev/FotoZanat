# PhotoCraft

**Uređivanje slika; open-source implementacija Adobe Photoshopa razvijena od nule, u čistom Rustu.**

Slojevi, maske, slojevi za prilagođavanje, stilovi slojeva, tekst, vektori, četkice i stvarne PSD datoteke — u izvornoj aplikaciji napisanoj u potpunosti u Rustu. Otvorenog koda, radi offline i pripada vama.

[PhotoCraft na getartcraft.com](https://getartcraft.com/) · [ArtCraft](https://getartcraft.com/) · Sve aplikacije Crafting Apps

> ArtCraft je zajednica umjetnika iz svih životnih sredina. Digitalna umjetnost, generativna umjetnost, muzika, igre — ako nešto stvarate, dio ste naše zajednice. [Pridružite nam se na Discordu](https://discord.gg/artcraft).

## 🎛️ Dizajn koji je odmah poznat

Meniji, prečice, paneli i alati nalaze se tamo gdje ih očekujete — od `⌘J` do `⇧⌘D`. Ako poznajete Photoshop, već poznajete i PhotoCraft.

## ⚡ Izvorna aplikacija, velika brzina

GPU kompozitor zasnovan na `wgpu` (Metal, Vulkan, DX12, WebGPU), pločice uz kopiranje pri izmjeni i višedretveni filteri. Nema Electrona, nema web-prikaza i nema čekanja.

## 🗂️ Prave PSD datoteke

Otvarajte, uređujte i čuvajte slojevite Photoshop dokumente. Nakon ponovnog čuvanja, prikaz ostaje jednak za 307 od 309 testnih datoteka iz skupa `psd-tools`.

## 🤖 Spremno za agente

Svaka radnja je komanda, pa isti mehanizam možete koristiti kroz korisničko sučelje, CLI, JSON kontrolni kanal ili MCP server.

# Funkcije

Sve snimke ekrana prikazuju stvarnu aplikaciju u radu s umjetničkim djelima iz javnog domena, renderovanim preko kontrolnog kanala.

### Uređujte bez straha od greške

Slojevi za prilagođavanje čuvaju svaku izmjenu kao aktivnu i promjenjivu. Slažite Levels, Curves, Vibrance, Hue/Saturation i mnoge druge, primjenjujte ih na određena područja pomoću maski, mijenjajte njihov redoslijed ili ih isključujte — izvorni pikseli se nikad ne mijenjaju.

**16 slojeva za prilagođavanje** može se primijeniti i direktno na piksele. Uključuju Curves s uređivanjem pojedinačnih kanala, Levels s histogramom uživo, Black & White, Channel Mixer, Gradient Map, Photo Filter, Selective Color i Color Lookup (`.cube`, `.3dl`, `.look`), kao i Shadows/Highlights, Replace Color, Match Color, HDR Toning, Desaturate i Equalize.

### Stilovi koji poboljšavaju sliku

Drop Shadow, Inner Shadow, Outer i Inner Glow, Bevel & Emboss, Satin, Stroke te Color, Gradient i Pattern Overlay rade uživo na svakom sloju, uključujući tekst.

Uzorci dolaze iz biblioteke: ugrađeni uzorci, **Edit › Define Pattern**, uvoz i izvoz `.pat` datoteka te PSD `Patt` blokovi.

Kopirajte stilove između slojeva, sakrijte sve efekte odjednom i otvarajte stilove direktno iz PSD datoteka. Prikaz je usklađen s Photoshopom.

### Selekcije koje razumiju sliku

Pravougaoni i eliptični odabir, laso i Magic Wand omogućavaju precizan rad; Quick Selection, Object Selection i Select Subject automatizuju izdvajanje objekata; Select and Mask služi za fino podešavanje rubova, čak i oko pojedinačnih vlasi kose.

Omekšajte rubove, proširite ili smanjite selekciju, zagladite je, dodajte područja ili je ponovo učitajte. Svaku selekciju možete pretvoriti u masku sloja, vektorsku putanju ili oblik. Pametna selekcija radi lokalno na vašem računaru, bez oblaka i korisničkog računa.

### Tekst koji izgleda profesionalno

Tačkasti i pasusni tekst uređuju se direktno na platnu, uz potpune kontrole Character i Paragraph: font, debljina, veličina, prored, razmak između znakova, poravnanje i boja.

**Type Color Picker** podržava i uzorkovanje boje s ekrana pomoću povećala piksela. Tekstualni slojevi ostaju uređivi, mogu koristiti stilove slojeva i zadržavaju uređivost pri razmjeni PSD datoteka.

### Vektori precizni do piksela

Alati Rectangle, Ellipse, Triangle, Polygon, Line, Pen, Freeform Pen i Curvature Pen stvaraju slojeve oblika nezavisne od rezolucije, s gradijentnim ispunama i isprekidanim ili poravnatim potezima.

Kombinujte oblike (sjedini, oduzmi, presjek, isključi), čuvajte putanje u panelu Paths, koristite ih kao vektorske maske ili ih ocrtavajte i ispunjavajte. Svih 116 od 116 slojeva oblika u našem PSD skupu odgovara Photoshopovim pikselima.

### Pregled prije primjene

Svaki dijalog filtera prikazuje rezultat uživo na platnu, ograničen vašom selekcijom. Dostupni su zamućenja (Gaussian, Box, Motion, Radial, Surface, Smart, Lens, Shape i Blur Gallery: Tilt-Shift, Iris, Field, Spin, Path), izoštravanje, Reduce Noise, izobličenja (Twirl, Wave, Ripple, Displace, Shear, Zig Zag…), Pixelate, Stylize (Oil Paint, Wind, Extrude…), Render (Clouds, Fibers, Lens Flare, Lighting Effects) i još mnogo toga.

Filteri primijenjeni na pametni objekat ostaju uređivi: kasnije ih možete mijenjati, sakriti, presložiti ili maskirati.

Zamućenja velikog radijusa koriste prolaze s kumulativnim zbirom kroz sve procesorske jezgre: Gaussian zamućenje radijusa 180 na slici od 3,6 megapiksela traje manje od sekunde.

### Oblikujte sliku kako želite

Free Transform podržava promjenu veličine, rotaciju, iskrivljavanje, deformaciju i perspektivu, tačne rotacije od 90° i 180°, okretanje te ponavljanje prethodne transformacije. Slojevi, tekst, oblici, maske i selekcije transformišu se zajedno.

Historija, Toggle Last State i History Brush omogućavaju poništavanje svakog koraka, čak i pojedinačnog poteza četkicom.

### Izvezite u željenom formatu

Export As nudi izbor formata, kvaliteta, prozirnosti i skale, uz pregled i trenutnu procjenu veličine datoteke. Quick Export omogućava izvoz u PNG jednim klikom.

Izaberite tamnu Pro temu, prozračne Studio teme ili klasični izgled.

# Sve što vam treba

## 🧰 67 alata

Move · Artboard · Rectangular i Elliptical Marquee · Single Row Marquee · Single Column Marquee · Lasso · Polygonal Lasso · Magnetic Lasso · Object Selection · Quick Selection · Magic Wand · Crop · Perspective Crop · Slice · Slice Select · Frame · Eyedropper · Color Sampler · Ruler · Note · Count · Remove · Spot Healing Brush · Healing Brush · Patch · Content-Aware Move · Red Eye · Brush · Pencil · Mixer Brush · Color Replacement · Clone Stamp · Pattern Stamp · History Brush · Eraser · Background Eraser · Magic Eraser · Gradient · Paint Bucket · Blur · Sharpen · Smudge · Dodge · Burn · Sponge · Pen · Freeform Pen · Curvature Pen · Add Anchor Point · Delete Anchor Point · Convert Point · Horizontal i Vertical Type · Horizontal i Vertical Type Mask · Path Selection · Direct Selection · Rectangle · Ellipse · Triangle · Polygon · Line · Custom Shape · Hand · Rotate View · Zoom

## 🖌️ Pravi mehanizam četkica

Shape Dynamics, Scattering, Texture, Dual Brush, Color Dynamics, Transfer, Brush Pose, Wet Edges, Build-up i Smoothing (uključujući Pulled String), uz podršku za pritisak olovke, nagib, rotaciju i smjer. Dostupni su unaprijed podešeni profili četkica, Define Brush from Selection te deterministički potezi koji se mogu ponovo reprodukovati.

## 🗃️ Slojevi, urađeni kako treba

Grupe, clipping maske, pikselne i vektorske maske, slojevi ispune (puna boja, gradijent i uzorak), slojevi za prilagođavanje, aktivni pametni objekti s pametnim filterima te transformacije i deformacije bez gubitka kvaliteta. Tu su i višestruki odabir slojeva uz poravnanje, raspoređivanje i povezivanje, alfa-kanali i Quick Mask, 27 Photoshop načina stapanja plus šest varijanti iz Paint.NET-a, neprozirnost i ispuna, zaključavanje, oznake boja, filter prema vrsti sloja, spajanje, poravnanje slojeva, rasterizacija, Layer via Copy/Cut i Paste Into.

## 🎨 Svaka boja i dubina

RGB, Grayscale, CMYK i Lab dokumenti s 8, 16 ili 32 bita po kanalu. Dubina bita i model boja podaci su dostupni tokom rada, tako da svaki alat funkcioniše na svakoj dubini.

Upravljanje ICC bojama u čistom Rustu: ugrađeni profili, Assign i Convert to Profile sa sva četiri načina prikaza i kompenzacijom crne tačke, soft proofing (`⌘Y`) i Gamut Warning (`⇧⌘Y`) na GPU-u.

## 🗂️ Formati

PSD i PSB; slojeviti TIFF (podaci o Photoshop slojevima nalaze se u TIFF datoteci i čitaju se i zapisuju u oba redoslijeda bajtova); Paint.NET PDN3 (čitanje, s uređivim slojevima i svih 14 načina stapanja); OpenRaster (čitanje i pisanje slojeva, grupa i načina stapanja za Krita, MyPaint i GIMP); Krita `.kra` (čitanje slojeva za slikanje, grupa, načina stapanja i maski prozirnosti); SVG (otvara se kao slojevi oblika, a može se postaviti kao vektorski Smart Object).

Podržani su i ravni PNG, JPEG, TIFF, WebP (s gubitkom i bez njega), GIF, BMP, TGA, ICO, QOI, PNM, OpenEXR, Radiance HDR i FITS (astronomske slike: 8/16-bitne i 32-bitne vrijednosti s pomičnim zarezom, s očuvanim zaglavljem), kao i izvorni format `.pcraft`.

Ravni formati čuvaju dubinu koju podržavaju: PNG zadržava uzorke od 8/16 bita, TIFF uzorke od 8/16 bita i 32-bitne uzorke s pomičnim zarezom, a OpenEXR uzorke half/float. JPEG, WebP i ostali 8-bitni formati smanjuju uzorke veće dubine i prikazuju upozorenje pri izvozu. Za svaki format pogledajte [matricu mogućnosti kodeka](https://github.com/storytold/photocraft).

HEIC fotografije s iPhonea i Maca mogu se samo čitati (uključene su u zvanične verzije; za izgradnju iz izvornog koda dostupna je opcionalna funkcija `--features heif`). AVIF je dostupan samo za pisanje uz opcionalnu funkciju izgradnje `avif`; dekodiranje AVIF-a i JPEG XL nisu dostupni.

Affinity dokumenti (`.af`, `.afdesign`, `.afphoto`, `.afpub`) otvaraju se izvorno i samo za čitanje, uključujući artboarde, slojeve, vektore, tekst, slike i maske. Efekti, prilagođavanja i drugi nepodržani dijelovi navode se u upozorenju; izvoz u Affinity format nije dostupan.

## 🪄 Svakodnevni osnovni alati

Auto Tone, Contrast i Color · Equalize · Image i Canvas Size · Crop i Trim · Reveal All · Edit › Fill and Stroke · Copy Merged · Paste in Place · vodiči, lenjiri, mreža i poravnanje · snimanje i reprodukcija radnji · paleta komandi (`⌘F`).

# PSD bez kompromisa

PSD podrška za PhotoCraft samostalni je crate napisan prema javnoj Adobe specifikaciji i testiran na skupu stvarnih datoteka.

- **Vjerno ponovno otvaranje i čuvanje:** otvaranje i ponovno čuvanje dokumenta daje isti prikaz za 307 od 309 datoteka iz skupa `psd-tools` i 169 od 170 datoteka iz našeg kombinovanog skupa `ag-psd`/`psd-tools` (`crates/io/tests/corpus.rs`; skup `psd-tools` preuzmite komandom `cargo xtask corpus --psd-tools`). Podaci koje još ne modeliramo (raw blokovi, deskriptori, dodatni podaci) prenose se dalje umjesto da budu odbačeni. Ponovo sačuvana datoteka nije identična izvorniku bajt po bajt: PhotoCraft ponovo zapisuje slikovne resurse, zapise slojeva i kompozitnu sliku. Samo samostalni crate `photocraft-psd`, koji parsira i zapisuje datoteku bez modela dokumenta, reprodukuje svaku datoteku iz korpusa koja se može parsirati bajt po bajt (`crates/psd/tests/corpus.rs`).
- **Podudarni pikseli:** kompozitni referentni test poredi naš prikaz s objedinjenom slikom koju generiše Photoshop, uključujući interpolaciju gradijenata (Classic, Perceptual i Linear), efekte slojeva, poteze oblika, clipping i neprozirnost ispune.
- **Veliki dokumenti:** PSB, 16-bitne i 32-bitne datoteke te CMYK i Lab dokumenti otvaraju se izvorno.

# Napravljen za agente

Svaka stavka menija, alat i dijalog pokreće komandu iz jedinstvenog registra s više od 500 komandi. Korisničko sučelje, CLI, JSON kontrolni kanal i MCP server koriste iste komande, tako da sve što možete kliknuti možete uraditi i skriptom ili AI agentom.

## Rad bez grafičkog sučelja: otvori, uredi, sačuvaj

```bash
photocraft-cli run wave.psd \
  --cmd filter.sharpen.smartSharpen --params '{"amount":80}' \
  --cmd layer.newAdjustmentLayer.curves --params '{"points":[[0,0],[64,48],[192,212],[255,255]]}' \
  --out wave-final.png
```

## Primijeni isti skup radnji na mapu slika

```bash
photocraft-cli batch --actions grade.json --in ./raw --out ./graded
```

## Svaka podkomanda objašnjava svoju upotrebu

```bash
photocraft-cli batch --help
```

## Omogućite agentu upravljanje preko MCP-a

Radi bez grafičkog sučelja ili povezano s aplikacijom koja je već pokrenuta:

```bash
photocraft-cli mcp
```

Desktop aplikacija nudi i autentifikovani kontrolni kanal ograničen na lokalnu petlju (`photocraft --control`) za pregled stanja korisničkog sučelja, upravljanje alatima pomoću događaja pokazivača i snimanje ekrana van ekrana. Sve slike u ovom README-ju renderovane su na taj način. Pogledajte `docs/control-protocol.md`.

# Ispod haube

- **Prvo mehanizam:** model dokumenta zasnovan na podacima i mehanizam komandi, uz tanki egui sloj korisničkog sučelja. Razdvajanje slojeva provjerava se pri izgradnji kroz 24 cratea.
- **Dva kompozitora:** CPU kompozitor služi kao referenca, a `wgpu` kompozitor prikazuje platno na GPU-u. Testiraju se međusobno.
- **Pločice uz kopiranje pri izmjeni:** rijetke pločice veličine 256² čine poništavanje izmjena jeftinim i omogućavaju rad s ogromnim platnima; mape efekata keširaju se prema stanju sloja.
- **Radi u pregledniku:** cijeli mehanizam i korisničko sučelje mogu se kompajlirati u WebAssembly.
- **Clean-room implementacija:** izrađena samo na osnovu javnih specifikacija i posmatranog ponašanja. Nema vlasničkog koda, shadera ili resursa.
- **Testirano:** više od 1.700 testova, uključujući PSD round-trip testove, sintetičke generatore, kompozitorske referentne testove i provjere više dubina boja.

# Početak rada

```bash
git clone https://github.com/storytold/photocraft
cd photocraft
cargo run --release -p photocraft -- image.psd
```

Pokretanje desktop aplikacije:

```bash
cargo run --release -p photocraft
```

Pokretanje testnog skupa:

```bash
cargo test --workspace
```

Japanski fontovi za korisničko sučelje i alat za tekst dolaze iz projekta `craft-fonts`, koji je opcionalan ulaz pri izgradnji (zvanične desktop verzije ga uvijek uključuju). Bez njega PhotoCraft koristi sistemske CJK fontove:

```bash
git clone https://github.com/storytold/craft-fonts ../craft-fonts
CRAFT_FONTS_DIR="$PWD/../craft-fonts" cargo run --release -p photocraft
```

Novi saradnici i AI agenti trebaju početi s `AGENTS.md`, a zatim pregledati `docs/`.

Instalacijski paketi za macOS, Windows, Linux, FreeBSD i web dostupni su uz svako [GitHub izdanje](https://github.com/storytold/photocraft/releases). Na Linuxu možete izabrati AppImage, `.deb`, `.rpm`, tarball ili Flatpak paket. Za paket je potrebno freedesktop okruženje iz [Flathuba](https://flathub.org/), a `flatpak` ga može instalirati zajedno s aplikacijom:

```bash
flatpak install --user photocraft-<version>-linux-x86_64.flatpak
# ili -linux-aarch64
flatpak run ai.storyteller.photocraft
```

AppImage ne zahtijeva instalaciju: pri prvom pokretanju registruje ikonu pokretača i unos u meniju u `~/.local/share`, kako bi se ikona PhotoCrafta prikazivala na docku u Waylandu. Postavite `PHOTOCRAFT_NO_DESKTOP_INTEGRATION=1` da to preskočite; za poništavanje pogledajte odjeljak Linux u `docs/releasing.md`.

U Wayland sesiji prevlačenje datoteka na prozor još ne radi: `winit 0.30`, biblioteka za prozore koju koristi egui, nema podršku za drag-and-drop na Waylandu (#386). Koristite File › Open ili kopirajte sliku u upravitelju datoteka i zalijepite je pomoću Ctrl+V. Za prevlačenje pokrenite PhotoCraft pod XWaylandom:

```bash
WAYLAND_DISPLAY= photocraft
WAYLAND_DISPLAY= ./photocraft-<version>-linux-x86_64.AppImage
flatpak run --nosocket=wayland --socket=x11 ai.storyteller.photocraft
```

Na Waylandu PhotoCraft prikazuje komandu za vašu instalaciju u obavijesti dok je ne zatvorite. Preferences › Performance › Linux display server = X11 radi isto pri svakom pokretanju. Uz djelimično skaliranje prikaza (125%, 150%, 175%) XWayland prozor crta se u nižoj rezoluciji, a kompozitor ga uvećava, pa sučelje može biti mutno; izvorni Wayland ostaje oštar (#1072).

Na macOS-u alat komandne linije dolazi kao `photocraft-cli-<version>-macos-universal.zip`. Binarna datoteka potpisana je istim Developer ID-jem kao aplikacija i ovjerena kod Applea. Samostalna binarna datoteka ne može sadržavati priloženi notarizacijski tiket kao DMG, pa macOS pri prvom pokretanju provjerava notarizaciju putem interneta. Možete je provjeriti ovako:

```bash
ditto -x -k photocraft-cli-<version>-macos-universal.zip .
spctl --assess --type install -vv photocraft-cli-<version>-macos-universal/photocraft-cli
# ... accepted, source=Notarized Developer ID
```

Na FreeBSD-u 14 (x86_64), izdanje dolazi kao tarball raspoređen poput `/usr/local`. Instalirajte biblioteke za izvršavanje, a zatim ga raspakujte tamo:

```bash
pkg install libxkbcommon wayland libX11 libXcursor libXrandr libXi libxcb mesa-libs vulkan-loader gtk3 fontconfig freetype2 alsa-lib
tar -xzf photocraft-<version>-freebsd-x86_64.tar.gz --strip-components 1 -C /usr/local
photocraft
```

Održavaoci projekta mogu u `docs/releasing.md` pronaći objašnjenje kako se izdanja izrađuju, potpisuju i objavljuju.

## Važno: status projekta

PhotoCraft je u ranoj alfa fazi i želimo iskreno opisati njegovo stanje: veliki dio funkcija Photoshopa postoji u nekom obliku, ali **još nije zamjena za Photoshop za svakodnevni profesionalni rad**. Najveći nedostaci su AI/generativne funkcije, 15 alata koji nedostaju, napredne mogućnosti tipografije i profesionalnih radnih procesa te kompatibilnost s dodacima.

Svaka stavka Photoshopovog menija povezana je s komandom (`docs/parity-checklist.md`), ali to pokazuje povezanost komandi, a ne nužno potpuno jednako ponašanje. Iskren pregled po pojedinačnim područjima i plan daljnjeg razvoja nalaze se u [mapi puta](https://github.com/storytold/photocraft) i procjeni kompatibilnosti. Očekujte nedovršenosti i prijavite probleme (navedite operativni sistem, veličinu dokumenta, broj slojeva i snimak ekrana). Možete nam reći šta ne radi ni na [Discordu](https://discord.gg/artcraft).

# Dokumentacija

Dokumentacija za programere, arhitekturu, automatizaciju, formate i sigurnost nalazi se u [knjizi dokumentacije PhotoCrafta](https://github.com/storytold/photocraft). Za samostalno hostovanje verzije za preglednik pomoću Dockera pogledajte dokumentaciju za [Docker web hosting](https://github.com/storytold/photocraft).

# Sigurnost

Sigurnosna arhitektura, modeliranje prijetnji, ojačavanje parsera, fuzz testiranje i prijava ranjivosti obrađeni su u sigurnosnoj dokumentaciji i sigurnosnim pravilima repozitorija.

# Testni skupovi

PhotoCraft se testira na stvarnim datotekama: našim PSD referentnim datotekama izrađenim u Photoshopu u projektu `photocraft-corpus`, kao i skupovima `psd-tools`, `ag-psd` i `PngSuite`, koji su fiksirani i provjereni pomoću SHA-256. Preuzmite ih komandom:

```bash
cargo xtask corpus --all
```

Pokrenite testove:

```bash
cargo xtask test-corpus
```

Više detalja nalazi se u `docs/development.md`.

# Preuzimanja

**Prvi put koristite PhotoCraft?** Preuzmite ga sa stranice [PhotoCraft na getartcraft.com](https://getartcraft.com/). To je najjednostavniji način instalacije.

**Želite određenu verziju ili format?** Na GitHubu se u [najnovijem izdanju](https://github.com/storytold/photocraft/releases/latest) nalaze sve dostupne verzije, a [sva izdanja](https://github.com/storytold/photocraft/releases) sadrže i starije verzije s bilješkama.

`<ver>` u nazivima datoteka predstavlja broj verzije. `SHA256SUMS.txt` sadrži kontrolni zbir za svaku datoteku.

## Windows

| Arhitektura | Instalacijski paket | Prijenosna verzija |
|---|---|---|
| x64 (64-bitni Intel/AMD) | `photocraft-<ver>-windows-x64.msi` | `photocraft-<ver>-windows-x64-portable.zip` |
| arm64 (Snapdragon i drugi ARM računari) | `photocraft-<ver>-windows-arm64.msi` | `photocraft-<ver>-windows-arm64-portable.zip` |
| x86 (32-bitni) | `photocraft-<ver>-windows-x86.msi` | `photocraft-<ver>-windows-x86-portable.zip` |

Instalacijski programi i izvršne datoteke digitalno su potpisani.

## macOS

| Verzija | Datoteka | Napomena |
|---|---|---|
| Univerzalna aplikacija (Apple silicon + Intel) | `photocraft-<ver>-macos-universal.dmg` | Potpisana i ovjerena |
| Univerzalni alat komandne linije | `photocraft-cli-<ver>-macos-universal.zip` | Potpisan i ovjeren |

## Linux

| Format | x86_64 | aarch64 (ARM64) | Napomena |
|---|---|---|---|
| AppImage | `photocraft-<ver>-linux-x86_64.AppImage` | `photocraft-<ver>-linux-aarch64.AppImage` | Radi na različitim distribucijama; sam se ažurira pomoću `AppImageUpdate` (`.zsync` datoteke) |
| Flatpak | `photocraft-<ver>-linux-x86_64.flatpak` | `photocraft-<ver>-linux-aarch64.flatpak` | Izolovano okruženje; `flatpak install --user <file>` |
| Debian/Ubuntu | `photocraft-<ver>-linux-x86_64.deb` | `photocraft-<ver>-linux-aarch64.deb` | |
| Fedora/RHEL/openSUSE | `photocraft-<ver>-linux-x86_64.rpm` | `photocraft-<ver>-linux-aarch64.rpm` | |
| Tarball | `photocraft-<ver>-linux-x86_64.tar.gz` | `photocraft-<ver>-linux-aarch64.tar.gz` | Raspakujte bilo gdje |

**RISC-V (riscv64):** dostupna je samo datoteka `photocraft-<ver>-linux-riscv64.tar.gz`, izrađena za Ubuntu 24.04 (potreban je `glibc 2.39` ili noviji).

## FreeBSD

| Arhitektura | Datoteka |
|---|---|
| x86_64 | `photocraft-<ver>-freebsd-x86_64.tar.gz` |

## Web (WebAssembly)

| Verzija | Datoteka | Napomena |
|---|---|---|
| Statička web-stranica | `photocraft-web-<ver>.zip` | Radi u modernom pregledniku; hostujte je na bilo kojem statičkom serveru |

# Aplikacije Crafting Apps

PhotoCraft je dio kolekcije [Crafting Apps](https://getartcraft.com/): besplatnih kreativnih alata otvorenog koda tima ArtCraft. Svaki je napisan od nule u Rustu i može raditi samostalno.

| Aplikacija | Namjena | Kod | Više informacija |
|---|---|---|---|
| PhotoCraft | Uređivanje slika: slojevi, maske, tekst i prave PSD datoteke — nalazite se ovdje | [GitHub](https://github.com/storytold/photocraft) | [Web-stranica](https://getartcraft.com/) |
| VectorCraft | Vektorska ilustracija | GitHub | Web-stranica |
| FilmCraft | Uređivanje videa, boja i zvuka | GitHub | Web-stranica |
| LightCraft | Biblioteka fotografija i obrada RAW datoteka | GitHub | Web-stranica |
| PdfCraft | Čitanje, organizovanje i zaštita PDF-ova | GitHub | Web-stranica |
| EffectCraft | Pokretna grafika i vizuelni efekti | GitHub | Web-stranica |
| DesignCraft | Prijelom stranica i priprema za objavljivanje | GitHub | Web-stranica |

Tu je i sam [ArtCraft](https://getartcraft.com/), AI studio za slike i video namijenjen umjetnicima koji žele stvarnu kontrolu.

Sve aplikacije Crafting Apps dijele iste principe: clean-room implementacija i čisti Rust, izvorne aplikacije za macOS, Windows i Linux, rad u pregledniku preko WebAssemblyja i potpuno upravljanje putem agenata.

# Stvarajmo zajedno

Na našem Discordu okupljaju se umjetnici svih vrsta: ljudi koji slikaju, fotografišu, crtaju, montiraju filmove, oblikuju tekst — kao i oni koji tek otkrivaju šta žele stvarati. Podijelite svoj rad, zatražite pomoć, prijavite probleme ili recite šta biste željeli da ovi alati mogu raditi.

Bez obzira na medij i iskustvo, dobrodošli ste.

[discord.gg/artcraft](https://discord.gg/artcraft) · [getartcraft.com](https://getartcraft.com/) · [Crafting Apps](https://getartcraft.com/) · [PhotoCraft](https://github.com/storytold/photocraft)

# Licenca i zasluge

PhotoCraft je dostupan pod dvostrukom licencom **MIT** ili **Apache-2.0**, po vašem izboru.

Autorska prava © 2026 ArtCraft Team i saradnici projekta PhotoCraft. Obavezne napomene nalaze se u `NOTICE`.

Ugrađeni fontovi, ikone, slike i drugi resursi zadržavaju vlastite licence otvorenog koda; autori, izvori i licence navedeni su u `ATTRIBUTION.md`.

Sva prikazana umjetnička djela su u javnom domenu (Wikimedia Commons, NASA, U.S. National Archives); izvori su navedeni u `docs/images/SOURCES.md`.

Naziv ArtCraft, logotip i oznake u `docs/brand/` zaštitni su znakovi ArtCraft Teama i nisu obuhvaćeni ovom licencom. Mogu se koristiti samo neizmijenjeni i samo kao dio ovog repozitorija i PhotoCrafta, u skladu s `docs/brand/LICENSE-brand.txt`. Forkovi i izmijenjene verzije moraju ih ukloniti.

Adobe, Photoshop, Illustrator, Premiere Pro, Lightroom, Acrobat, After Effects i InDesign zaštitni su znakovi ili registrovani zaštitni znakovi kompanije Adobe Inc. u Sjedinjenim Američkim Državama i/ili drugim zemljama. PhotoCraft je nezavisan projekat otvorenog koda i nije povezan s kompanijom Adobe Inc., niti ga ona sponzoriše ili podržava. Ovi nazivi koriste se samo za opis kompatibilnih radnih procesa.

Izradili su ga ArtCraft tim i zajednica.

# Historija zvjezdica

