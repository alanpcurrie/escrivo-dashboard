<template>
    <div id="layout">
    </div>
</template>

<script>
export default {
  name: 'layout',

}
</script>



<style>

/*--------------------------------------------------------------
CSS Variables
--------------------------------------------------------------*/

:root {
  --color-white: #FFFFFF;
  --color-black: #000000;
  --color-grey:#D3D3D3;
  --color-orange:#FC4B1F;
  --color-green:#1BAF54;
}

/*--------------------------------------------------------------
CSS Reset
--------------------------------------------------------------*/


html {
    box-sizing: border-box;
    font-family: Ubuntu, sans-serif;
    -webkit-text-size-adjust: 100%;
    -ms-text-size-adjust: 100%; 
    background-color: var(--color-white);
}


body {
  margin: 1em;
  padding: 1em;
  min-height: 100vmax;
  overflow-x: hidden;
  border: 3px solid var(--color-grey);
}

h1, h2 {
  font-weight: normal;
  font-family: Montserrat, sans-serif;

}

p {
font-family: Ubuntu, sans-serif;

}

article,
aside,
details,
figcaption,
figure,
footer,
header,
main,
menu,
nav,
section,
summary {
    display: block;
}

audio,
canvas,
progress,
video {
    display: inline-block;
    vertical-align: baseline;
}

audio:not([controls]) {
    display: none;
    height: 0;
}

[hidden],
template {
    display: none;
}

a {
    background-color: transparent;
}

a:active,
a:hover {
    outline: 0;
}

abbr[title] {
    border-bottom: 1px dotted;
}

b,
strong {
    font-weight: bold;
}

dfn {
    font-style: italic;
}

h1 {
    font-size: 2em;
    margin: 0.67em 0;
}

mark {
    background: #ff0;
    color: #000;
}

small {
    font-size: 80%;
}

sub,
sup {
    font-size: 75%;
    line-height: 0;
    position: relative;
    vertical-align: baseline;
}

sup {
    top: -0.5em;
}

sub {
    bottom: -0.25em;
}

img {
    display: block;
    border: 0;
    width: 100%;
    height: auto;
}

svg:not(:root) {
    overflow: hidden;
}

figure {
    margin: 1em 40px;
}

hr {
    box-sizing: content-box;
    height: 0;
}

pre {
    overflow: auto;
}

code,
kbd,
pre,
samp {
    font-family: monospace, monospace;
    font-size: 1em;
}

button,
input,
optgroup,
select,
textarea {
    color: inherit;
    font: inherit;
    margin: 0;
}

button {
    overflow: visible;
}

button,
select {
    text-transform: none;
}

button,
html input[type="button"],
input[type="reset"],
input[type="submit"] {
    -webkit-appearance: button;
    cursor: pointer;
}

button[disabled],
html input[disabled] {
    cursor: default;
}

button::-moz-focus-inner,
input::-moz-focus-inner {
    border: 0;
    padding: 0;
}

input {
    line-height: normal;
}

input[type="checkbox"],
input[type="radio"] {
    box-sizing: border-box;
    padding: 0;
}

input[type="number"]::-webkit-inner-spin-button,
input[type="number"]::-webkit-outer-spin-button {
    height: auto;
}

input[type="search"] {
    -webkit-appearance: textfield;
    box-sizing: content-box;
}

input[type="search"]::-webkit-search-cancel-button,
input[type="search"]::-webkit-search-decoration {
    -webkit-appearance: none;
}

fieldset {
    border: 1px solid var(--color-grey);
    margin: 0 2px;
    padding: 0.35em 0.625em 0.75em;
}

legend {
    border: 0;
    padding: 0;
}

textarea {
    overflow: auto;
}

optgroup {
    font-weight: bold;
}

table {
    border-collapse: collapse;
    border-spacing: 0;
}

td,
th {
    padding: 0;
}

/*--------------------------------------------------------------
Typography
--------------------------------------------------------------*/


h1,
h2,
h3,
h4,
h5,
h6 {
	clear: both;
}

p {
	// margin-bottom: 1.5em;
}

b,
strong {
	font-weight: bold;
}

dfn,
cite,
em,
i {
	font-style: italic;
}

blockquote {
	margin: 0 1.5em;
}

address {
	margin: 0 0 1.5em;
}

pre {
	background: var(--color-grey);
	font-family: monospace;
	font-size: 15px;
	font-size: 1.5rem;
	line-height: 1.6;
	margin-bottom: 1.6em;
	max-width: 100%;
	overflow: auto;
	padding: 1.6em;
}

code,
kbd,
tt,
var {
	font: 15px  monospace;
}

abbr,
acronym {
	border-bottom: 1px dotted #666;
	cursor: help;
}

mark,
ins {
	background: #fff9c0;
	text-decoration: none;
}

sup,
sub {
	font-size: 75%;
	height: 0;
	line-height: 0;
	position: relative;
	vertical-align: baseline;
}

sup {
	bottom: 1ex;
}

sub {
	top: .5ex;
}

small {
	font-size: 75%;
}

big {
	font-size: 125%;
}
</style>
