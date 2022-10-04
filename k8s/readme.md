- Prometheus operator로 배포
- helm diff plugin 설치: helm upgrade 명령어에 대한 결과 미리보기
- helm-monitor plugin 설치: prometheus 쿼리를 기반으로 release/rollback 모니터링

- values.yml에 externalIPS, nodeAffinity 삭제해서 helm install --set 매개변수로 전달할 수 있도록 하기
- securityContext 정의하기
- chart release 시 namespace 정의하기