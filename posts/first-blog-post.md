---
title: Week 1
published_at: 2022-11-04
snippet: Introduction to my video  
disable_html_sanitization: true
allow_math: true
---

#  THEMES

For my self portrait video I am to portray the themes of duality and growth. 
When I think about myself there are two versions that exist in me;

**There is Sami,** who is very relaxed, introverted and quiet. If not at work or uni his day mainly looks like going on walks, shopping, or being at a cafe enjoying his own company or occasionally catching up with a friend. Mornings/early afternoons are his favourite time of the day. 

**Then there is Persia,** who is my personality when I'm on stage performing or when I have to step up. 
I am involved in the Ballroom queer scene here in Naarm and a part of the House of DIESEL who are my chosen family. We do a lot of work for the scene here holding balls, vogue nights, performances, workshops, community sessions etc. This side of me is very outgoing, usually for nightlife and when I'm performing I completely tap into her essence. 

When I’m not doing community work or performing I’m a very reserved and peaceful person. I will usually spend my time outside by nature alone, I love my alone time, and just be walking around or listening to music. I wanted to start with that side of me, and end with the other side of my life which is on the opposite end of the spectrum. 

I find the difference between sami and persia quite interesting so i wanted to theme my video around the different sides while also showing my life, family and friends. 

 `[My Ballroom family](https://www.starobserver.com.au/artsentertainment/my-cnt-so-lethal-the-house-of-diesel-naarms-newest-ballroom-family-have-arrived/228521)`






![a drippy lemon](logo.svg)

^ images are written like this: `![storyboard](file_path/file_storyboards.png)`

## This is h2

*This is italic.*[^1]

[^1]: This is a footnote, *which can also be italic*.

**This is bold.**

Hyperlinks can be written like this: 

You can find a markdown cheat-sheet [here](https://www.markdownguide.org/cheat-sheet/).

## Maths:

... which can be written inline, like this: $\{ x, y, z \} \in \N$

... or block, like this:

$$ x^2 + y^2 = z^2 $$

Visit [ $\KaTeX$ ](https://katex.org/docs/supported#fractions-and-binomials) for more information about writing maths.

## Embedding video:

<iframe id="coding_train_video" src="https://www.youtube.com/embed/rI_y2GAlQFM?si=RDgjkpunxk1mQzMI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<script type="module">

    console.log (`hello world! 🚀`)

    const iframe  = document.getElementById (`coding_train_video`)
    iframe.width  = iframe.parentNode.scrollWidth
    iframe.height = iframe.width * 9 / 16

</script>

## Embedding p5 sketches:

<iframe id="falling_falling" src="https://editor.p5js.org/capogreco/full/Fkg05m7aA"></iframe>

<script type="module">

    const iframe  = document.getElementById (`falling_falling`)
    iframe.width  = iframe.parentNode.scrollWidth
    iframe.height = iframe.width * 9 / 16 + 42

</script>

## Canvas API

<canvas id="canvas_example"></canvas>

<script type="module">
    const cnv = document.getElementById (`canvas_example`)
    cnv.width = cnv.parentNode.scrollWidth
    cnv.height = cnv.width * 9 / 16

    const ctx = cnv.getContext (`2d`)
    const pos = {
        x: -100,
        y: cnv.height / 2 - 50
    }
    
    function draw_frame () {
        ctx.fillStyle = `turquoise`
        ctx.fillRect (0, 0, cnv.width, cnv.height)

        ctx.fillStyle = `hotpink`
        ctx.fillRect (pos.x, pos.y, 100, 100)

        pos.x += 2

        if (pos.x > cnv.width) {
            pos.x = -100
        }

        requestAnimationFrame (draw_frame)
    }

    draw_frame ()
</script>


