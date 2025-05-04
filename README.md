# npmtest

로컬, github action에서 npm과 pnpm으로 패키지를 다운로드 시의 퍼포먼스를 측정하기위한 프로젝트입니다.
자세한 측정결과 레포트는 해당 글 참고
https://www.murphybooks.me/projects/library/kr/000/020/020-30/kr-020-30-a/


결론은 패키지 횟수라는 요인이 반영된 경우 pnpm이 npm에 비해 큰 상대적 이점이 발생하지만 네트워크 환경이나 SSD등의 인프라 성능이 부족한 경우 pnpm의 첫 다운로드시 느려질 수 있습니다.
특히 npm 호환성에 문제가 생기는 패키지도 검증 등이 필요하기에 상황에따라 pnpm보다 npm을 사용하는 것이 적절한 경우 일 수도 있습니다.
