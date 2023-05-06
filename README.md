<!DOCTYPE html>
<html lang="en"><head>
<script src="QMD_show_files/libs/clipboard/clipboard.min.js"></script>
<script src="QMD_show_files/libs/quarto-html/tabby.min.js"></script>
<script src="QMD_show_files/libs/quarto-html/popper.min.js"></script>
<script src="QMD_show_files/libs/quarto-html/tippy.umd.min.js"></script>
<link href="QMD_show_files/libs/quarto-html/tippy.css" rel="stylesheet">
<link href="QMD_show_files/libs/quarto-html/light-border.css" rel="stylesheet">
<link href="QMD_show_files/libs/quarto-html/quarto-html.min.css" rel="stylesheet" data-mode="light">
<link href="QMD_show_files/libs/quarto-html/quarto-syntax-highlighting.css" rel="stylesheet" id="quarto-text-highlighting-styles"><meta charset="utf-8">
  <meta name="generator" content="quarto-1.3.326">

  <meta name="author" content="Marcus Antonio Cardoso Ramalho PPGAd-UFF">
  <title>O Quarto como ferramenta de PKM para pesquisa científica</title>
  <meta name="apple-mobile-web-app-capable" content="yes">
  <meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no, minimal-ui">
  <link rel="stylesheet" href="QMD_show_files/libs/revealjs/dist/reset.css">
  <link rel="stylesheet" href="QMD_show_files/libs/revealjs/dist/reveal.css">
  <style>
    code{white-space: pre-wrap;}
    span.smallcaps{font-variant: small-caps;}
    div.columns{display: flex; gap: min(4vw, 1.5em);}
    div.column{flex: auto; overflow-x: auto;}
    div.hanging-indent{margin-left: 1.5em; text-indent: -1.5em;}
    ul.task-list{list-style: none;}
    ul.task-list li input[type="checkbox"] {
      width: 0.8em;
      margin: 0 0.8em 0.2em -1em; /* quarto-specific, see https://github.com/quarto-dev/quarto-cli/issues/4556 */ 
      vertical-align: middle;
    }
  </style>
  <link rel="stylesheet" href="QMD_show_files/libs/revealjs/dist/theme/quarto.css" id="theme">
  <link href="QMD_show_files/libs/revealjs/plugin/quarto-line-highlight/line-highlight.css" rel="stylesheet">
  <link href="QMD_show_files/libs/revealjs/plugin/reveal-menu/menu.css" rel="stylesheet">
  <link href="QMD_show_files/libs/revealjs/plugin/reveal-menu/quarto-menu.css" rel="stylesheet">
  <link href="QMD_show_files/libs/revealjs/plugin/quarto-support/footer.css" rel="stylesheet">
  <style type="text/css">

  .callout {
    margin-top: 1em;
    margin-bottom: 1em;  
    border-radius: .25rem;
  }

  .callout.callout-style-simple { 
    padding: 0em 0.5em;
    border-left: solid #acacac .3rem;
    border-right: solid 1px silver;
    border-top: solid 1px silver;
    border-bottom: solid 1px silver;
    display: flex;
  }

  .callout.callout-style-default {
    border-left: solid #acacac .3rem;
    border-right: solid 1px silver;
    border-top: solid 1px silver;
    border-bottom: solid 1px silver;
  }

  .callout .callout-body-container {
    flex-grow: 1;
  }

  .callout.callout-style-simple .callout-body {
    font-size: 1rem;
    font-weight: 400;
  }

  .callout.callout-style-default .callout-body {
    font-size: 0.9rem;
    font-weight: 400;
  }

  .callout.callout-titled.callout-style-simple .callout-body {
    margin-top: 0.2em;
  }

  .callout:not(.callout-titled) .callout-body {
      display: flex;
  }

  .callout:not(.no-icon).callout-titled.callout-style-simple .callout-content {
    padding-left: 1.6em;
  }

  .callout.callout-titled .callout-header {
    padding-top: 0.2em;
    margin-bottom: -0.2em;
  }

  .callout.callout-titled .callout-title  p {
    margin-top: 0.5em;
    margin-bottom: 0.5em;
  }
    
  .callout.callout-titled.callout-style-simple .callout-content  p {
    margin-top: 0;
  }

  .callout.callout-titled.callout-style-default .callout-content  p {
    margin-top: 0.7em;
  }

  .callout.callout-style-simple div.callout-title {
    border-bottom: none;
    font-size: .9rem;
    font-weight: 600;
    opacity: 75%;
  }

  .callout.callout-style-default  div.callout-title {
    border-bottom: none;
    font-weight: 600;
    opacity: 85%;
    font-size: 0.9rem;
    padding-left: 0.5em;
    padding-right: 0.5em;
  }

  .callout.callout-style-default div.callout-content {
    padding-left: 0.5em;
    padding-right: 0.5em;
  }

  .callout.callout-style-simple .callout-icon::before {
    height: 1rem;
    width: 1rem;
    display: inline-block;
    content: "";
    background-repeat: no-repeat;
    background-size: 1rem 1rem;
  }

  .callout.callout-style-default .callout-icon::before {
    height: 0.9rem;
    width: 0.9rem;
    display: inline-block;
    content: "";
    background-repeat: no-repeat;
    background-size: 0.9rem 0.9rem;
  }

  .callout-title {
    display: flex
  }
    
  .callout-icon::before {
    margin-top: 1rem;
    padding-right: .5rem;
  }

  .callout.no-icon::before {
    display: none !important;
  }

  .callout.callout-titled .callout-body > .callout-content > :last-child {
    margin-bottom: 0.5rem;
  }

  .callout.callout-titled .callout-icon::before {
    margin-top: .5rem;
    padding-right: .5rem;
  }

  .callout:not(.callout-titled) .callout-icon::before {
    margin-top: 1rem;
    padding-right: .5rem;
  }

  /* Callout Types */

  div.callout-note {
    border-left-color: #4582ec !important;
  }

  div.callout-note .callout-icon::before {
    background-image: url('data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAYAAABzenr0AAAAAXNSR0IArs4c6QAAAERlWElmTU0AKgAAAAgAAYdpAAQAAAABAAAAGgAAAAAAA6ABAAMAAAABAAEAAKACAAQAAAABAAAAIKADAAQAAAABAAAAIAAAAACshmLzAAAEU0lEQVRYCcVXTWhcVRQ+586kSUMMxkyaElstCto2SIhitS5Ek8xUKV2poatCcVHtUlFQk8mbaaziwpWgglJwVaquitBOfhQXFlqlzSJpFSpIYyXNjBNiTCck7x2/8/LeNDOZxDuEkgOXe++553zfefee+/OYLOXFk3+1LLrRdiO81yNqZ6K9cG0P3MeFaMIQjXssE8Z1JzLO9ls20MBZX7oG8w9GxB0goaPrW5aNMp1yOZIa7Wv6o2ykpLtmAPs/vrG14Z+6d4jpbSKuhdcSyq9wGMPXjonwmESXrriLzFGOdDBLB8Y6MNYBu0dRokSygMA/mrun8MGFN3behm6VVAwg4WR3i6FvYK1T7MHo9BK7ydH+1uurECoouk5MPRyVSBrBHMYwVobG2aOXM07sWrn5qgB60rc6mcwIDJtQrnrEr44kmy+UO9r0u9O5/YbkS9juQckLed3DyW2XV/qWBBB3ptvI8EUY3I9p/67OW+g967TNr3Sotn3IuVlfMLVnsBwH4fsnebJvyGm5GeIUA3jljERmrv49SizPYuq+z7c2H/jlGC+Ghhupn/hcapqmcudB9jwJ/3jvnvu6vu5lVzF1fXyZuZZ7U8nRmVzytvT+H3kilYvH09mLWrQdwFSsFEsxFVs5fK7A0g8gMZjbif4ACpKbjv7gNGaD8bUrlk8x+KRflttr22JEMRUbTUwwDQScyzPgedQHZT0xnx7ujw2jfVfExwYHwOsDTjLdJ2ebmeQIlJ7neo41s/DrsL3kl+W2lWvAga0tR3zueGr6GL78M3ifH0rGXrBC2aAR8uYcIA5gwV8zIE8onoh8u0Fca/ciF7j1uOzEnqcIm59sEXoGc0+z6+H45V1CvAvHcD7THztu669cnp+L0okAeIc6zjbM/24LgGM1gZk7jnRu1aQWoU9sfUOuhrmtaPIO3YY1KLLWZaEO5TKUbMY5zx8W9UJ6elpLwKXbsaZ4EFl7B4bMtDv0iRipKoDQT2sNQI9b1utXFdYisi+wzZ/ri/1m7QfDgEuvgUUEIJPq3DhX/5DWNqIXDOweC2wvIR90Oq3lDpdMIgD2r0dXvGdsEW5H6x6HLRJYU7C69VefO1x8Gde1ZFSJLfWS1jbCnhtOPxmpfv2LXOA2Xk2tvnwKKPFuZ/oRmwBwqRQDcKNeVQkYcOjtWVBuM/JuYw5b6isojIkYxyYAFn5K7ZBF10fea52y8QltAg6jnMqNHFBmGkQ1j+U43HMi2xMar1Nv0zGsf1s8nUsmUtPOOrbFIR8bHFDMB5zL13Gmr/kGlCkUzedTzzmzsaJXhYawnA3UmARpiYj5ooJZiUoxFRtK3X6pgNPv+IZVPcnwbOl6f+aBaO1CNvPW9n9LmCp01nuSaTRF2YxHqZ8DYQT6WsXT+RD6eUztwYLZ8rM+rcPxamv1VQzFUkzFXvkiVrySGQgJNvXHJAxiU3/NwiC03rSf05VBaPtu/Z7/B8Yn/w7eguloAAAAAElFTkSuQmCC');
  }

  div.callout-note.callout-style-default .callout-title {
    background-color: #dae6fb
  }

  div.callout-important {
    border-left-color: #d9534f !important;
  }

  div.callout-important .callout-icon::before {
    background-image: url('data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAYAAABzenr0AAAAAXNSR0IArs4c6QAAAERlWElmTU0AKgAAAAgAAYdpAAQAAAABAAAAGgAAAAAAA6ABAAMAAAABAAEAAKACAAQAAAABAAAAIKADAAQAAAABAAAAIAAAAACshmLzAAAEKklEQVRYCcVXTWhcVRS+575MJym48A+hSRFr00ySRQhURRfd2HYjk2SSTokuBCkU2o0LoSKKraKIBTcuFCoidGFD08nkBzdREbpQ1EDNIv8qSGMFUboImMSZd4/f9zJv8ibJMC8xJQfO3HPPPef7zrvvvnvviIkpC9nsw0UttFunbUhpFzFtarSd6WJkStVMw5xyVqYTvkwfzuf/5FgtkVoB0729j1rjXwThS7Vio+Mo6DNnvLfahoZ+i/o32lULuJ3NNiz7q6+pyAUkJaFF6JwaM2lUJlV0MlnQn5aTRbEu0SEqHUa0A4AdiGuB1kFXRfVyg5d87+Dg4DL6m2TLAub60ilj7A1Ec4odSAc8X95sHh7+ZRPCFo6Fnp7HfU/fBng/hi10CjCnWnJjsxvDNxWw0NfV6Rv5GgP3I3jGWXumdTD/3cbEOP2ZbOZp69yniG3FQ9z1jD7bnBu9Fc2tKGC2q+uAJOQHBDRiZX1x36o7fWBs7J9ownbtO+n0/qWkvW7UPIfc37WgT6ZGR++EOJyeQDSb9UB+DZ1G6DdLDzyS+b/kBCYGsYgJbSQHuThGKRcw5xdeQf8YdNHsc6ePXrlSYMBuSIAFTGAtQo+VuALo4BX83N190NWZWbynBjhOHsmNfFWLeL6v+ynsA58zDvvAC8j5PkbOcXCMg2PZFk3q8MjI7WAG/Dp9AwP7jdGBOOQkAvlFUB+irtm16I1Zw9YBcpGTGXYmk3kQIC/Cds55l+iMI3jqhjAuaoe+am2Jw5GT3Nbz3CkE12NavmzN5+erJW7046n/CH1RO/RVa8lBLozXk9uqykkGAyRXLWlLv5jyp4RFsG5vGVzpDLnIjTWgnRy2Rr+tDKvRc7Y8AyZq10jj8DqXdnIRNtFZb+t/ZRtXcDiVnzpqx8mPcDWxgARUqx0W1QB9MeUZiNrV4qP+Ehc+BpNgATsTX8ozYKL2NtFYAHc84fG7ndxUPr+AR/iQSns7uSUufAymwDOb2+NjK27lEFocm/EE2WpyIy/Hi66MWuMKJn8RvxIcj87IM5Vh9663ziW36kR0HNenXuxmfaD8JC7tfKbrhFr7LiZCrMjrzTeGx+PmkosrkNzW94ObzwocJ7A1HokLolY+AvkTiD/q1H0cN48c5EL8Crkttsa/AXQVDmutfyku0E7jShx49XqV3MFK8IryDhYVbj7Sj2P2eBxwcXoe8T8idsKKPRcnZw1b+slFTubwUwhktrfnAt7J++jwQtLZcm3sr9LQrjRzz6cfMv9aLvgmnAGvpoaGLxM4mAEaLV7iAzQ3oU0IvD5x9ix3yF2RAAuYAOO2f7PEFWCXZ4C9Pb2UsgDeVnFSpbFK7/IWu7TPTvBqzbGdCHOJQSxiEjt6IyZmxQyEJHv6xyQsYk//moVFsN2zP6fRImjfq7/n/wFDguUQFNEwugAAAABJRU5ErkJggg==');
  }

  div.callout-important.callout-style-default .callout-title {
    background-color: #f7dddc
  }

  div.callout-warning {
    border-left-color: #f0ad4e !important;
  }

  div.callout-warning .callout-icon::before {
    background-image: url('data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAYAAABzenr0AAAAAXNSR0IArs4c6QAAAERlWElmTU0AKgAAAAgAAYdpAAQAAAABAAAAGgAAAAAAA6ABAAMAAAABAAEAAKACAAQAAAABAAAAIKADAAQAAAABAAAAIAAAAACshmLzAAAETklEQVRYCeVWW2gcVRg+58yaTUnizqbipZeX4uWhBEniBaoUX1Ioze52t7sRq6APio9V9MEaoWlVsFasRq0gltaAPuxms8lu0gcviE/FFOstVbSIxgcv6SU7EZqmdc7v9+9mJtNks51NTUH84ed889/PP+cmxP+d5FIbMJmNbpREu4WUkiTtCicKny0l1pIKmBzovF2S+hIJHX8iEu3hZJ5lNZGqyRrGSIQpq15AzF28jgpeY6yk6GVdrfFqdrD6Iw+QlB8g0YS2g7dyQmXM/IDhBhT0UCiRf59lfqmmDvzRt6kByV/m4JjtzuaujMUM2c5Z2d6JdKrRb3K2q6mA+oYVz8JnDdKPmmNthzkAk/lN63sYPgevrguc72aZX/L9C6x09GYyxBgCX4NlvyGUHOKELlm5rXeR1kchuChJt4SSwyddZRXgvwMGvYo4QSlk3/zkHD8UHxwVJA6zjZZqP8v8kK8OWLnIZtLyCAJagYC4rTGW/9Pqj92N/c+LUaAj27movwbi19tk/whRCIE7Q9vyI6yvRpftAKVTdUjOW40X3h5OXsKCdmFcx0xlLJoSuQngnrJe7Kcjm4OMq9FlC7CMmScQANuNvjfP3PjGXDBaUQmbp296S5L4DrpbrHN1T87ZVEZVCzg1FF0Ft+dKrlLukI+/c9ENo+TvlTDbYFvuKPtQ9+l052rXrgKoWkDAFnvh0wTOmYn8R5f4k/jN/fZiCM1tQx9jQQ4ANhqG4hiL0qIFTGViG9DKB7GYzgubnpofgYRwO+DFjh0Zin2m4b/97EDkXkc+f6xYAPX0KK2I/7fUQuwzuwo/L3AkcjugPNixC8cHf0FyPjWlItmLxWw4Ou9YsQCr5fijMGoD/zpdRy95HRysyXA74MWOnscpO4j2y3HAVisw85hX5+AFBRSHt4ShfLFkIMXTqyKFc46xdzQM6XbAi702a7sy04J0+feReMFKp5q9esYLCqAZYw/k14E/xcLLsFElaornTuJB0svMuJINy8xkIYuL+xPAlWRceH6+HX7THJ0djLUom46zREu7tTkxwmf/FdOZ/sh6Q8qvEAiHpm4PJ4a/doJe0gH1t+aHRgCzOvBvJedEK5OFE5jpm4AGP2a8Dxe3gGJ/pAutug9Gp6he92CsSsWBaEcxGx0FHytmIpuqGkOpldqNYQK8cSoXvd+xLxXADw0kf6UkJNFtdo5MOgaLjiQOQHcn+A6h5NuL2s0qsC2LOM75PcF3yr5STuBSAcGG+meA14K/CI21HcS4LBT6tv0QAh8Dr5l93AhZzG5ZJ4VxAqdZUEl9z7WJ4aN+svMvwHHL21UKTd1mqvChH7/Za5xzXBBKrUcB0TQ+Ulgkfbi/H/YT5EptrGzsEK7tR1B7ln9BBwckYfMiuSqklSznIuoIIOM42MQO+QnduCoFCI0bpkzjCjddHPN/F+2Yu+sd9bKNpVwHhbS3LluK/0zgfwD0xYI5dXuzlQAAAABJRU5ErkJggg==');
  }

  div.callout-warning.callout-style-default .callout-title {
    background-color: #fcefdc
  }

  div.callout-tip {
    border-left-color: #02b875 !important;
  }

  div.callout-tip .callout-icon::before {
    background-image: url('data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAYAAABzenr0AAAAAXNSR0IArs4c6QAAAERlWElmTU0AKgAAAAgAAYdpAAQAAAABAAAAGgAAAAAAA6ABAAMAAAABAAEAAKACAAQAAAABAAAAIKADAAQAAAABAAAAIAAAAACshmLzAAADr0lEQVRYCe1XTWgTQRj9ZjZV8a9SPIkKgj8I1bMHsUWrqYLVg4Ue6v9BwZOxSYsIerFao7UiUryIqJcqgtpimhbBXoSCVxUFe9CTiogUrUp2Pt+3aUI2u5vdNh4dmMzOzHvvezuz8xNFM0mjnbXaNu1MvFWRXkXEyE6aYOYJpdW4IXuA4r0fo8qqSMDBU0v1HJUgVieAXxzCsdE/YJTdFcVIZQNMyhruOMJKXYFoLfIfIvVIMWdsrd+Rpd86ZmyzzjJmLStqRn0v8lzkb4rVIXvnpScOJuAn2ACC65FkPzEdEy4TPWRLJ2h7z4cArXzzaOdKlbOvKKX25Wl00jSnrwVxAg3o4dRxhO13RBSdNvH0xSARv3adTXbBdTf64IWO2vH0LT+cv4GR1DJt+DUItaQogeBX/chhbTBxEiZ6gftlDNXTrvT7co4ub5A6gp9HIcHvzTa46OS5fBeP87Qm0fQkr4FsYgVQ7Qg+ZayaDg9jhg1GkWj8RG6lkeSacrrHgDaxdoBiZPg+NXV/KifMuB6//JmYH4CntVEHy/keA6x4h4CU5oFy8GzrBS18cLJMXcljAKB6INjWsRcuZBWVaS3GDrqB7rdapVIeA+isQ57Eev9eCqzqOa81CY05VLd6SamW2wA2H3SiTbnbSxmzfp7WtKZkqy4mdyAlGx7ennghYf8voqp9cLSgKdqNfa6RdRsAAkPwRuJZNbpByn+RrJi1RXTwdi8RQF6ymDwGMAtZ6TVE+4uoKh+MYkcLsT0Hk8eAienbiGdjJHZTpmNjlbFJNKDVAp2fJlYju6IreQxQ08UJDNYdoLSl6AadO+fFuCQqVMB1NJwPm69T04Wv5WhfcWyfXQB+wXRs1pt+nCknRa0LVzSA/2B+a9+zQJadb7IyyV24YAxKp2Jqs3emZTuNnKxsah+uabKbMk7CbTgJx/zIgQYErIeTKRQ9yD9wxVof5YolPHqaWo7TD6tJlh7jQnK5z2n3+fGdggIOx2kaa2YI9QWarc5Ce1ipNWMKeSG4DysFF52KBmTNMmn5HqCFkwy34rDg05gDwgH3bBi+sgFhN/e8QvRn8kbamCOhgrZ9GJhFDgfcMHzFb6BAtjKpFhzTjwv1KCVuxHvCbsSiEz4CANnj84cwHdFXAbAOJ4LTSAawGWFn5tDhLMYz6nWeU2wJfIhmIJBefcd/A5FWQWGgrWzyORZ3Q6HuV+Jf0Bj+BTX69fm1zWgK7By1YTXchFDORywnfQ7GpzOo6S+qECrsx2ifVQAAAABJRU5ErkJggg==');
  }

  div.callout-tip.callout-style-default .callout-title {
    background-color: #ccf1e3
  }

  div.callout-caution {
    border-left-color: #fd7e14 !important;
  }

  div.callout-caution .callout-icon::before {
    background-image: url('data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAYAAABzenr0AAAAAXNSR0IArs4c6QAAAERlWElmTU0AKgAAAAgAAYdpAAQAAAABAAAAGgAAAAAAA6ABAAMAAAABAAEAAKACAAQAAAABAAAAIKADAAQAAAABAAAAIAAAAACshmLzAAACV0lEQVRYCdVWzWoUQRCuqp2ICBLJXgITZL1EfQDBW/bkzUMUD7klD+ATSHBEfAIfQO+iXsWDxJsHL96EHAwhgzlkg8nBg25XWb0zIb0zs9muYYWkoKeru+vn664fBqElyZNuyh167NXJ8Ut8McjbmEraKHkd7uAnAFku+VWdb3reSmRV8PKSLfZ0Gjn3a6Xlcq9YGb6tADjn+lUfTXtVmaZ1KwBIvFI11rRXlWlatwIAAv2asaa9mlB9wwygiDX26qaw1yYPzFXg2N1GgG0FMF8Oj+VIx7E/03lHx8UhvYyNZLN7BwSPgekXXLribw7w5/c8EF+DBK5idvDVYtEEwMeYefjjLAdEyQ3M9nfOkgnPTEkYU+sxMq0BxNR6jExrAI31H1rzvLEfRIdgcv1XEdj6QTQAS2wtstEALLG1yEZ3QhH6oDX7ExBSFEkFINXH98NTrme5IOaaA7kIfiu2L8A3qhH9zRbukdCqdsA98TdElyeMe5BI8Rs2xHRIsoTSSVFfCFCWGPn9XHb4cdobRIWABNf0add9jakDjQJpJ1bTXOJXnnRXHRf+dNL1ZV1MBRCXhMbaHqGI1JkKIL7+i8uffuP6wVQAzO7+qVEbF6NbS0LJureYcWXUUhH66nLR5rYmva+2tjRFtojkM2aD76HEGAD3tPtKM309FJg5j/K682ywcWJ3PASCcycH/22u+Bh7Aa0ehM2Fu4z0SAE81HF9RkB21c5bEn4Dzw+/qNOyXr3DCTQDMBOdhi4nAgiFDGCinIa2owCEChUwD8qzd03PG+qdW/4fDzjUMcE1ZpIAAAAASUVORK5CYII=');
  }

  div.callout-caution.callout-style-default .callout-title {
    background-color: #ffe5d0
  }

  </style>
  <style type="text/css">
    .reveal div.sourceCode {
      margin: 0;
      overflow: auto;
    }
    .reveal div.hanging-indent {
      margin-left: 1em;
      text-indent: -1em;
    }
    .reveal .slide:not(.center) {
      height: 100%;
    }
    .reveal .slide.scrollable {
      overflow-y: auto;
    }
    .reveal .footnotes {
      height: 100%;
      overflow-y: auto;
    }
    .reveal .slide .absolute {
      position: absolute;
      display: block;
    }
    .reveal .footnotes ol {
      counter-reset: ol;
      list-style-type: none; 
      margin-left: 0;
    }
    .reveal .footnotes ol li:before {
      counter-increment: ol;
      content: counter(ol) ". "; 
    }
    .reveal .footnotes ol li > p:first-child {
      display: inline-block;
    }
    .reveal .slide ul,
    .reveal .slide ol {
      margin-bottom: 0.5em;
    }
    .reveal .slide ul li,
    .reveal .slide ol li {
      margin-top: 0.4em;
      margin-bottom: 0.2em;
    }
    .reveal .slide ul[role="tablist"] li {
      margin-bottom: 0;
    }
    .reveal .slide ul li > *:first-child,
    .reveal .slide ol li > *:first-child {
      margin-block-start: 0;
    }
    .reveal .slide ul li > *:last-child,
    .reveal .slide ol li > *:last-child {
      margin-block-end: 0;
    }
    .reveal .slide .columns:nth-child(3) {
      margin-block-start: 0.8em;
    }
    .reveal blockquote {
      box-shadow: none;
    }
    .reveal .tippy-content>* {
      margin-top: 0.2em;
      margin-bottom: 0.7em;
    }
    .reveal .tippy-content>*:last-child {
      margin-bottom: 0.2em;
    }
    .reveal .slide > img.stretch.quarto-figure-center,
    .reveal .slide > img.r-stretch.quarto-figure-center {
      display: block;
      margin-left: auto;
      margin-right: auto; 
    }
    .reveal .slide > img.stretch.quarto-figure-left,
    .reveal .slide > img.r-stretch.quarto-figure-left  {
      display: block;
      margin-left: 0;
      margin-right: auto; 
    }
    .reveal .slide > img.stretch.quarto-figure-right,
    .reveal .slide > img.r-stretch.quarto-figure-right  {
      display: block;
      margin-left: auto;
      margin-right: 0; 
    }
  </style>
</head>
<body class="quarto-light">
  <div class="reveal">
    <div class="slides">

<section id="title-slide" class="quarto-title-block center">
  <h1 class="title">O Quarto como ferramenta de PKM para pesquisa científica</h1>

<div class="quarto-title-authors">
<div class="quarto-title-author">
<div class="quarto-title-author-name">
Marcus Antonio Cardoso Ramalho PPGAd-UFF 
</div>
</div>
</div>

</section>
<section id="sec-sobre-mim" class="slide level2">
<h2>Sobre mim</h2>
<div class="columns">
<div class="column" style="font-size: 30px">
<div>
<ul>
<li>Bacharel em Administração pela Universidade Federal Fluminense</li>
<li>Aluno do mestrado acadêmico em admnistração PPGAd-UFF
<ul>
<li><p>marcusantonio@id.uff.br <img data-src="https://cdn-icons-png.flaticon.com/512/6711/6711567.png" style="width:5.0%"></p></li>
<li><p>nextmarcus <a href="https://twitter.com/nextmarcus"><img data-src="https://cdn-icons-png.flaticon.com/512/124/124021.png" style="width:5.0%"></a></p></li>
<li><p>nextmarte <a href="https://github.com/nextmarte"><img data-src="https://cdn3.iconfinder.com/data/icons/sociocons/256/github-sociocon.png" style="width:6.0%"></a></p></li>
</ul></li>
</ul>
</div>
</div><div class="column" style="font-size: 30px">
<p><img data-src="https://i.pinimg.com/originals/72/4e/13/724e1305a1390ab8fe408d43e7c82b7a.jpg" style="width:50.0%"></p>
</div>
</div>
</section>
<section id="sec-quarto" class="slide level2" data-background-image="https://i.pinimg.com/originals/bb/7f/75/bb7f75f8abc5c505254d9d6830659b48.png" data-background-size="40%" data-background-opacity="30%" style="font-size: 35px">
<h2>Quarto</h2>
<div id="tabset1" class="panel-tabset">
<ul id="tabset-1" class="panel-tabset-tabby"><li><a data-tabby-default="" href="#tabset-1-1">O que é o Quarto?</a></li><li><a href="#tabset-1-2">E tem mais…</a></li></ul>
<div id="tabset1" class="tab-content">
<div id="tabset-1-1">
<ul>
<li class="fragment"><p>O Quarto é um sistema de publicação técnico-científica baseado em pandoc e markdown, proposto pela POSIT com o objetivo de unir texto e código para produzir diversos tipos de documentos como:</p>
<div>
<ul>
<li>relatórios dinâmicos;</li>
<li>páginas web;</li>
<li>posts de blogs;</li>
<li>livros, artigos científicos, apresentações e muito mais.</li>
</ul>
</div></li>
</ul>
</div>
<div id="tabset-1-2">
<div>
<ul>
<li><p>Ele é um sistema que suporta diversas linguagens de programação como R, Python, Julia e ObservableJs.</p></li>
<li><p>É versátil e por isso pode ser usado como uma das ferramentas de um sistema de PKM.</p></li>
</ul>
</div>
</div>
</div>
</div>
</section>
<section id="sec-o-que-é-pkm" class="slide level2" data-background-image="https://i.pinimg.com/564x/65/fa/34/65fa34f84a27eaa4c92ee6a32457a028.jpg" data-background-size="40%" data-background-opacity="30%" style="font-size: 35px">
<h2>O que é PKM?!</h2>
<ul>
<li class="fragment"><p>PKM significa Personal Knowledge Management, ou Gestão do conhecimento pessoal.</p></li>
<li class="fragment"><p>É o processo de gerenciar e organizar informações, conhecimento e experiências para aprimorar a tomada de decisões, a criatividade e a inovação.</p></li>
<li class="fragment"><p>O framework “Seek &gt; Sense &gt; Share” criado por Harold Jarche, é um modelo de PKM que envolve três etapas: busca de informação, interpretação e compartilhamento de conhecimento.</p></li>
</ul>
</section>
<section id="sec-o-quarto-como-ferramenta-de-pkm" class="slide level2" data-background-image="https://cdn-icons-png.flaticon.com/512/2145/2145537.png" data-background-size="30%" data-background-opacity="20%" style="font-size: 35px">
<h2>O Quarto como ferramenta de PKM</h2>
<ul>
<li class="fragment">Diversas funcionalidades que conversam com os objetivos do PKM.</li>
<li class="fragment">Permite a criação de documentos, anotações, tabelas, gráficos e visualizações de dados.</li>
<li class="fragment">Além disso, pode ser utilizado com linguagens de programação como R e Python, possibilitando a automatização de tarefas e a análise de dados.</li>
</ul>
</section>
<section id="sec-o-framework-seek---sense---share-no-quarto" class="slide level2" data-background-image="https://i.pinimg.com/originals/70/c8/f9/70c8f9820ffef5d9276811ad2627fcc3.png" data-background-size="50%" data-background-opacity="30%" style="font-size: 30px">
<h2>O framework “Seek - Sense - Share no Quarto”</h2>
<div id="tabset2" class="panel-tabset">
<ul id="tabset-2" class="panel-tabset-tabby"><li><a data-tabby-default="" href="#tabset-2-1">Seek</a></li><li><a href="#tabset-2-2">Sense</a></li><li><a href="#tabset-2-3">Share</a></li></ul>
<div id="tabset2" class="tab-content">
<div id="tabset-2-1">
<div>
<ul>
<li>O “Seek” envolve a busca e coleta de informações relevantes para a criação de novas ideias. No Quarto, é possível usar scripts em diversas linguagens, permitindo importar dados das mais diversas fontes e tipos.</li>
</ul>
</div>
</div>
<div id="tabset-2-2">
<div>
<ul>
<li>O “Sense” envolve a absorção de informações e criação de novas ideias a partir dessa base. No Quarto, as funcionalidades de edição e organização ajudam a estruturar as informações coletadas e facilitar o processo de criação do conhecimento, conectando texto e código em documentos dinâmicos por exemplo.</li>
</ul>
</div>
</div>
<div id="tabset-2-3">
<div>
<ul>
<li>O “Share” envolve o compartilhamento do conhecimento criado. No Quarto, é possível exportar e compartilhar documentos criados, bem como análises e visualizações de dados para diversos tipos de mídia como livros, artigos, blogs, apresentações, etc…</li>
</ul>
</div>
</div>
</div>
</div>
</section>
<section id="sec-primeiros-passos-no-quarto-com-rstudio." class="slide level2">
<h2>Primeiros passos no quarto com RStudio.</h2>
<!-- inicio da coluna  -->
<div class="columns">
<div class="column" style="font-size: 30px">
<p>Requisitos:</p>
<p>Ter o R, RStudio instalados e Instalar o Quarto CLI para usar comandos para instalar templates de documento ou renderizar documentos usando linha de comando por exemplo.</p>
</div><div class="column" style="width:50%;">
<p><img data-src="https://i.pinimg.com/originals/f5/21/dd/f521dd722410fbfaeeee0243809a1832.png"></p>
</div>
</div>
<!-- fim de coluna -->
<!-- inicio da parte prática da apresentação -->
</section>
<section id="sec-criando-um-documento-quarto" class="slide level2">
<h2>Criando um documento quarto</h2>
<div class="columns">
<div class="column" style="font-size: 15px">
<p>Clique em File &gt;&gt; New File &gt;&gt; Quarto document <img data-src="https://i.pinimg.com/originals/7f/2b/fc/7f2bfc3c278d57aad177f127469fd634.png" style="width:80.0%"></p>
</div><div class="column" style="font-size: 15px">
<p>Escolha o tipo de documento e preencha os campos de título e autor <img data-src="https://i.pinimg.com/originals/be/74/41/be7441a8dca36546bbb6ae6f222abd51.png" style="width:80.0%"></p>
</div>
</div>
</section>
<section id="sec-estrutura-básica-de-um-documento-e-interface" class="slide level2">
<h2>Estrutura básica de um documento e interface</h2>

<img data-src="https://i.pinimg.com/originals/af/b0/8d/afb08d6f04c0b657050db89f3f6f1026.png" class="r-stretch"></section>
<section id="sec-metadados" class="slide level2">
<h2>Metadados</h2>
<div id="tabset3" class="panel-tabset">
<ul id="tabset-3" class="panel-tabset-tabby"><li><a data-tabby-default="" href="#tabset-3-1">Estrutura</a></li><li><a href="#tabset-3-2">Exemplos</a></li></ul>
<div id="tabset3" class="tab-content">
<div id="tabset-3-1">
<div style="font-size: 25px">
<ul>
<li class="fragment">Essa é uma das partes mais importantes, principalmente quando pensamos em Seek e Share, pois nessa etapa vamos facilitar ou dificultar o acesso à informações chave do artigo por terceiros depois de publicado.</li>
<li class="fragment">Essa parte define:</li>
<li class="fragment">o tipo do documento</li>
<li class="fragment">o formato de saída</li>
<li class="fragment">as informações autorais, incluindo título, autor, afiliação, resumo, contato, etc…</li>
<li class="fragment">Elementos estruturais do documento como cores, fontes, tamanhos, etc…</li>
<li class="fragment">A maioria das definições de manuscrito podem ser sobreescritas no corpo do documento usando estilos css, HTML ou TEX por exemplo.</li>
</ul>
</div>
</div>
<div id="tabset-3-2">
<div class="columns">
<div class="column" style="width:50%;">
<p><img data-src="https://i.pinimg.com/originals/bd/53/71/bd5371acd8387b157be8f894764e6dec.png"></p>
</div><div class="column" style="width:50%;">
<p><img data-src="https://i.pinimg.com/originals/ae/aa/e7/aeaae7798d21ae437e1b320c331abee8.png"></p>
</div>
</div>
</div>
</div>
</div>
</section>
<section id="onde-encontrar-informaçãoseek" class="slide level2" style="font-size: 25px">
<h2>Onde encontrar informação?(SEEK)</h2>
<div id="tabset4" class="panel-tabset">
<ul id="tabset-4" class="panel-tabset-tabby"><li><a data-tabby-default="" href="#tabset-4-1">Pergunte</a></li><li><a href="#tabset-4-2">Quarto.org</a></li></ul>
<div id="tabset4" class="tab-content">
<div id="tabset-4-1">
<ul>
<li class="fragment">Procure os membros da comunidade</li>
<li class="fragment">Leia as referências e procure exemplos</li>
</ul>
<p><img data-src="https://i.pinimg.com/originals/a4/c2/22/a4c22234bb37f1c6357eb85154edbded.png" style="width:50.0%"></p>
</div>
<div id="tabset-4-2">
<iframe src="https://quarto.org/docs/reference/formats/ms.html#fonts" width="1800" height="500">
</iframe>
<!-- ![](https://i.pinimg.com/originals/38/13/bb/3813bb20e1e281bf626dc610b6803334.png)  -->
</div>
</div>
</div>
</section>
<section id="aprenda-fazendo-sense" class="slide level2">
<h2>Aprenda fazendo (SENSE)</h2>
<ul>
<li class="fragment">Crie um caderno de pesquisa</li>
<li class="fragment">Faça uma apresentação</li>
<li class="fragment">Escreva um texto para seu blog</li>
<li class="fragment">Escreva um livro</li>
</ul>
</section>
<section id="compartilhe-o-que-você-criou-share" class="slide level2">
<h2>Compartilhe o que você criou (Share)</h2>
<ul>
<li class="fragment">Receba feedback dos seus pares</li>
<li class="fragment">Aprenda com seus erros</li>
<li class="fragment">Construa conhecimento com quem tem menos informação</li>
<li class="fragment">Volte ao início</li>
</ul>
</section>
<section id="mãos-a-obra" class="slide level2" style="font-size: 15px">
<h2>Mãos a obra!!</h2>
<ul>
<li class="fragment">Depois de finalizar nosso artigo podemos escolher uma grande variedade de opções para compartilhamento.</li>
</ul>
<iframe src="https://quarto.org/docs/journals/formats.html" width="1800" height="500">
</iframe>
</section>
<section id="sec-boas-práticas-com-pkm" class="slide level2">
<h2>Boas práticas com PKM</h2>
<div id="tabset5" class="panel-tabset" style="font-size: 20px">
<ul id="tabset-5" class="panel-tabset-tabby"><li><a data-tabby-default="" href="#tabset-5-1">Seek</a></li><li><a href="#tabset-5-2">Sense</a></li><li><a href="#tabset-5-3">Share</a></li></ul>
<div id="tabset5" class="tab-content" style="font-size: 20px">
<div id="tabset-5-1">
<ul>
<li class="fragment">Prefira dados abertos sempre que possível para facilitar a reprodução do código apresentado no trabalho.</li>
<li class="fragment">Use ferramentas como Zotero e Mendeley integrados ao RStudio para gerenciar sua bibliografia.</li>
<li class="fragment">Organize seus scripts e outros arquivos em uma pasta específica do seu projeto.</li>
<li class="fragment">Procure templates que se encaixem no seu objetivo ou crie novos.</li>
</ul>
</div>
<div id="tabset-5-2">
<ul>
<li class="fragment">Use referências cruzadas para manter a coesão</li>
<li class="fragment">Comente todas as etapas do seu documento e dos seus scripts</li>
<li class="fragment">Evite criar muitos chunks de código entre os textos</li>
<li class="fragment">Organize seu documento para gerar insights e conectar idéias</li>
<li class="fragment">Use o github para trabalhar de forma colaborativa e revisar seu trabalho</li>
<li class="fragment">Use a opção freeze no YML para evitar recomputação</li>
</ul>
</div>
<div id="tabset-5-3">
<ul>
<li class="fragment">Pergunte a opinião dos seus pares sobre sua produção</li>
<li class="fragment">Compartilhe o que você aprendeu enquanto desenvolvia seu trabalho</li>
<li class="fragment">Não tenha medo de mostrar sesus resultados</li>
<li class="fragment">Errar faz parte do processo de construção do conhecimento</li>
</ul>
</div>
</div>
</div>
</section>
<section id="obrigado" class="title-slide slide level1 center">
<h1>Obrigado!!</h1>
<p>marcusantonio@id.uff.br<img data-src="https://cdn-icons-png.flaticon.com/512/6711/6711567.png" style="width:5.0%"></p>
<p>nextmarcus <a href="https://twitter.com/nextmarcus"><img data-src="https://cdn-icons-png.flaticon.com/512/124/124021.png" style="width:5.0%"></a></p>
<p>nextmarte <a href="https://github.com/nextmarte"><img data-src="https://cdn3.iconfinder.com/data/icons/sociocons/256/github-sociocon.png" style="width:6.0%"></a></p>
<p><img src="https://raw.githubusercontent.com/nextmarte/TalkProposal/main/img/logoSER_transparente.png" class="slide-logo"></p>
<div class="footer footer-default">
<p>Marcus Ramalho - PPGAd-UFF</p>
</div>
</section>
    </div>
  </div>

  <script>window.backupDefine = window.define; window.define = undefined;</script>
  <script src="QMD_show_files/libs/revealjs/dist/reveal.js"></script>
  <!-- reveal.js plugins -->
  <script src="QMD_show_files/libs/revealjs/plugin/quarto-line-highlight/line-highlight.js"></script>
  <script src="QMD_show_files/libs/revealjs/plugin/pdf-export/pdfexport.js"></script>
  <script src="QMD_show_files/libs/revealjs/plugin/reveal-menu/menu.js"></script>
  <script src="QMD_show_files/libs/revealjs/plugin/reveal-menu/quarto-menu.js"></script>
  <script src="QMD_show_files/libs/revealjs/plugin/quarto-support/support.js"></script>
  

  <script src="QMD_show_files/libs/revealjs/plugin/notes/notes.js"></script>
  <script src="QMD_show_files/libs/revealjs/plugin/search/search.js"></script>
  <script src="QMD_show_files/libs/revealjs/plugin/zoom/zoom.js"></script>
  <script src="QMD_show_files/libs/revealjs/plugin/math/math.js"></script>
  <script>window.define = window.backupDefine; window.backupDefine = undefined;</script>

  <script>

      // Full list of configuration options available at:
      // https://revealjs.com/config/
      Reveal.initialize({
'controlsAuto': true,
'previewLinksAuto': false,
'smaller': false,
'pdfSeparateFragments': false,
'autoAnimateEasing': "ease",
'autoAnimateDuration': 1,
'autoAnimateUnmatched': true,
'menu': {"side":"left","useTextContentForMissingTitles":true,"markers":false,"loadIcons":false,"custom":[{"title":"Tools","icon":"<i class=\"fas fa-gear\"></i>","content":"<ul class=\"slide-menu-items\">\n<li class=\"slide-tool-item active\" data-item=\"0\"><a href=\"#\" onclick=\"RevealMenuToolHandlers.fullscreen(event)\"><kbd>f</kbd> Fullscreen</a></li>\n<li class=\"slide-tool-item\" data-item=\"1\"><a href=\"#\" onclick=\"RevealMenuToolHandlers.speakerMode(event)\"><kbd>s</kbd> Speaker View</a></li>\n<li class=\"slide-tool-item\" data-item=\"2\"><a href=\"#\" onclick=\"RevealMenuToolHandlers.overview(event)\"><kbd>o</kbd> Slide Overview</a></li>\n<li class=\"slide-tool-item\" data-item=\"3\"><a href=\"#\" onclick=\"RevealMenuToolHandlers.togglePdfExport(event)\"><kbd>e</kbd> PDF Export Mode</a></li>\n<li class=\"slide-tool-item\" data-item=\"4\"><a href=\"#\" onclick=\"RevealMenuToolHandlers.keyboardHelp(event)\"><kbd>?</kbd> Keyboard Help</a></li>\n</ul>"}],"openButton":true},
'smaller': false,
 
        // Display controls in the bottom right corner
        controls: false,

        // Help the user learn the controls by providing hints, for example by
        // bouncing the down arrow when they first encounter a vertical slide
        controlsTutorial: false,

        // Determines where controls appear, "edges" or "bottom-right"
        controlsLayout: 'edges',

        // Visibility rule for backwards navigation arrows; "faded", "hidden"
        // or "visible"
        controlsBackArrows: 'faded',

        // Display a presentation progress bar
        progress: true,

        // Display the page number of the current slide
        slideNumber: false,

        // 'all', 'print', or 'speaker'
        showSlideNumber: 'all',

        // Add the current slide number to the URL hash so that reloading the
        // page/copying the URL will return you to the same slide
        hash: true,

        // Start with 1 for the hash rather than 0
        hashOneBasedIndex: false,

        // Flags if we should monitor the hash and change slides accordingly
        respondToHashChanges: true,

        // Push each slide change to the browser history
        history: true,

        // Enable keyboard shortcuts for navigation
        keyboard: true,

        // Enable the slide overview mode
        overview: true,

        // Disables the default reveal.js slide layout (scaling and centering)
        // so that you can use custom CSS layout
        disableLayout: false,

        // Vertical centering of slides
        center: false,

        // Enables touch navigation on devices with touch input
        touch: true,

        // Loop the presentation
        loop: false,

        // Change the presentation direction to be RTL
        rtl: false,

        // see https://revealjs.com/vertical-slides/#navigation-mode
        navigationMode: 'linear',

        // Randomizes the order of slides each time the presentation loads
        shuffle: false,

        // Turns fragments on and off globally
        fragments: true,

        // Flags whether to include the current fragment in the URL,
        // so that reloading brings you to the same fragment position
        fragmentInURL: false,

        // Flags if the presentation is running in an embedded mode,
        // i.e. contained within a limited portion of the screen
        embedded: false,

        // Flags if we should show a help overlay when the questionmark
        // key is pressed
        help: true,

        // Flags if it should be possible to pause the presentation (blackout)
        pause: true,

        // Flags if speaker notes should be visible to all viewers
        showNotes: false,

        // Global override for autoplaying embedded media (null/true/false)
        autoPlayMedia: null,

        // Global override for preloading lazy-loaded iframes (null/true/false)
        preloadIframes: null,

        // Number of milliseconds between automatically proceeding to the
        // next slide, disabled when set to 0, this value can be overwritten
        // by using a data-autoslide attribute on your slides
        autoSlide: 0,

        // Stop auto-sliding after user input
        autoSlideStoppable: true,

        // Use this method for navigation when auto-sliding
        autoSlideMethod: null,

        // Specify the average time in seconds that you think you will spend
        // presenting each slide. This is used to show a pacing timer in the
        // speaker view
        defaultTiming: null,

        // Enable slide navigation via mouse wheel
        mouseWheel: false,

        // The display mode that will be used to show slides
        display: 'block',

        // Hide cursor if inactive
        hideInactiveCursor: true,

        // Time before the cursor is hidden (in ms)
        hideCursorTime: 5000,

        // Opens links in an iframe preview overlay
        previewLinks: false,

        // Transition style (none/fade/slide/convex/concave/zoom)
        transition: 'none',

        // Transition speed (default/fast/slow)
        transitionSpeed: 'default',

        // Transition style for full page slide backgrounds
        // (none/fade/slide/convex/concave/zoom)
        backgroundTransition: 'none',

        // Number of slides away from the current that are visible
        viewDistance: 3,

        // Number of slides away from the current that are visible on mobile
        // devices. It is advisable to set this to a lower number than
        // viewDistance in order to save resources.
        mobileViewDistance: 2,

        // The "normal" size of the presentation, aspect ratio will be preserved
        // when the presentation is scaled to fit different resolutions. Can be
        // specified using percentage units.
        width: 1050,

        height: 700,

        // Factor of the display size that should remain empty around the content
        margin: 0.1,

        math: {
          mathjax: 'https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.0/MathJax.js',
          config: 'TeX-AMS_HTML-full',
          tex2jax: {
            inlineMath: [['\\(','\\)']],
            displayMath: [['\\[','\\]']],
            balanceBraces: true,
            processEscapes: false,
            processRefs: true,
            processEnvironments: true,
            preview: 'TeX',
            skipTags: ['script','noscript','style','textarea','pre','code'],
            ignoreClass: 'tex2jax_ignore',
            processClass: 'tex2jax_process'
          },
        },

        // reveal.js plugins
        plugins: [QuartoLineHighlight, PdfExport, RevealMenu, QuartoSupport,

          RevealMath,
          RevealNotes,
          RevealSearch,
          RevealZoom
        ]
      });
    </script>
    <script id="quarto-html-after-body" type="application/javascript">
    window.document.addEventListener("DOMContentLoaded", function (event) {
      const toggleBodyColorMode = (bsSheetEl) => {
        const mode = bsSheetEl.getAttribute("data-mode");
        const bodyEl = window.document.querySelector("body");
        if (mode === "dark") {
          bodyEl.classList.add("quarto-dark");
          bodyEl.classList.remove("quarto-light");
        } else {
          bodyEl.classList.add("quarto-light");
          bodyEl.classList.remove("quarto-dark");
        }
      }
      const toggleBodyColorPrimary = () => {
        const bsSheetEl = window.document.querySelector("link#quarto-bootstrap");
        if (bsSheetEl) {
          toggleBodyColorMode(bsSheetEl);
        }
      }
      toggleBodyColorPrimary();  
      const tabsets =  window.document.querySelectorAll(".panel-tabset-tabby")
      tabsets.forEach(function(tabset) {
        const tabby = new Tabby('#' + tabset.id);
      });
      const isCodeAnnotation = (el) => {
        for (const clz of el.classList) {
          if (clz.startsWith('code-annotation-')) {                     
            return true;
          }
        }
        return false;
      }
      const clipboard = new window.ClipboardJS('.code-copy-button', {
        text: function(trigger) {
          const codeEl = trigger.previousElementSibling.cloneNode(true);
          for (const childEl of codeEl.children) {
            if (isCodeAnnotation(childEl)) {
              childEl.remove();
            }
          }
          return codeEl.innerText;
        }
      });
      clipboard.on('success', function(e) {
        // button target
        const button = e.trigger;
        // don't keep focus
        button.blur();
        // flash "checked"
        button.classList.add('code-copy-button-checked');
        var currentTitle = button.getAttribute("title");
        button.setAttribute("title", "Copied!");
        let tooltip;
        if (window.bootstrap) {
          button.setAttribute("data-bs-toggle", "tooltip");
          button.setAttribute("data-bs-placement", "left");
          button.setAttribute("data-bs-title", "Copied!");
          tooltip = new bootstrap.Tooltip(button, 
            { trigger: "manual", 
              customClass: "code-copy-button-tooltip",
              offset: [0, -8]});
          tooltip.show();    
        }
        setTimeout(function() {
          if (tooltip) {
            tooltip.hide();
            button.removeAttribute("data-bs-title");
            button.removeAttribute("data-bs-toggle");
            button.removeAttribute("data-bs-placement");
          }
          button.setAttribute("title", currentTitle);
          button.classList.remove('code-copy-button-checked');
        }, 1000);
        // clear code selection
        e.clearSelection();
      });
      function tippyHover(el, contentFn) {
        const config = {
          allowHTML: true,
          content: contentFn,
          maxWidth: 500,
          delay: 100,
          arrow: false,
          appendTo: function(el) {
              return el.closest('section.slide') || el.parentElement;
          },
          interactive: true,
          interactiveBorder: 10,
          theme: 'light-border',
          placement: 'bottom-start'
        };
          config['offset'] = [0,0];
          config['maxWidth'] = 700;
        window.tippy(el, config); 
      }
      const noterefs = window.document.querySelectorAll('a[role="doc-noteref"]');
      for (var i=0; i<noterefs.length; i++) {
        const ref = noterefs[i];
        tippyHover(ref, function() {
          // use id or data attribute instead here
          let href = ref.getAttribute('data-footnote-href') || ref.getAttribute('href');
          try { href = new URL(href).hash; } catch {}
          const id = href.replace(/^#\/?/, "");
          const note = window.document.getElementById(id);
          return note.innerHTML;
        });
      }
      const findCites = (el) => {
        const parentEl = el.parentElement;
        if (parentEl) {
          const cites = parentEl.dataset.cites;
          if (cites) {
            return {
              el,
              cites: cites.split(' ')
            };
          } else {
            return findCites(el.parentElement)
          }
        } else {
          return undefined;
        }
      };
      var bibliorefs = window.document.querySelectorAll('a[role="doc-biblioref"]');
      for (var i=0; i<bibliorefs.length; i++) {
        const ref = bibliorefs[i];
        const citeInfo = findCites(ref);
        if (citeInfo) {
          tippyHover(citeInfo.el, function() {
            var popup = window.document.createElement('div');
            citeInfo.cites.forEach(function(cite) {
              var citeDiv = window.document.createElement('div');
              citeDiv.classList.add('hanging-indent');
              citeDiv.classList.add('csl-entry');
              var biblioDiv = window.document.getElementById('ref-' + cite);
              if (biblioDiv) {
                citeDiv.innerHTML = biblioDiv.innerHTML;
              }
              popup.appendChild(citeDiv);
            });
            return popup.innerHTML;
          });
        }
      }
    });
    </script>
    

</body></html>
