# 🈂 Translation Contribution Guidelines

Thank you for helping improve the translations of **TV Shows & Movies
Tracker**.\
To keep the app stable and the translations consistent, please follow
these rules carefully.

Contributions that do not follow these guidelines may be rejected.

------------------------------------------------------------------------

## ✅ What you are allowed to do

-   Translate existing values.
-   Improve wording and grammar.
-   Fix typos.
-   Adapt text naturally for your language.
-   Keep formatting consistent with the source language.

------------------------------------------------------------------------

## ❌ What you must NOT do
-   Do **not rename keys**.
-   Do **not delete keys**.
-   Do **not add new keys** without discussion.
-   Do **not change placeholders** like `{0}`, `{1}`, `{2}`.
-   Do **not remove `\n` line breaks**.
-   Do **not change XML structure**.
-   Do **not translate technical tokens, URLs, or variables**.

Only the text value should change.

------------------------------------------------------------------------

## ✅ Source of truth

The reference language is:

    English (.resx)

All other languages must match it:

-   Same keys
-   Same placeholders
-   Same line breaks

If a key is missing in your language, copy it from English and translate
only the value.

------------------------------------------------------------------------

## ✅ Placeholders and formatting

You **must keep placeholders unchanged**:

Correct:

``` xml
<string name="Login_Message">Welcome {0}</string>
```

Correct translation:

``` xml
<string name="Login_Message">Bienvenue {0}</string>
```

Wrong:

``` xml
<string name="Login_Message">Bienvenue</string>
```

Wrong:

``` xml
<string name="Login_Message">Bienvenue %s</string>
```

Also keep: - `\n` - punctuation when meaningful - spacing around
placeholders

------------------------------------------------------------------------

## ✅ File naming

Respect the format:

    strings.xx.resx

Examples: - `strings.fr.resx` - `strings.it.resx` - `strings.es.resx` -
`strings.pt-BR.resx`

Do not invent new formats without approval.

------------------------------------------------------------------------

## ✅ Encoding

-   UTF-8
-   No BOM changes
-   Keep XML valid

If your editor breaks encoding, the PR will be rejected.

------------------------------------------------------------------------

## ✅ Before submitting

Before opening a Pull Request:

-   Check XML validity.
-   Check no keys were removed.
-   Check placeholders `{0}` `{1}` are still present.
-   Check line breaks `\n`.
-   Test for obvious truncations.

------------------------------------------------------------------------

## ✅ How to contribute

1.  Fork the repository.
2.  Edit the `.resx` file for your language.
3.  Commit your changes.
4.  Open a Pull Request.
5.  Describe what you changed.

Example PR description:

    Improved Italian translations for login and settings screens.
    Fixed grammar and consistency.

------------------------------------------------------------------------

## ⚠ Quality expectations

Please avoid blind machine translation.

Try to:

-   Keep UI short.
-   Respect context.
-   Avoid overly long sentences.
-   Match the app tone.

If you are unsure about a sentence, leave a comment in the PR.

------------------------------------------------------------------------

## 🛠 Advanced contributors

If you want to:
-   Add a new language
-   Add new keys
-   Change structure

Open an Issue first before submitting code.

------------------------------------------------------------------------

## 📌 License

By contributing, you agree that your translations can be used, modified,
and distributed with the application.

------------------------------------------------------------------------

## Questions?

Open an Issue and explain what you want to improve.
