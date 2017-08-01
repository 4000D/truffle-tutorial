http://truffleframework.com/docs/getting_started/project

```bash
# 샘플 프로젝트를 위한 디렉토리 생성 후 이동
mkdir SampleProject && cd SampleProject

# truffle 프로젝트 initialize
truffle init

# 기본적으로 contracts, migrations, test 디렉토리와 truffle.js 파일이 생성됨
```

- `contracts/`: solidity contract codes
- `migrations/`: 배포를 위한 스크립트 파일들
- `test/`: 테스트 파일들 (js test, sol test)
- `truffle.js`: Truffle configuration file


### truffle 프로젝트 initialize 하는 다른 방법
1. [`truffle init webpack`](https://github.com/trufflesuite/truffle-init-webpack)
  - 웹팩이 사전 설정된 truffle 프로젝트

2. [`truffle unbox react`](https://github.com/truffle-box/react-box)
  - 웹팩, 리액트가 사전 설정된 truffle 프로젝트
  - unbox 명령어 식별 안될 시 truffle 업데이트   (`npm install -g truffle`)
