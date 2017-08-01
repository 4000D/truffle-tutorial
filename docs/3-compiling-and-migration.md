http://truffleframework.com/docs/getting_started/compile
http://truffleframework.com/docs/getting_started/migrations


### Compile
```bash
truffle compile
```

- `./contracts` 안에 있는 컨트랙 코드를 컴파일
- `./build/contracts` 에 컴파일 된 결과물을 저장
- 이전에 컴파일 한 적이 있는 경우, 변경 사항만 다시 컴파일됨
  - 이를 원치 않으면 `truffle compile --all` 실행
- `./build/contracts` 는 artifacts 라고 불림



### Migration
```bash
truffle migration
```

- `./migrations` 디렉토리의 스크립트를 파일명 순으로 실행, 네트워크에 배포
- 컴파일과 마찬가지로 변경 사항만 반영
  - 이를 원치 않으면 `truffle migration --reset` 실행
- [다양한 기법들](http://truffleframework.com/docs/getting_started/migrations#migration-files)
  ```javascript
  // import contract
  artifacts.require(CONTRACT_TO_IMPORT)

  /**
   * deployer: stage deployment tasks
   * network: network name?
   * accounts: returned from web3.eth.getAccounts()
   */
  module.exports = function(deployer, network, accounts) { ... }
  ```
- [deployer api](deployer to stage deployment tasks)
