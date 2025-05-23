<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@lynx-js/rspeedy](./rspeedy.md) &gt; [CssModules](./rspeedy.cssmodules.md)

## CssModules interface

The [CssModules](./rspeedy.cssmodules.md) option is used for the customization of CSS Modules configurations.

**Signature:**

```typescript
export interface CssModules 
```

## Remarks

The CSS module is enabled for `*.module.css`<!-- -->, `*.module.scss` and `*.module.less`<!-- -->. Use [CssModules.auto](./rspeedy.cssmodules.auto.md) to customize the filtering behavior.

## Properties

|  Property | Modifiers | Type | Description |
|  --- | --- | --- | --- |
|  [auto?](./rspeedy.cssmodules.auto.md) |  | boolean \| RegExp \| ((filename: string) =&gt; boolean) \| undefined | _(Optional)_ The <code>auto</code> option allows CSS modules to be automatically enabled based on their filenames. |
|  [exportGlobals?](./rspeedy.cssmodules.exportglobals.md) |  | boolean \| undefined | _(Optional)_ Allows exporting names from global class names, so you can use them via import. |
|  [exportLocalsConvention?](./rspeedy.cssmodules.exportlocalsconvention.md) |  | [CssModuleLocalsConvention](./rspeedy.cssmodulelocalsconvention.md) \| undefined | _(Optional)_ The style of exported class names. |
|  [localIdentName?](./rspeedy.cssmodules.localidentname.md) |  | string \| undefined | _(Optional)_ Sets the format of the className generated by CSS Modules after compilation. |

