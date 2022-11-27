# proofreading-ja

## Setting up the environment

```sh
npm install --save-dev \
    textlint \
    textlint-filter-rule-comments \
    textlint-filter-rule-whitelist \
    textlint-rule-abbr-within-parentheses \
    textlint-rule-footnote-order \
    textlint-rule-general-novel-style-ja \
    textlint-rule-ja-hiragana-fukushi \
    textlint-rule-ja-hiragana-hojodoushi \
    textlint-rule-ja-hiragana-keishikimeishi \
    textlint-rule-ja-unnatural-alphabet \
    textlint-rule-ng-word \
    textlint-rule-no-mixed-zenkaku-and-hankaku-alphabet \
    textlint-rule-period-in-list-item \
    textlint-rule-prefer-tari-tari \
    textlint-rule-preset-ja-spacing \
    textlint-rule-preset-ja-technical-writing \
    textlint-rule-preset-jtf-style \
    textlint-rule-prh \
    textlint-rule-spellcheck-tech-word \
    @textlint-ja/textlint-rule-no-insert-dropping-sa

npx textlint --init

npm install --save-dev husky
npm pkg set scripts.prepare="husky install"
npm run prepare
npx husky add .husky/pre-commit "npm run lint"
```
