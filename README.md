# Install Plugins

```bash
$ yarn
```

<br>

## Gulp

### Dev

```bash
$ gulp
```

### Production

```bash
$ gulp --env production
```

---

# 參考 Vue core 的 tsconfig.json

https://github.com/vuejs/core/blob/main/tsconfig.json

```json
{
  "compilerOptions": {
    "baseUrl": ".",
    "outDir": "temp",
    "sourceMap": false,
    "target": "es2016",
    "newLine": "LF",
    "useDefineForClassFields": false,
    "module": "esnext",
    "moduleResolution": "node",
    "allowJs": false,
    "strict": true,
    "noUnusedLocals": true,
    "experimentalDecorators": true,
    "resolveJsonModule": true,
    "isolatedModules": true,
    "skipLibCheck": true,
    "esModuleInterop": true,
    "removeComments": false,
    "jsx": "preserve",
    "lib": ["esnext", "dom"],
    "types": ["vitest/globals", "puppeteer", "node"],
    "rootDir": ".",
    "paths": {
      "@vue/compat": ["packages/vue-compat/src"],
      "@vue/*": ["packages/*/src"],
      "vue": ["packages/vue/src"]
    }
  },
  "include": [
    "packages/global.d.ts",
    "packages/*/src",
    "packages/runtime-dom/types/jsx.d.ts",
    "packages/*/__tests__",
    "packages/dts-test"
  ]
}
```
