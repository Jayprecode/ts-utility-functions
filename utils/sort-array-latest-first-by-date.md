```ts
export const sortArrayLatestFirstByDate = <T extends { createdAt: Date | string; updatedAt?: Date | string }>(
	data: T[]
): T[] => {
	return data.sort(
		(a, b) => new Date(b.createdAt ?? b.updatedAt).getTime() - new Date(a.createdAt ?? a.updatedAt).getTime()
	);
};
```
