# Tutorial de Skinning 


* **_Skin_**: Son todas aquellas variaciones del aspecto original de _osu!_
* **_Skinning_**: Es la acción de modificar/crear elementos para la interfaz de _osu!_

Los articulos de tutoriales de skin son para enseñar de manera general como hacer skinning.

## Skinning FAQ _(Preguntas frecuentes)_

### ¿Podría alguien hacer una skin de este programa/juego?

Si has pasado por todo el foro de osu!skinning y estás seghuro que no puedes encontrar _esa_ skin, entonces felicitaciones, osu! aún no la tiene.
Con esto en mente, tu puedes tomar esta iniciativa para crear la skin de tus sueños y hacer algo que todos los demás pueden querer!

Sin embargo, por favor, **nunca** hagas una solicitud de una Skin en cualquier lugar de osu!forums.
El no seguir esta regla hará que se mueva tu hilo del foro a los terrenos baldíos del mismo.

### ¿Donde puedo conseguir esta skin que usó un YouTuber/Streamer?

Antes que nada, no vayas preguntando esto en los osu!forums, tu hilo será muy probablemente tirado en los terrenos baldíos del mismo.
Segundo, tu mejor apuesta es simplemente preguntarle a esa persona por la skin que está usando.

### ¡Quiero hacer una skin! pero, ¿qué necesito?

Buena elección, pero recuerda, el skinning puede ser un poco dificil para un novato.
Al comienzo de hacer cualquier skin, deberías tener:

- Habilidades de principiante con cualquier programa de edición de fotos (que soporte transparencia) como Photoshop, GIMP, Paint.NET, etc.
- Paciencia (si, el skinning toma tiempo).
- ¡Una idea! (si, esto es **muy** importante, trata de ser ingenioso cuando estés haciendo tu skin).

### ¿Que hay acerca del "new" y el "old" estilo de skinning?

Esta pregunta también podria ser, ¿Que es la versión 1.0 y 2.0+ en las skins?

El nuevo y viejo estilo de skinning fué una opción en el osu!client.
Era, sin embargo, removido por que el skin.ini ahora maneja el control de versiones de skins.

El estilo "old" de skinning, ahora conocido como "version 1.0", es un estilo que fué usado para la antigua skin por defecto (antes de Marzo del 2013).
Después de la actualización de Marzo 2013 ("March 2013 update"), también conocida como "version 2.0", peppy introdujo una nueva skin por defecto con sus nuevos comportamientos y partes.
Hubo unos pocos cambios importantes como un nuevo spinner, countdown, hitbursts, y el comportamiento del ranking-panel.
Para un registro de cambios en las actualizaciones de skinning, vease [Skinning](../).

Puede que no parezca importante denotar qué versión usas, pero recuerda que algunas de las caracteristicas antiguas pueden no estár disponibles en la ultima versión de skinning.

### ¿Qué es skinning? ¿Necesito algún tipo de poder mágico para hacer una skin?

Afortunadamente, no necesitas poderes mágicos para hacer una skin.

Skinning es un simple mecanismo de cambiar imágenes que osu! cargará al seleccionar una skin en las opciones.
Crear skins es facil (pero crear elementos, las imagenes, es un poco más complicado de lograr).

Primero necesitarás encontrar tu carpeta de `Skins` la cual está dentro de tu directorio de osu!
Desde ahí, podrías hacer una carpeta nueva y llamarla como quieras y de ahí empezar a hacer la skin.

Deberías notar que osu! cuenta con más de 200 elementos modificables en una skin (sin incluir los fotogramas individuales de animación).
No tengas miedo con la cantidad por que,recuerda, **no estás obligado a cambiar todo**

### ¿Qué debería contener mi carpeta de Skin?

Generally, the skinning elements and the skin.ini file are important parts of your skin and should be included.Generalmente, los elementos de skinning y el atchivo skin.ini son partes importantes de tu skin y deberán ser incluidos.
Qué partes son las que añadirás, es completamente tu decisión ya que, para los elementos que no cambies, se utilizaran los de la skin por defecto.

Eres capaz de añadir diferentes carpetas con partes alternativas para tu skin.
A osu! no le importan si están o no.
Notese que, sin embargo, la sub-carpeta llamada `taiko` (aiuda con -> "name is case-insensitive") es reservada para skins de osu!taiko, que anulará todos los elementos de osu!taiko (y algunos elementos de la interfaz cuando juegas un mapa de osu!taiko).

### ¿Puedo usar un elemento skineado de la skin de alguien más?

**¡Nunca publiques una skin con elemento(s) de skin de otro usuario sin su permiso!**

Esta es una regla importante en el skinning.
Si obtienes su permiso, o el usuario no está activo y es imposible de contactarlo, solamente recuerda darle el credito de manera apropiada.

### ¿Que hay acerca de los "remixes"?

This will help skinners make their original skins stand out than the remixed/mashup-ed skins.Esto ayudará a mantener las skins originales apartadas de las skins "remix".

### ¿Cómo puedo animar un elemento?

Know that osu! allows you to animate some elements, but not all of them.
To create an animation for an animatable element, you will need the frames for that animation frame by frame.
With those, name them in order prefixed with the skinning element name then suffix with a hyphen (`-`), an index number (start the count at zero), then the file extension (`.png`).

Most of the animatable skinning elements do not limit you to the amount of frames.
However, know that the animation rate could play the animation too slowly before the user would be able to see them.
To find the balance between the animation rate and the frames, you'll need to do trail-and-error (see next section below for more details).

Lastly, while most do, not all skinning elements use the hyphen then number system for animating a skinning element.
For example:

- `sliderb` has its frames named: sliderb0, sliderb1, sliderb2, etc.
- `pippidonclear` has its frames named: pippidonclear0, pippidonclear1, pippidonclear2, etc.

### Mi animación se reproduce muy lento/rapido, ¿como lo puedo solucionar?

If your animation is too fast/slow, you have two ways to fix it

1. if it is playing too fast, try to make them longer by doubling frames (or half, if too slow)
   - i.e. frame 0 and 1 are the same picture (so picture will last 2 frames), frame 2 and 3 are second picture, etc.
   - this will make animation slightly slower (or slightly faster);
     however the animation rate is still the same, this means that even if you slowed/sped-up one down, another's animation rate may still be too fast/slow
2. use the `AnimationFramerate` command in the skin.ini
   - this command affects all animations expect for a few, like pippidon or the hitcircleoverlay

### What are "normal", "simplified", and "PRO" skins?

Those are the three basic categories for skins:

- **Normal**
  - Normal skins contains elements that the skinner wants to change.
  - They don't have to necessarily follow the given template sizes.
  - These skins are often colourful and creative.
  - May contains many different animations.
  - Typical skin for casual player.
- **Simplified**
  - Simplified skins are directed to a players who dislike distractions, but like to see some things.
  - Skins like this often have minimized size of hitbursts (300,100, 50 etc.), size of parts aren't larger than template's, less colourful, less animations.
- **PRO**
  - This kind of skin it totally focused on removing any distractions that skin can provide.
  - Skins like this contains transparent hitbursts, no animations, reduced amount of colours used in it, larger `followpoint.png`, semi-transparent hit circle, and less sounds.

### What is the skin.ini for and what does it do?

The skin.ini file allows you to define specific behaviors on how osu! will display your skin.
The list includes but isn't limited to:

- name of a skin that show up in osu!
- the creator's name (fourm name is prefered)
- skin version (what behavior should osu! use, not your skin's verisoning number)
- colours
- osu!mania key, note, and stage behaviors
- osu!mania image names and paths

### How do I share?

To make sharing your skin easy, you should export your skin as an `OSK` file.
With this file, you can upload it then post about it in the skinning subfourms.

Here is how to make an `OSK` file with osu!

1. Open to osu!
2. Click on `Options`
3. Load your skin
4. Click the button that says `Export as .osk`
5. From there osu! will open a window for your exported skin.
6. Take that file and upload it then share!

### Can I post R15 skins in the osu!skinning subforums?

**Yes, and if you do, you _must_ add warning that your skin contains any of the below.**

Probably some of you ~~perverts~~ would like to make a skin that will contain mature content.
All cases are simple, if you are going to post a skin that have it, you are only allowed to post R15 or "ecchi" skins.

R15 skins may include but are not limited to:

- suggestive or visible underwear
- swimsuits and/or bikini
- characters with revealing clothing (or with really skimpy clothing)

### Can I post R18 skins in the osu!skinning subforums?

**You are _NOT_ allowed to post skins that contains any R18 content anywhere in osu!. Period.**

If you post your R18 skin anywhere in the osu!community, be aware that you will be punished for that.
On the other hand, if you release it outside the osu!community walls, nobody will hunt you down.


## Posting your skin in the osu! skinning subforums

Of course, this is the _optional_ last step to skinning!

1. Delete all non-skinned parts
   - there is no need to include them because this will make your folder larger than it should be
   - and that osu! will have to load more images than it would have to if it used its defaults anyways
2. Next, create the `OSK` file (follow steps from above) and upload it somewhere
   - Most people prefer a direct download, so you can use upppy! or puush
   - Mediafire is fine too (but of course, you aren't limited to the ones listed)

### Skinning Thread Template

If you don't know how to make friendly looking thread you can use this template by Dragvon (modified).

```
[General]
[b]Skin Name[/b]: Your skin name will go here.
[b]Creator[/b]: Name(s) of who made it.
[b]Theme[/b]: Tell us what theme your skin is based at.
[b]Version[/b]: Self-explanatory
[b]Tags[/b]: This can make finding your skin easier.
[b]Download[/b]: Put download link here.

[Data]
[b]Size[/b]: Approx. size of your skin
[b]Is it fully skinned? Yes/No.[/b] (Gameplay/Menu/Taiko/Catch the Beat/cursor - only?)
[b]HD support? Yes/No.[/b] (does the skin use HD images (using the @2x suffix))
[b]Screenshots[/b]: Screenshots go here. (Adding a spoilerbox is useful for people with slow connections)
[b]Video preview[/b]: (Optional, if you have one)

[Misc]
[b]Creator's comment[/b]: Self-explanatory.
[b]Updates[/b]: Leave your updates here (Again, a spoilerbox could be very useful here)
[b]Requests[/b]: Since no one is perfect, you can use this to request help to your skin :)
```

It is really important to include various screenshots of gameplay and the song selection, etc..
A lot of people will want to see your skin looks like before carelessly downloading it!
You can use upppy or puush to upload them.
