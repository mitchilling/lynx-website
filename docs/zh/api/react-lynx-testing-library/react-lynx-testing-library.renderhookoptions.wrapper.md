<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@lynx-js/react/testing-library](./react-lynx-testing-library.md) &gt; [RenderHookOptions](./react-lynx-testing-library.renderhookoptions.md) &gt; [wrapper](./react-lynx-testing-library.renderhookoptions.wrapper.md)

## RenderHookOptions.wrapper property

Pass a React Component as the wrapper option to have it rendered around the inner element. This is most useful for creating reusable custom render functions for common data providers. See setup for examples.

**Signature:**

```typescript
wrapper?: ComponentType<{ children: LynxElement }>;
```

## Example

```ts
import { renderHook } from '@lynx-js/react/testing-library'
import { ThemeProvider } from 'my-ui-lib'
import { TranslationProvider } from 'my-i18n-lib'
import defaultStrings from 'i18n/en-x-default'

const AllTheProviders = ({children}) => {
  return (
    <ThemeProvider theme="light">
      <TranslationProvider messages={defaultStrings}>
        {children}
      </TranslationProvider>
    </ThemeProvider>
  )
}

const customRenderHook = (ui, options) =>
  renderHook(ui, { wrapper: AllTheProviders, ...options })

// re-export everything
export * from '@lynx-js/react/testing-library'

// override renderHook method
export { customRender as renderHook }
```
