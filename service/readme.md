# 포드

- 포드 : 컨테이너 애플리케이션의 기본 단위

## 1. YAML 파일의 의미

```yaml
apiVersion: v1
kind: Pod
metadata:
  name: my-nginx-pod
spec:
  containers:
    - name: my-nginx-container
      image: nginx:latest
      ports:
        - containerPort: 80
          protocol: TCP
```

- apiVersion : yaml파일에서 정의한 오브젝트의 API버전

* kind : 리소스의 종류

## kubectl 명령어

- kubectl exec : 포드의 컨테이너에 명령어 전달

- kubectl logs : 포드의 로그 확인

* kubectl delete -f : 오브젝트 삭제
