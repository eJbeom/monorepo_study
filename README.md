# Monorepo_study 개요
pnpm workspace(monorepo)를 사용하여 library, frontend 개발 환경 구축해보기.

## Configuration
- root에서 eslint+prettier 를(을) 관리합니다. 모든 패키지에 적용됩니다.
- git hook(husky)를 사용해 커밋 전 변경 된 파일에만 eslint+prettier 를 자동 적용합니다.
- "lib": "workspace:*" -> library 배포 없이 examples에 심볼릭 링크로 연결되어 빠른 개발이 가능합니다.

## Use case
서로 자주 상호작용하는 lib와 front 개발을 동시에 개발해야 할 때

## Problems
규모가 커지면(팀 프로젝트 등) 개발 복잡성 증가
