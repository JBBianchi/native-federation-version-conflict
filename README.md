# Illustrate version conflict

This repository illustrates a version conflict in (native federation)[https://github.com/angular-architects/module-federation-plugin/blob/main/libs/native-federation/README.md].

## How to

In parallel
- `cd remote-app && npm start`
- `cd shell-app && npm start`
- Go to http://localhost:4200

This error should appear in the console:
```
ERROR Error: NG0203: inject() must be called from an injection context such as a constructor, a factory function, a field initializer, or a function used with `runInInjectionContext`. Find more at https://angular.io/errors/NG0203
    at injectInjectorOnly (_angular_core-17_0_5-dev.js:512:11)
    at ɵɵinject (_angular_core-17_0_5-dev.js:522:59)
    at Object.factory (_angular_core-17_0_5-dev.js:15005:45)
    at _angular_core-17_0_4-dev.js:3518:33
    at runInInjectorProfilerContext (_angular_core-17_0_4-dev.js:488:5)
    at R3Injector.hydrate (_angular_core-17_0_4-dev.js:3517:9)
    at R3Injector.get (_angular_core-17_0_4-dev.js:3413:23)
    at definition.getStandaloneInjector (_angular_core-17_0_5-dev.js:15012:27)
    at ComponentFactory.create (_angular_core-17_0_4-dev.js:9287:51)
    at ViewContainerRef2.createComponent (_angular_core-17_0_4-dev.js:11455:43)
```