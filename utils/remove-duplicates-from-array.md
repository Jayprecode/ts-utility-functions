```ts
export const removeDuplicatesFromArray = <T>(arr: T[]): T[] => {
	return [...new Set(arr)];
};
```
