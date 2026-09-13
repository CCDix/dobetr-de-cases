# Commissioner Logos

Dieses Verzeichnis enthält die Logos der drei Commissioners:

1. **deutschebaseballiga.png** – Logo der Deutschen Baseball Liga
   - Größe: mind. 200x200px
   - Format: PNG mit Transparenz
   - Quelle: https://www.baseball.de

2. **longevity-center-nuernberg.png** – Logo des Longevity Center Nuernberg
   - Größe: mind. 200x200px
   - Format: PNG mit Transparenz
   - Quelle: https://longevity-center-nuernberg.de/

3. **baumgartner-sports.png** – Logo von Baumgartner Sports
   - Größe: mind. 200x200px
   - Format: PNG mit Transparenz
   - Quelle: https://www.baumgartnersports.ch/en

## Integration

Die Logos können einfach in die `index.html` integriert werden. Beispiel:

```html
<div class="commissioner-logo">
    <img src="assets/logos/deutschebaseballiga.png" alt="Deutsche Baseball Liga Logo">
</div>
```

Und entsprechendes CSS in `styles.css`:

```css
.commissioner-logo {
    margin: var(--spacing-md) 0;
}

.commissioner-logo img {
    max-width: 150px;
    height: auto;
    filter: grayscale(0%);
    transition: filter 0.3s ease;
}

.case-card:hover .commissioner-logo img {
    filter: grayscale(20%);
}
```
