http://truffleframework.com/docs/getting_started/testing

### 0. Common

```bash
truffle test # ./test 디렉토리에 있는 파일들 테스트
truffle test ./path/to/file # 특정 파일 대상 테스트
```
테스트 대상 파일 확장자: `.sol`, `.js`, `.es`, `.es6`, `.jsx`

### 1. JavaScript Application Test
관련 프레임워크 / 라이브러리
- [Mocha](https://mochajs.org/)
```javascript
describe('Array', function() {
  describe('#indexOf()', function() {
    it('should return -1 when the value is not present', function() {
      assert.equal(-1, [1,2,3].indexOf(4));
    });
  });
});
```
- [Chai](http://chaijs.com/)
```javascript
foo.should.be.a('string');
foo.should.equal('bar');
foo.should.have.lengthOf(3);
tea.should.have.property('flavors')
  .with.lengthOf(3);
```

자세한 내용은 [여기](http://truffleframework.com/docs/getting_started/javascript-tests#use-contract-instead-of-describe-)부터


### 2. Solidity Contract Test
작성중...
