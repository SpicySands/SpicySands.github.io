---
layout: default
title: library
permalink: /library/
---

#songs
[<script type="module" src="https://cdn.jsdelivr.net/npm/@strudel/embed@latest"></script>](https://cdn.jsdelivr.net/npm/@strudel/embed@1.1.1/embed.min.js)

<h1>Strudel Library</h1>

<h2>Example 1: First Attempt</h2>
<strudel-repl>
// @title first try @by Dee
setcpm(180/4)

$:sound("<bd>*4")._scope() // Four on the Floor

$:note("<0 - 7 5 - 3 2 - 4 0 - 7 4 - 2 2- 3 0 - 7>* 8").scale("d:minor")
  .sound("gm_synth_bass_1").trans(-24).decay(.8)._scope()
$:note("<0 - 7 4 - 2 2 - 4 0 - 7 3 - 4 2- 3 0 - 7>* 8").scale("d:minor")
  .sound("gm_synth_bass_2").trans(-24)._scope()// bass

$:note("<0 - 7 5 - 3 2 - 4 0 - 7 4 - 2 2- 3 0 - 7>* 8").scale("d:minor")
  .sound("gm_synth_brass_1")._pianoroll()

$:note("<0 - 7 4 - 2 2 - 4 0 - 7 3 - 4 2- 3 0 - 7>* 8").scale("d:minor")
  .sound("gm_synth_brass_2").trans(24)._pianoroll()
$:note("<1 2 2 3 1 1 2 3>").scale("d:minor")
  .sound("gm_french_horn").gain(.5)._pianoroll()
  
$:note("<<G#,B,D#> <A#,C#,E#> <F#,A#,C#> <B,D#,F#>>/4").scale("d:minor")
  .sound("gm_drawbar_organ").decay(5)._pianoroll()
</strudel-repl>
