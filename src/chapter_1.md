# Chapter 1

Testing [mdbook-gettext](https://github.com/google/mdbook-i18n-helpers)
with [mdbook-katex](https://github.com/lzanini/mdbook-katex).

This is an example of inline latex $ \pi(\theta)$ which should render as expected.

This shows that `skip` instruction does not work on inline latex snippet <!-- i18n:skip --> $\pi(\theta)$.

This is an example Latex block that generates too many
gettext entries.

$$
\begin{array}{|c|c|c|c|c|}
\hline
1 & x_1 & x_2 & x_3 & out \\
\hline
0 & 1 & 1 & 0 & 0 \\
\hline
\end{array}
$$

This is an example Latex block with `skip` instruction which works as expected.
<!-- i18n:skip --> $$
\begin{array}{|c|c|c|c|c|}
\hline
1 & x_1 & x_2 & x_3 & out \\
\hline
0 & 1 & 1 & 0 & 0 \\
\hline
\end{array}
$$
