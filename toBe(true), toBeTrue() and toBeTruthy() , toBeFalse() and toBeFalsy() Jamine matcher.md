### toBe(true), toBeTrue() and toBeTruthy() , toBeFalse() and toBeFalsy() Jamine matcher

1. **toBe(true)**

- `Matcher function performs the test: actual === expected`
- `Syntax: expect(flag).toBe(true | false)`
- `This test passes only if flag has the value true, in the case of expect(flag).toBe(true).` 

2. **toBeTrue()**

- `Matcher function performs the test: (actual === true || is(actual, 'Boolean') && actual.valueOf())`
- `Syntax: expect(flag).toBeTrue()`
- `This function behaves the same way as toBe(true) but handles an additional case.`
- `toBe(true) ➜ only handles a primitive boolean type.`
- `ToBeTrue() ➜ handles both a primitive boolean type and a Boolean object.`

3. **ToBeTruthy()**

- `This Boolean matcher is used in Jasmine to check whether the result is equal to true or false.`

4. **toBeFalsy()**

- `toBeFalsy() also works the same way as toBeTruthy() method. It matches the output to be false whereas toBeTruthy matches the output to be true.`

5. **toBeFalse()**

- `Matcher function performs the test: (actual === false || is(actual, 'Boolean') && actual.valueOf())`
- `Syntax: expect(flag).toBeFalse()`
- `This function behaves the same way as toBe(true) but handles an additional case.`
- `toBe(true) ➜ only handles a primitive boolean type.`
- `toBeFalse() ➜ handles both a primitive boolean type and a Boolean object.`

 

