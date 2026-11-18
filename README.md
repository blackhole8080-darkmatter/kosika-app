# Kosika Apps

Things you can open and use, built with the [Kosika](https://github.com/blackhole8080-darkmatter/kosika) language.

## Kosika Chat

You type a question. Kosika answers in a few short lines and draws a picture that explains it, with the hover-to-highlight drawings from [Kosika Designs](https://github.com/blackhole8080-darkmatter/kosika-designs).

![Kosika Chat answering in the Dark Matter theme](chat/preview/chat-dark-matter.gif)

Ask it about the Fibonacci sequence and you get the golden spiral next to a real sunflower:

![Chat drawing the Fibonacci sequence](chat/preview/chat-fibonacci.png)

Kosi, the assistant, lives in the same window. It can check your news, your services and your GitHub, but only the sites you've allowed, and it asks before it changes anything.

![Kosi answering inside Chat](chat/preview/kosi-in-chat.png)

### Run it

Chat expects its three sister repos next to it, in one folder:

```text
git clone https://github.com/blackhole8080-darkmatter/kosika
git clone https://github.com/blackhole8080-darkmatter/kosika-agents
git clone https://github.com/blackhole8080-darkmatter/kosika-designs
git clone https://github.com/blackhole8080-darkmatter/kosika-app
cd kosika && python -m pip install . && cd ..
python -m pip install numpy pillow scipy
python kosika-app/chat/server.py          # then open http://127.0.0.1:8793
```

It uses free models only. Set `GROQ_API_KEY` first. If your folders sit somewhere else, point `KOSIKA_HOME`, `KOSIKA_AGENTS_HOME` and `KOSIKA_DESIGNS_HOME` at them.

## What Kosika draws

Chat draws beside its answers with Kosika Designs. These are some of the
newest drawings: Kosi as a living cell, maths that moves, and the Kosika
Brain in 3D.

<table>
<tr>
<td><img src="gallery/kosi-shapes.gif" width="240" alt="Kosi changing shape"></td>
<td><img src="gallery/m-taylor-growing.gif" width="240" alt="A Taylor series growing"></td>
<td><img src="gallery/a-black-hole.gif" width="240" alt="A black hole"></td>
</tr>
<tr><td>Kosi, a living cell</td><td>A Taylor series, growing</td><td>A black hole</td></tr>
</table>

<img src="gallery/b-brain-maths-3d-lit.webp" width="480" alt="The Kosika Brain drawn in 3D">

**More, moving and live in 3D, in the [Kosika Gallery](https://blackhole8080-darkmatter.github.io/kosika-site/gallery/).**

## MayaOS

`mayaos/maya.kos` is the mind of MayaOS, an AI layer over the computer. It decides what to greet you with, what needs your attention and which Kosika app to open. The window that shows it is part of Kosika Studio in the main repo.

```text
kosika test mayaos/maya.kos
```

## Licence

MIT, like the rest of Kosika.
