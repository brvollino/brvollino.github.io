---
layout: single
title:  "How to test if an overriden TypeScript super class method has been called in the child class"
date:   2019-08-21 21:14:00 -0300
---
Here is how to test if a child class has called the super class method it has overriden.

Given these classes:
```typescript
class Parent {
  method() {
      console.log('Parent method');
  }
}

class Child extends Parent {
  method() {
      super.method();
      console.log('Child method');
  }
}
```

You would have this test:
```typescript
describe('The Child class', () => {
  it('should call the Parent method when its own method is called', () => {
    const child = new Child();
    spyOn(Parent.prototype, 'method');

    child.method();

    expect(Parent.prototype.method).toHaveBeenCalled();
  });
});
```

Got it from [this TypeScript issue](https://github.com/Microsoft/TypeScript/issues/5629).
