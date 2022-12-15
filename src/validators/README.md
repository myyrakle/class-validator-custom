
example
```
// allow [[1,2], [3,4], [5,6], [7,8]]
export class RequestDto {
  @ArrayLength({ depth: 1, length: 4 })
  @ArrayLength({ depth: 2, length: 2 })
  @IsArrayOfType({ depth: 2, elementType: Number })
  foo: number[][];
}
```

