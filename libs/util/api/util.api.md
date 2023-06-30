## API Report File for "@gooddata/util"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts

declare namespace arrayUtils {
    export {
        shiftArrayRight
    }
}
export { arrayUtils }

// @internal
function combineGuards<T extends ((x: unknown) => x is unknown)[]>(...guards: T): (x: unknown) => x is GuardType<T[number]>;

// @internal
function delay(timeout?: number): Promise<void>;

// @internal
function escapeRegExp(value: string): string;

// @internal (undocumented)
type GuardType<T> = T extends (o: unknown) => o is infer U ? U : never;

// @internal
function hashCodeString(value: string): number;

// @internal (undocumented)
interface IShortenTextOptions {
    // (undocumented)
    maxLength?: number;
}

declare namespace objectUtils {
    export {
        shallowEqualObjects
    }
}
export { objectUtils }

// @internal
function parseStringToArray(str: string): string[] | null;

// @internal
function randomString(len: number): string;

// @internal
function removeMetadata(translationsWithMetadata: Record<string, any>): Record<string, string>;

// @internal
const sanitizeLocaleForMoment: (intlLocale: string) => string;

// @internal (undocumented)
function shallowEqualObjects(objA: Record<string, any>, objB: Record<string, any>): boolean;

// @internal
function shiftArrayRight<T>(array: Array<T>): Array<T>;

// @internal
function shortenText(value: string, options?: IShortenTextOptions): string;

// @internal
function simplifyText(value: string | number | null): string;

declare namespace stringUtils {
    export {
        shortenText,
        escapeRegExp,
        randomString,
        simplifyText,
        parseStringToArray,
        hashCodeString,
        IShortenTextOptions
    }
}
export { stringUtils }

declare namespace testUtils {
    export {
        delay
    }
}
export { testUtils }

declare namespace translationUtils {
    export {
        removeMetadata,
        sanitizeLocaleForMoment
    }
}
export { translationUtils }

declare namespace typesUtils {
    export {
        combineGuards,
        GuardType
    }
}
export { typesUtils }

```