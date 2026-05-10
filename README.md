# @oiij/tsconfig

My shared TypeScript configuration.

## Usage

```bash
pnpm add -D @oiij/tsconfig
```

Extend in your `tsconfig.json`:

```json
{
  "extends": "@oiij/tsconfig"
}
```

## Compiler Options

| Option | Value | Description |
| --- | --- | --- |
| `target` | `ESNext` | 最新 ECMAScript 特性 |
| `module` | `ESNext` | ES 模块系统 |
| `moduleResolution` | `bundler` | 适配 Vite / webpack / esbuild 等打包工具 |
| `jsx` | `preserve` | 保留 JSX 语法，交给框架处理 |
| `lib` | `ESNext`, `DOM` | 支持最新语法和浏览器 DOM API |
| `isolatedModules` | `true` | 确保每个文件可独立编译，打包工具必需 |
| `resolveJsonModule` | `true` | 允许导入 JSON 文件 |
| `resolvePackageJsonExports` | `true` | 支持 package.json `exports` 字段 |
| `allowJs` | `true` | 允许编译 JavaScript 文件 |
| `strict` | `true` | 启用所有严格类型检查 |
| `noUncheckedIndexedAccess` | `true` | 索引访问自动包含 `undefined` |
| `noUnusedLocals` | `true` | 检查未使用的局部变量 |
| `noUnusedParameters` | `true` | 检查未使用的函数参数 |
| `noImplicitReturns` | `true` | 确保所有代码路径都有返回值 |
| `noImplicitOverride` | `true` | 要求使用 `override` 关键字显式重写父类方法 |
| `noPropertyAccessFromIndexSignature` | `true` | 索引签名访问必须使用方括号语法 |
| `exactOptionalPropertyTypes` | `true` | 区分 `undefined` 和缺失属性 |
| `noFallthroughCasesInSwitch` | `true` | 防止 switch 穿透 |
| `esModuleInterop` | `true` | 兼容 CommonJS 默认导出 |
| `forceConsistentCasingInFileNames` | `true` | 文件名大小写一致性 |
| `skipLibCheck` | `true` | 跳过 `.d.ts` 类型检查 |