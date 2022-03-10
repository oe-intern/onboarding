```

function isEven() {
  const button = document.getElementById('button');
  const input = document.getElementById('input');

  button.onClick(function() {
    if (input.value % 2 === 0) {
      console.log('true');
      return;
    }

    console.log('false');
    return;
  });
};
```

A good function should be
```
function isEven(x) {
  return !!x % 2;
}

function main() {
  const button = document.getElementById('button');
  const input = document.getElementById('input');

  button.onClick(function() {
    return isEven(input.value);
  });
}
```

Write a test

```
expect(isEven(1)).toBe(false);
expect(isEven(2)).toBe(true);
expect(isEven(-1)).toBe(false);
```
