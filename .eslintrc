module.exports = {
  root: true,
  env: { browser: true, es6: true },
  parser: "@typescript-eslint/parser",
  parserOptions: {
    sourceType: "module",
    extends: "./tsconfig.json",
    extraFileExtensions: [".svelte"],
    ecmaVersion: 2020,
    ecmaFeatures: {
      jsx: true,
      modules: true,
    },
  },
  plugins: ["svelte3", "@typescript-eslint"],
  extends: ["eslint:recommended", "plugin:@typescript-eslint/recommended"],
  overrides: [
    {
      files: ["*.svelte"],
      processor: "svelte3/svelte3",
    },
  ],
  globals: {
    Atomics: "readonly",
    SharedArrayBuffer: "readonly",
  },
  rules: {
    "@typescript-eslint/ban-ts-comment": "off",
    "@typescript-eslint/explicit-module-boundary-types": "off",
    "@typescript-eslint/explicit-function-return-type": "off",
    "@typescript-eslint/no-empty-interface": [
      "error",
      {
        allowSingleExtends: true,
      },
    ],
    "@typescript-eslint/no-explicit-any": "off",
    "@typescript-eslint/no-non-null-assertion": "off",
    "@typescript-eslint/no-use-before-define": "off",
    "@typescript-eslint/no-var-requires": "off",
    "@typescript-eslint/no-shadow": "off",
    "no-undef": "off",
    "no-unused-vars": "off",
    "no-use-before-define": "off",
    "no-shadow": "off",
    "require-await": "error",
  },
  settings: {
    "svelte3/typescript": true, // load TypeScript as peer dependency
  },
  ignorePatterns: ["src/api/*", "node_modules"],
};
