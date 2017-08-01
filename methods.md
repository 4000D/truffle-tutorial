## artifactor.saveAll()
https://github.com/trufflesuite/truffle-migrate/blob/15134317417a032a0ef91525a30e85a2b2bc84a2/index.js#L60

truffle package | function name    | arguments                               | description
----------------|------------------|-----------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------
resolver        | require          | import_path, search_path                | .sol 파일을 읽음 (fs.readFile)
resolver        | resolve          | import_path, imported_from              | npm, ethpm 패키지를 읽음
contract-schema | normalizeOptions | options, extra_opetions                 | contract 에서 사용되지 않는 불필요한 key-value 제거
contract-schema | generateBinary   | options, existing_binary, extra_options | normalizeOptions 에서 적절한 binary 를 생성함
contract        | default          | options                                 | binary 에서 [TruffleContract](https://github.com/trufflesuite/truffle-contract/blob/master/contract.js#L570) 객체 생성
deployer        | deploy           | contract, args                          | [컴파일 된 json 에서 Truffle Contract 객체 생성 후 네트워크에 배포 후 반환](https://github.com/trufflesuite/truffle-deployer/blob/master/src/actions/deploy.js)
