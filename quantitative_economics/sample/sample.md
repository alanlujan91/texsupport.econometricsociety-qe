---
title: A sample article title
short_title: A sample running head title
authors:
  - name: First Author
    affiliations:
      - Department of Economics, University of Somewhere
    email: first@somewhere.com
  - name: Second Author
    affiliations:
      - Department of Economics, Another University
    email: second@somewhere.com
  - name: Third Author
    affiliations:
      - Department of Economics, Yet Another University
    email: third@somewhere.com
keywords:
  - First keyword
  - second keyword
  - third keyword
bibliography: references.bib
exports:
  - format: pdf+tex
    template: ../template.tex
    article_type: qe
    citation_style: nameyear
    draft: true
---

+++ {"part": "abstract"}
The abstract should summarize the contents of the paper. It should be clear,
descriptive, self-explanatory and not longer than 150 words. It should also be
suitable for publication in abstracting services. Please avoid using math formulas
as much as possible. We recommend 3--8 keywords and up to 3 JEL codes.
+++

+++ {"part": "support"}
We thank four anonymous referees. The Editor should not be thanked anonymously or by name in this footnote, or elsewhere in the paper. The first author gratefully acknowledges
financial support from the National Science Foundation through Grant XXX-0000000.
+++

+++ {"part": "coeditor"}
[Name Surname; will be inserted later]
+++

+++ {"part": "jel"}
First JEL
second JEL
+++

# Introduction {#s1}

This template helps you to create a properly formatted manuscript.
Prepare your paper in the same style as used in this sample file.
Try to avoid excessive use of italics and bold face; underlining is generally banned (except for exceptional cases). Please do not use any commands that affect the layout or formatting of your document (i.e., commands like `\textheight`, `\textwidth`, etc.). Note that the Introduction should be Section {#s1} it should not immediately follow the abstract without a heading.

# Section headings

Here are some subsections:

## A subsection

Regular text.

### A subsubsection

Regular text.

#### Paragraph heading

If you want to add mini-headings for paragraphs without numbers please use `\paragraph*{}`.

# Text

## Lists

The following is an example of an *itemized* list, two levels deep:

- This is the first item of an itemized list. Each item in the list is marked with a "tick." The document style determines what kind of tick mark is used.
- This is the second item of the list. It contains another list nested inside of it.
  - This is the first item of an itemized list that is nested within the itemized list.
  - This is the second item of the inner list. LaTeX allows you to nest lists deeper than you really should.
  This is the rest of the second item of the outer list.
- This is the third item of the list.

The following is an example of an *enumerated* list, two levels deep:

(i) This is the first item of an enumerated list. Each item in the list is marked with a "tick." The document style determines what kind of tick mark is used.
(ii) This is the second item of the list. It contains another list nested inside of it.
    1. This is the first item of an enumerated list that is nested within.
    2. This is the second item of the inner list. LaTeX allows you to nest lists deeper than you really should.
    This is the rest of the second item of the outer list.
(iii) This is the third item of the list.

Do not use (1), (2), etc. for items in order to avoid confusion with numbered equations.

## Punctuation

Avoid unnecessary hyphenation; many hyphenated words can be treated as one or two words.
Dashes come in three sizes: a hyphen, an intra-word dash like "$U$-statistics" or "the time-homogeneous model";
a medium dash (also called an "en-dash") for number ranges or between two equal entities like "1--2" or "Cauchy--Schwarz inequality";
and a punctuation dash (also called an "em-dash") in place of a comma, semicolon,
colon or parentheses---like this.

Generating an ellipsis ... with the right spacing around the periods requires using `\ldots`.

*Quantitative Economics* is using longer spaces after periods, please add `\` after periods that are not at the end of a sentence, in order to have regular spaces. For example, if there is an abbreviation (e.g., econ. theory) which is not the end of an article but appears in a middle of a sentence, please code it as `(e.g., econ.\ theory)`.

## Citation

Only include in the reference list entries for which there are text citations,
and make sure all citations are included in the reference list.
Simple author and year cite: @aiyagari1994uninsured.
Multiple bibliography items cite: [@krusell1998income; @fernandez2016solving].

## Fonts

Please use text fonts in text mode, e.g.:

- Roman `\textrm{}`
- *Italic* `\textit{}`
- **Bold** `\textbf{}`
- Small Caps `\textsc{}`
- Sans serif `\textsf{}`
- `Typewriter` `\texttt{}`

Please use mathematical fonts in mathematical mode, e.g.:

- $\mathrm{ABCabc123}$ `\mathrm{}`
- $\mathit{ABCabc123}$ `\mathit{}`
- $\mathbf{ABCabc123}$ `\mathbf{}`
- $\boldsymbol{ABCabc123\alpha\beta\gamma}$ `\boldsymbol{}`
- $\mathcal{ABC}$ `\mathcal{}`
- $\mathbb{ABC}$ `\mathbb{}`
- $\mathsf{ABCabc123}$ `\mathsf{}`
- $\mathtt{ABCabc123}$ `\mathtt{}`
- $\mathfrak{ABCabc123}$ `\mathfrak{}`

Note that `\mathcal, \mathbb` belongs to capital letters-only font typefaces.

## Notes

Footnotes[^1] pose no problems in text.[^2] Please do not add footnotes on math.

[^1]: This is an example of a footnote.
[^2]: Note that footnote number is after punctuation.

## Numbers

A decimal point always should be preceded by a whole number and never should be left "naked." Decimal expressions of numbers less than 1 always should be preceded by a zero (0) to enhance the visibility of the decimal. For example, .3 should be 0.3. This applies to text, tables, and figures.

## Quotations

Text is displayed by indenting it from the left margin. There are short quotations:

> This is a short quotation. It consists of a single paragraph of text. There is no paragraph indentation. It should be coded between `\begin{quote}` and `\end{quote}`.

and longer ones:

> This is a longer quotation. It consists of two paragraphs of text. The beginning of each paragraph is indicated by an extra indentation.
>
> This is the second paragraph of the quotation. It is just as dull as the first paragraph. It should be coded between `\begin{quotation}` and `\end{quotation}`.

## Environments

Please use regular counters (Theorem 1) as opposed to counters belonging on sections (Theorem 3.1). Results (Lemmas, Propositions, Theorems, Claims) can be on the same or different counters.

### Examples for *plain*-style environments

:::{admonition} Theorem 1
:class: theorem

This is the body of Theorem 1.
:::

:::{admonition} Proof
:class: proof

This is the body of the proof of the theorem above.
:::

:::{admonition} Claim 1
:class: claim

This is the body of Claim 1.
:::

:::{admonition} Axiom 1
:class: axiom

This is the body of Axiom 1. Axioms should be on a different counter from results (e.g. Theorems, Propositions, Lemmas).
:::

:::{admonition} Theorem 2 (Title of the Theorem)
:class: theorem

This is the body of Theorem 2. Theorem 2 has additional title.
:::

:::{admonition} Lemma 1
:class: lemma

This is the body of Lemma 1. Lemma 1 is numbered after Theorem 2 because we used `[theorem]` in `\newtheorem`.
:::

:::{admonition} Fact
:class: fact

This is the body of the fact. Fact is unnumbered because we used the command `\newtheorem*` instead of `\newtheorem`.
:::

:::{admonition} Proof of Theorem 2
:class: proof

This is the body of the proof of Theorem 2.
:::

### Examples for *remark*-style environments

The following environments can be numbered or not; if numbered, they should be on different counters from results.

:::{admonition} Definition 1
:class: definition

This is the body of Definition 1. Definitions should be on a different counter from results (e.g. Theorems, Propositions, Lemmas).
:::

:::{admonition} Example
:class: example

This is the body of the example. Example is unnumbered because we used `\newtheorem*` instead of `\newtheorem`.
:::

:::{admonition} Remark
:class: remark

This is the body of the remark.
:::

# Equations and the like

Only number equations to which there is a subsequent reference.
See equations below {eq}`ccs`--{eq}`e7`. Please punctuate equations as you would punctuate a sentence, that is add a comma between two equations and add a period if it ends a sentence.

Two equations:

```{math}
:label: ccs
C_{s} = K_{M} \frac{\mu/\mu_{x}}{1-\mu/\mu_{x}}
```

and

```{math}
G = \frac{P_{\mathrm{opt}} - P_{\mathrm{ref}}}{P_{\mathrm{ref}}} 100(\%).
```

Equation arrays:

```{math}
\begin{aligned}
\frac{dS}{dt} &= -\sigma X + s_{F} F, \\
\frac{dX}{dt} &= \mu X, \\
\frac{dP}{dt} &= \pi X - k_{h} P, \\
\frac{dV}{dt} &= F.
\end{aligned}
```

One long equation, note that the equation number is on the last line:

```{math}
:label: e7
\begin{aligned}
\mu_{\text{normal}} &= \mu_{x} \frac{C_{s}}{K_{x}C_{x}+C_{s}} \\
&= \mu_{\text{normal}} - Y_{x/s}\bigl(1-H(C_{s})\bigr)(m_{s}+\pi /Y_{p/s}) \\
&= \mu_{\text{normal}}/Y_{x/s}+ H(C_{s}) (m_{s}+ \pi /Y_{p/s}).
\end{aligned}
```

Note that variables made of more than one letter should use command `\mathit`,
e.g., $\mathit{sov}=550$, where $\mathit{sov}$ is sum of votes. Abbreviations used in subscripts or superscripts should use `\mathrm`,
e.g., $t_{\mathrm{max}}-t_{\mathrm{min}} =10$. Operator names should use `\operatorname`, e.g. $\operatorname{AR}(1)$. Also, note that $\emptyset$ symbol is preferred to $\varnothing$.

# Tables and figures

Cross-references to labeled tables: As you can see in Table {#sphericcase} and also in Table {#parset}.

Sample of cross-reference to figure: Figure {#penG} shows that it is not easy to get something on paper. Note that figures will be in grayscale in the printed version.

:::{table} The spherical case ($I_1=0$, $I_2=0$).
:name: sphericcase

| Equil. Points | $x$ | $y$ | $z$ | $C$ | S |
|---------------|-----|-----|-----|-----|---|
| $L_1$ | $-$2.485252241 | 0.000000000 | 0.017100631 | 8.230711648 | U |
| $L_2$ | 0.000000000 | 0.000000000 | 3.068883732 | 0.000000000 | S |
| $L_3$ | 0.009869059 | 0.000000000 | 4.756386544 | $-$0.000057922 | U |
| $L_4$ | 0.210589855 | 0.000000000 | $-$0.007021459 | 9.440510897 | U |
| $L_5$ | 0.455926604 | 0.000000000 | $-$0.212446624 | 7.586126667 | U |
| $L_6$ | 0.667031314 | 0.000000000 | 0.529879957 | 3.497660052 | U |
| $L_7$ | 2.164386674 | 0.000000000 | $-$0.169308438 | 6.866562449 | U |
| $L_8$ | 0.560414471 | 0.421735658 | $-$0.093667445 | 9.241525367 | U |
| $L_9$ | 0.560414471 | $-$0.421735658 | $-$0.093667445 | 9.241525367 | U |
| $L_{10}$ | 1.472523232 | 1.393484549 | $-$0.083801333 | 6.733436505 | U |
| $L_{11}$ | 1.472523232 | $-$1.393484549 | $-$0.083801333 | 6.733436505 | U |

This is how table note should be presented.
Please do not use asterisks or bold face to denote statistical significance.
We encourage authors to report standard errors and coverage sets or confidence intervals.
:::

:::{table} Sample posterior estimates for each model.
:name: parset

| Model | Parameter | Mean | Std. Dev. | 2.5% | 50% | 97.5% |
|-------|-----------|------|-----------|------|-----|--------|
| Model 0 | $\beta_0$ | $-$12.29 | 2.29 | $-$18.04 | $-$11.99 | $-$8.56 |
|         | $\beta_1$ | 0.10 | 0.07 | $-$0.05 | 0.10 | 0.26 |
|         | $\beta_2$ | 0.01 | 0.09 | $-$0.22 | 0.02 | 0.16 |
| Model 1 | $\beta_0$ | $-$4.58 | 3.04 | $-$11.00 | $-$4.44 | 1.06 |
|         | $\beta_1$ | 0.79 | 0.21 | 0.38 | 0.78 | 1.20 |
|         | $\beta_2$ | $-$0.28 | 0.10 | $-$0.48 | $-$0.28 | $-$0.07 |
| Model 2 | $\beta_0$ | $-$11.85 | 2.24 | $-$17.34 | $-$11.60 | $-$7.85 |
|         | $\beta_1$ | 0.73 | 0.21 | 0.32 | 0.73 | 1.16 |
|         | $\beta_2$ | $-$0.60 | 0.14 | $-$0.88 | $-$0.60 | $-$0.34 |
|         | $\beta_3$ | 0.22 | 0.17 | $-$0.10 | 0.22 | 0.55 |
:::

\begin{figure}[!htbp]
\centering
\includegraphics[width=0.7\linewidth]{files/figure_sample.pdf}

\caption{The dotted lines show the values of $u(x)$ for $x$ in the discrete support of $F$. The solid lines show $u_\textrm{conv}(x)$.}
\label{penG}
\end{figure}

+++ {"part": "appendix"}
(appendix)=
# Appendix

Appendices should be provided in `{appendix}` environment. If there is only one appendix,
then please refer to it in text as ... in the [Appendix](#appendix).

(appendixA)=
# First Appendix

If there are more than one appendix, then please refer to it
as ... in [Appendix A](#appendixA), [Appendix B](#appendixB), etc.

(appendixB)=
# Second Appendix

(appendixB1)=
## First subsection of Appendix [B](#appendixB)

If your appendix is long, make sure to divide it into subsections and refer to them in text. Use the standard LaTeX commands for headings in `{appendix}`.
Headings and other objects will be numbered automatically.

```{math}
:label: path
\mathcal{P}=(j_{k,1},j_{k,2},\dots,j_{k,m(k)}).
```

Sample of cross-reference to formula {eq}`path` in [Appendix B.1](#appendixB1).
Note that it is better to refer to [Appendix B.1](#appendixB1) as opposed to [Appendix B](#appendixB), because it is easier for the reader to locate the necessary place.
+++ 