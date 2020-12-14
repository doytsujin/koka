adown: []{.fa .fa-angle-double-down}
aup:   []{.fa .fa-angle-double-up}

.title {
  font-size: xxx-large;
}

toc {
  .expand-all;
}

toc.toc-contents {
  before:clear;
}

.math-inline {
  input: mathpre;
}

.pre-fenced3, .code1 {
  language: koka;
}

.pre-indented, .console {
  replace: "/^( *>[^\n\r]+)/\(**``\1``**\)/mg";
}

.mapsto {
  padding: 0ex 1em;
  align-self: center;
  font-size: 125%;
}

.learn {
  .button;
}

@if preview {
  .code1 {
    border-bottom: 1px solid green;
  }

  .pre-fenced3 {
    border-left: 0.5ex solid green;
  }

  .token.predefined {
    color: navy;
  }
}

h4 {
  @h1-h2-h3-h4: upper-alpha;
}

.toc, h1, h2, h3, h4, h5 {
  font-family: 'Nunito', 'Segoe UI', sans-serif;
}

li {
  margin-bottom: 1ex;
}

.note {
  font-style: italic;
}

.advanced {
  .boxed;
  before: "[advanced]{.boxed-label}";
}

.translate {
  .boxed;
  replace: "[translation]{.boxed-label}&nl;~begin translate-row&nl;&source;&nl;~end translate-row&nl;";
}

.boxed {
  border: 1px solid #AAA;
  padding: 0em 1em;  
}

.boxed-label {
  display: block;
  float: left;
  margin: -1.5em 0em -1em -1em;
  font-size: 70%;
  color: #999;
}

.banner {
  before: "[&caption;]{.banner-caption}";
}