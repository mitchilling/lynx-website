<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@lynx-js/react/testing-library](./react-lynx-testing-library.md) &gt; [RenderHookResult](./react-lynx-testing-library.renderhookresult.md)

## RenderHookResult interface

The result of [renderHook()](./react-lynx-testing-library.renderhook.md)

**Signature:**

```typescript
export interface RenderHookResult<Result, Props>
```

## Properties

| Property                                                              | Modifiers | Type                       | Description                                                                                             |
| --------------------------------------------------------------------- | --------- | -------------------------- | ------------------------------------------------------------------------------------------------------- |
| [rerender](./react-lynx-testing-library.renderhookresult.rerender.md) |           | (props?: Props) =&gt; void | Triggers a re-render. The props will be passed to your renderHook callback.                             |
| [result](./react-lynx-testing-library.renderhookresult.result.md)     |           | { current: Result; }       | This is a stable reference to the latest value returned by your renderHook callback                     |
| [unmount](./react-lynx-testing-library.renderhookresult.unmount.md)   |           | () =&gt; void              | Unmounts the test component. This is useful for when you need to test any cleanup your useEffects have. |
