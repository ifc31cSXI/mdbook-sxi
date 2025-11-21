# mdbook-sxi
Aquesta serà el respositori inicial amb les instruccions per crear la documentació del modul de Serveis de Xarxes i Internet.
**mdBook** és una eina per crear llibres, manuals i apunts a partir de fitxers **Markdown**.

## mdBook
- Creat inicialment per a la documentació de **Rust**.
- Permet escriure un llibre amb Markdown i exportar-lo com a web navegable.
- Característiques:
  - Genera índex i navegació automàtica.
  - Suporta cerca integrada.
  - Suporta temes i estils personalitzats.
  - Es pot desplegar fàcilment amb GitHub Pages.

## Instruccions
En aquestes instruccions es descriuran les passes per instal·lar mdBook, crear un mdBook, publicar-lo amb GitHub Pages.
1. Assegura't de tenir instal·lat **Rust**: [Instal·lació](https://www.rust-lang.org/tools/install).
2. Executa la següent ordre per instal·lar mdBook:
   ```sh
   cargo install mdbook
   ```
3. Crear estructura bàsica amb
   ```sh
   mdbook init
   ```
   - `book.toml`: configuració del llibre.
   - `src/SUMMARY.md`: índex de continguts.
   - `src/*.md`: capítols en Markdown. -
4. Dins `src/SUMMARY.md` crear l'estructura de continguts del llibre per exemple:
   ```
   - [Chapter 1](./chapter_1.md)
   - [Chapter 2](./chapter_2.md)
   - [Chapter 3](./chapter_3.md)
   ```
5. Dins els fitxers `chapter_1.md`, `chapter_2.md` ... s'ha de fe la documentació de cada apartat.
4. Generar i veure el llibre
   ```sh
   mdbook build   # genera el llibre a /book
   mdbook serve   # inicia un servidor local (http://localhost:3000)
   ```
## Lliurament
Només cal fer commits i push al teu repositori generat per GitHub Classroom.
