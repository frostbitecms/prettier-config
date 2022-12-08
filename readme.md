# Frostbite prettier rules <img src="https://avatars.githubusercontent.com/u/120051982?s=200&v=4" align="right" width="128" height="128">


## Install with npm

```
npm i -D @frostbitecms/prettier
```
### with yarn

```
yarn add -D @frostbitecms/prettier
```


### use in package.json

```json
{
  "prettier": "@frostbitecms/prettier"
}
```

will add the rules for the formatter


### Rationale

rule | value | reason
----|-------|----
`arrowParens` | `always` |this is for consistency, i dont really like one liners usually and will just prefer `function()` anyway, but in react this rule makes it easier to read
`bracketSameLine` | `true` | i think it looks really weird when the `>` character is on its own line
`bracketSpacing` | `true` | improves readability of object properties
`embeddedLanguageFormatting` | `auto` | its usually alright about getting this right but it isn't really a big deal to begin with
`endOfLine` | `lf` | this is for git consistency with diffs since ultimately windows is not a production environment or a "git environment"
`jsxSingleQuote`, `singleQuote` | `true` | i like to make the lines less wide so that more can fit on the screen without a horizontal scroll in a multi-window environment
`printWidth` | `90` | 80 is a bit low, 100 is too wide for multi-window workspaces but 90 is a nice middle ground
`semi` | `true` | ending a statement explicitly when you can is just better
`trailingComma` | `none` | just looks more neat when it doesn't "trail off"
`useTabs` | `true` | consistency for people's custom tab width preferences (i prefer 2 personally for the same reasons as quotes)
`quoteProps` | `as-needed` | ideally we dont need to quote object keys in sourcecode but if we need to we need to
