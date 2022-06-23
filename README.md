# Error:

```
[!] The following Swift pods cannot yet be integrated as static libraries:

The Swift pod `FirebaseCoreInternal` depends upon `GoogleUtilities`, which does not define modules. To opt into those targets generating module maps (which is necessary to import them from Swift when building as static libraries), you may set `use_modular_headers!` globally in your Podfile, or specify `:modular_headers => true` for particular dependencies.
```

# How to reproduce

1. `git clone git@github.com:RodolfoGS/FirebaseCoreInternal-issue.git`
2. `cd FirebaseCoreInternal-issue/`
3. `npm i`
4. `cd ios`
5. `pod install`
6. Error happens
