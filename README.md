-- шаблон файла конфигурации .stylelintrc.json --
{
  "extends": [
    "stylelint-config-standard",
    "stylelint-config-rational-order",
  ],
  "plugins": [
    "stylelint-order",
    "stylelint-config-rational-order/plugin"
  ],
  "rules": {
    "declaration-empty-line-before": null,
    "order/properties-order": [],
    "plugin/rational-order": [true, {
      "border-in-box-model": true,
      "empty-line-between-groups": true,
    }]
  }
}

-- package.json --
{
  "name": "html5-css-boilerplate",
  "version": "0.1.0",
  "description": "HTML5/CSS Boilerplate with HTMLHint and StyleLint",
  "repository": {
    "type": "git",
    "url": "https://github.com/hexlet-boilerplates/html-boilerplate.git"
  },
  "main": "",
  "devDependencies": {
    "htmlhint": "^0.16.1",
    "stylelint-config-rational-order": "^0.0.4",
    "stylelint-config-standard": "^20.0.0",
    "stylelint-order": "^4.1.0",
    "surge": "^0.23.0"
  },
  "author": "Nikita Mikhaylov",
  "license": "ISC",
  "dependencies": {
    "stylelint": "^14.1.0"
  }
}

-- моя конфигурация --

{
  "extends": [
	"stylelint-config-recommended",
    "stylelint-config-rational-order",
	"stylelint-config-html"
  ],
  "plugins": [
    "stylelint-order",
    "stylelint-config-rational-order/plugin"
  ],
  "rules": {
		"at-rule-no-unknown": true,
		"block-no-empty": true,
		"color-no-invalid-hex": true,
		"comment-no-empty": true,
		"declaration-block-no-duplicate-custom-properties": true,
		"order/properties-order": [],
		"declaration-block-no-duplicate-properties": [
			true,
			{
				"ignore": ["consecutive-duplicates-with-different-values"]
			}
		],
		"declaration-block-no-shorthand-property-overrides": true,
		"declaration-empty-line-before": [
			"never",
			{
				"ignore": ["after-comment"]
			}
		],
		"max-empty-lines": 1,
		"plugin/rational-order": [true, {
			"border-in-box-model": true,
			"empty-line-between-groups": true
		  }],
		"font-family-no-duplicate-names": true,
		"font-family-no-missing-generic-family-keyword": true,
		"function-calc-no-unspaced-operator": true,
		"function-linear-gradient-no-nonstandard-direction": true,
		"keyframe-declaration-no-important": true,
		"media-feature-name-no-unknown": true,
		"named-grid-areas-no-invalid": true,
		"no-descending-specificity": true,
		"no-duplicate-at-import-rules": true,
		"no-duplicate-selectors": true,
		"no-empty-source": true,
		"no-extra-semicolons": true,
		"no-invalid-double-slash-comments": true,
		"no-invalid-position-at-import-rule": true,
		"no-irregular-whitespace": true,
		"property-no-unknown": true,
		"rule-empty-line-before": "always-multi-line",
		"selector-pseudo-class-no-unknown": true,
		"selector-pseudo-element-no-unknown": true,
		"selector-type-no-unknown": [
			true,
			{
				"ignore": ["custom-elements"]
			}
		],
		"string-no-newline": true,
		"unit-no-unknown": true
	}
}
