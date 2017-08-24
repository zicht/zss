# Media object

The ZSS media object is an abstraction of a common UI pattern: placing an image next to a bunch of text. It's based on the idea of [Nicole Sullivan](http://www.stubbornella.org/content/2010/06/25/the-media-object-saves-hundreds-of-lines-of-code/) but uses flexbox instead of floats.

## Source files

- [objects/_media.scss](../../src/objects/_media.scss)

## Usage

- Add `o-media` to the container of the image and text.
    - Optionally, add `o-media--center-figure` if the image should be vertically 
    aligned in the middle.
    - Optionally, add `o-media--reverse` to reverse the order: the text will be
    placed on the left, and the image on the right.
- Add `o-media__figure` to the image.
- Add `o-media__body` to the element that contains the text.

## Examples

```html
<!-- A regular media object -->
<article class="o-media">
    <figure class="o-media__figure">
        <img src="" alt="">
    </figure>
    <div class="o-media__body">
        <p>Text that will positioned to the right of the image.</p>
    </div>
</article>

<!-- A reversed media object -->
<article class="o-media  o-media--reverse">
    <figure class="o-media__figure">
        <img src="" alt="">
    </figure>
    <div class="o-media__body">
        <p>Text that will positioned to the left of the image.</p>
    </div>
</article>
```