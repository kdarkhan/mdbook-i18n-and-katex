# POC for making mdbook-i18n-helpers work with mdbook-katex

Pre-built versions of the books are available in Pages
[here](https://kdarkhan.github.io/mdbook-i18n-and-katex/).

I created this repo while investigating
[mdbook-i18n-helpers/issues/105](https://github.com/google/mdbook-i18n-helpers/issues/105).

This shows how to make [mdbook-i18n-helpers](https://github.com/google/mdbook-i18n-helpers)
work with [mdbook-katex](https://github.com/lzanini/mdbook-katex).

If `mdbook-katex` is executed before `mdbook-gettext`, then most of the things work as
expected. `mdbook-gettext` starts parsing `MathJax` HTML elements and generates often
redundant entries which can be seen from `po/messages.pot`. There is a way to bypass
it by skipping translations for Latex blocks by putting `i18n:skip` comments. However,
that does not seem to work for inline Latex at the moment.
