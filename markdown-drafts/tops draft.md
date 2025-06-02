---
title: "Instrumental Timbre and Texture in Popular Song"
author: "Megan Lavengood"
date: "June 5, 2025"

customTheme: "solarized-custom"
slideNumber: true
preloadiframes: true
fragments: true

output: revealjs::revealjs_presentation
---

<!-- This workshop investigates instrumental timbre and texture in popular song, building on the approaches of Moore (2012) and Lavengood (2020, 2021) to explicate relationships between an instrument's timbral qualities and its role within the larger texture. Regardless of the specific instrumentation, many popular songs comprise four basic layers of the musical texture, which are typically separated by register (different pitch levels) and timbre (different tone colors): melody, harmony, bass, and explicit beat layers; some songs additionally feature a rhythmically and timbrally marked novelty layer that does not blend with the others. By bringing attention to various marginalized subgenres of popular music (e.g., rap, EDM), we will also scrutinize the assumptions that underlie existing definitions of popular-music terms and analytical models. -->

<link rel="stylesheet" href="bootstrap-2.css">
<!-- <link rel="stylesheet" href="custom.css"> -->

# Instrumental Timbre</br>and Texture<br/>in Popular Song <!-- .element: class="r-fit-text" -->

<div class="r-stretch"></div>
<div class="row justify-content-between align-content-end g-2">
    <div class="col"><p style="text-align:left;">
        Megan Lavengood<br/>
        <a href="mailto:mlavengo@gmu.edu">mlavengo@gmu.edu</a>
    </p></div>
    <div class="col" style="text-align:right;"><p class="r-fit-text">Timbre and Orchestration in Popular Song<br/>
Montreal, QC</br>
June 5, 2025</p></div>
</div>

--

## [Bibliography](https://www.zotero.org/mlavengood/collections/2URXWKKL/item-list)

<a href="https://www.zotero.org/mlavengood/collections/2URXWKKL/item-list"><img src="/teaching-timbre/bibqr-tops.svg" width="50%"></a>

---

## Workshop outline

1. Timbre analysis methodology
2. Texture analysis
3. Refining definitions: texture analysis in EDM

---

## 1. Timbre analysis

-   Explained in [2020 _MTO_ article](https://mtosmt.org/issues/mto.20.26.3/mto.20.26.3.lavengood.html)
-   Spectrograms are used to aid in describing timbre
    -   Visual analysis suffices for many features
    -   MIR (measuring spectral centroid) more helpful for brightness in particular
-   Timbre vocabulary set up in a system of binary oppositions

--

### Oppositional vocabulary

[Lavengood (2020), \[1.9–19\]](https://mtosmt.org/issues/mto.20.26.3/mto.20.26.3.lavengood.html)<!-- .element: class='r-fit-text' -->

<div class='container'>

::: .col

#### Spectral - sustain

-   _bright / dark_
-   _pure / noisy_
-   _full / hollow_
-   _rich / sparse_
-   _beatless / beating_
-   _harmonic / inharmonic_

::: ::: .col

#### Spectral - attack

-   _percussive / legato_
-   _bright / dark_

&nbsp;

#### Pitch

-   _low / high_
-   _steady / wavering_

:::

</div>

--

### Markedness

[Hatten (1994)](https://www.zotero.org/mlavengood/collections/2URXWKKL/item-list)

-   "the valuation given to difference" (Hatten 1994, 34)
-   One oppositional term carries more meaning than the other: more culturally specific
-   Inherently culturally situated
    -   Lavengood (2020) compares to a clean electric guitar sound
    -   Other contexts need to have a more appropriate context

---

## Instrument-specific vocabulary

-   Lavengood (2020) is meant to be generally specific, but it was built with the DX7 in mind as a case study; probably best for pitched instruments.
-   Vocal timbre: probably better to use Heidemann (2016) embodied terms
-   Percussion timbre: see Lavengood and Barranco (forthcoming): based on orchestral music, but illustrates how different vocabulary is useful for percussion.

--

### Vocal timbre

::: .container

::: {style=width:25%;}

:::

::: {style=width:50%;}

<img src="https://www.mtosmt.org/issues/mto.16.22.1/heidemann_table1.png" class="r-frame">

:::

::: {style=width:25%;}

Heidemann (2016) <br/> Table 1 {style=text-align:right;}

:::

:::

--

### Percussion timbre

Lavengood and Barranco (2020)

<div class='container align-items-center' style="text-align:left;">

::: .col

#### Triangles

-   _simple/complex_
-   [_dark/bright_]
-   [_beatless/beating_]

#### Crash cymbals <!-- .element: style="margin-top: 20px;" -->

-   [_dark/brilliant (attack)_]
-   [_dark/brilliant (decay)_]
-   _thin/full_

:::

::: .col

#### Tambourines

-   [_dark/brilliant_]
-   _wet/dry_
-   [_pure/noisy_]
-   _clicky/washy_

:::

</div>

<aside class="notes">

-   _Brilliant/dark_. Percussionists associate a brilliant attack with one that has high overtones on striking the tambourine. To evaluate this, we measure the frequencies of these resonant overtones through spectrogram analysis, focusing on the frequencies that extend beyond the band of noise produced by the initial attack. For this analysis, we have chosen 11,500 Hz as our threshold: a tambourine with jingles resonating over 11,500 Hz is brilliant, while a tambourine with resonating jingles only below that value is dark.
-   _Dry/wet_. A wet sound has a decay that lasts for a substantial period of time, while a dry sound has a shorter decay. We measure this using the struck tambourine samples, and our threshold is 0.7 seconds—anything above is wet, and anything below is dry.
-   _Pure/noisy_. This opposition refers to the aural clarity of individual jingles in the sound when the tambourine is struck. On the spectrogram, a pure decay has overtones that are visually thin and separated from the other bands on the spectrogram. A noisy sound has thicker bands that are closer together, obscuring the pitches of the jingles.
-   _Clicky/washy_. This is the only opposition that refers to the tambourine when shaken instead of struck; it correlates to average spectral centroid measurements, and thus to the brightness of the shake. Samples with a centroid of over 9000 Hz are considered washy, while those below 9000 are clicky. In practice a washy tambourine would be particularly good for a smooth, shimmery tambourine shake-roll, while a clicky tambourine shake would have more subtle micro-attacks that render better rhythmic clarity.
-   _Simple/complex_. Percussionists tend to speak of triangles in terms of their simple or complex overtones. To evaluate this, we count the number of overtones above -110 dBV for each triangle sample, as shown in a spectrum plot of the sample at one second past the initial attack. For this study, we call triangles with less than eighteen such overtones simple, while those with eighteen or more are complex.
-   _Bright/dark_. Similar to brilliant/dark when discussing tambourines, bright/dark references the presence of high-pitched overtones as the instrument decays. With tambourines, we look for the presence of overtones above the specified threshold, but with triangles, we are looking for overtones below the threshold—in this case, 1,300 Hz. In other words, all triangles have high and low overtones, but dark triangles have particularly noticeable low-frequency overtones. If a relatively strong partial is present at 1,300 Hz or below, we consider the instrument dark, due to the foregrounded presence of these lower overtones. If an instrument does not have activity at or below 1,300 Hz, we classify it as bright.
-   _Beatless/beating_. These oppositions refer to acoustic beats created through interference between slightly different frequencies (not to be confused with triangle beaters), which may or may not be audible in the triangle’s decay. Visually, a beatless decay has thin, consistent lines on the spectrogram, while a beating decay has dotted lines.
-   _Brilliant/dark_ (attack). This opposition accounts for the frequency of the highest-amplitude peak in the spectrum in the cymbal’s attack. If a cymbal has a dark attack, the highest amplitude peak occurs at a lower frequency. Therefore, a brilliant classification would indicate that the highest amplitudes occur at a higher frequency. This measurement reflects the way that specific frequencies might be detected by the listener in the initial attack. For this study, we determined 400 Hz to be the dividing line.
-   _Brilliant/dark_ (decay). This opposition is based on the spectral centroid of the sound signal, measured at four seconds after the initial attack, which gives ample time for the wash of noise in the initial contact sound to dissipate; only the strongest overtones will continue to ring at this point. For this study, 2000 Hz was a useful dividing line between brilliant/dark.
-   _Thin/full_. This opposition summarizes the amplitude of the decay across a broad frequency range. A cymbal crash is full if the amplitude of the decay is relatively even across the entire frequency range. If the crash has an unusually narrow range, or if the amplitude is particularly uneven in certain ranges of the spectrogram, then the timbre is thin.

</aside>

---

## Data collection

1. Analyst determines which timbres to focus on
2. Obtain isolated audio for that timbre (recreate, rebalance in iZotope, look for stems online, pull from a stripped-down texture) and generate spectrograms for that audio … **or just listen really closely**
3. Go through each opposition and assign a term (+, −, ∅, ±)

--

### Interpretation

-   Assigning +/− is a first step in analysis, like identfiying Roman numerals. It is not in itself very meaningful.
-   The analyst must go on to do something with that data: compare it to other data, etc.
-   **In Lavengood (2020; 2021), the question is: what are the relationships between timbre and texture?**

---

## 2. Texture

-   Expanding on work by Allan Moore (2012)
-   Traditional terms—homophony, polyphony, heterophony, monophony—are not very useful for analyzing pop (or classical…? …or anything?)

--

### Functional layers

1. Explicit beat layer
2. Functional bass layer
3. Harmonic filler layer
4. Melodic layer
5. Novelty layer

--

#### Novelty layer

(see also Reymore's work)

-   Often melodic in content, but not necessarily
-   Intermittent—cuts in and out of the texture, often in call-and-response with melodic layers
-   Least common of all functional layer types
-   Typically uses marked timbres and instruments

--

Moore (2012), 20

<div class="row flex-wrap justify-content-between">

::: .col

#### Explicit beat layer

-   "articulate[s] an explicit pattern of beats"
-   uses unpitched percussion
-   part of the song's groove

:::

::: .col

#### Functional bass layer

-   "connect[s] root position harmonies in one or more ways"
-   also part of the groove

:::

</div>

--

Moore (2012), 20

<div class="row flex-wrap justify-content-between">

::: .col

#### Melodic layer

-   primary and secondary melodic lines; "the tune"
-   "articulate[s] the songs lyrics"
-   most memorable and identifiable

:::

::: .col

#### Harmonic filler layer

-   "fill[s] the 'registral space' between these bass and treble layers"
-   contributes greatly to a listener's sense of genre in a song

:::

</div>

--

-   Moore's textural layers are certainly an improvement on traditional texture terms, but
-   Moore's definitions rely on intuition and unspoken rules
-   Based in mainstream pop and rock music

**How do other genres complicate these definitions?**

**How can these complications reveal more about what the definitons should be?**

---

## 3. Breakout activity <!-- .element: class="r-fit-text" -->

<iframe style="border: 0; width: 100%; max-width: 700px; height: 120px; margin-left: auto; margin-right: auto;" data-src="https://bandcamp.com/EmbeddedPlayer/album=2765736108/size=large/bgcol=333333/linkcol=9a64ff/tracklist=false/artwork=small/track=4231873605/transparent=true/" seamless><a href="https://jlin.bandcamp.com/album/black-origami">Black Origami by Jlin</a></iframe>

[download mp3](https://gmuedu-my.sharepoint.com/:u:/g/personal/mlavengo_gmu_edu/EfrL_MJQkOhIiijUnpwF1toBt4kmLv1Sr1pKm9mjI01Vqw?e=cYIqHx) <!-- .element: class="small" -->

::: .r-stretch

Possible activities:

1. Identify instruments (by name, by timbre, onomotopoeia)
2. Categorize instruments as belonging to functional layers (melody, harmony, bass, beat, novelty)
3. Transcribe rhythmic motives

:::

--

## Discussion: Jlin

<iframe style="border: 0; width: 100%; max-width: 700px; height: 120px; margin-left: auto; margin-right: auto;" data-src="https://bandcamp.com/EmbeddedPlayer/album=2765736108/size=large/bgcol=333333/linkcol=9a64ff/tracklist=false/artwork=small/track=448110133/transparent=true/" seamless><a href="https://jlin.bandcamp.com/album/black-origami">Black Origami by Jlin</a></iframe>

-   How do we need to modify functional layer definitions to accommodate music like this?
-   What does that tell us about all pop music textures?

---
