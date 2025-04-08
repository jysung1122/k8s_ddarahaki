# k8s_ddarahaki

# 2025.04.08
쿠버네티스 설치

- [유튜브](https://www.youtube.com/watch?v=5Y847xaXe7U])
- [블로그](https://velog.io/@sororiri/k8s-kubeadm-%EC%84%A4%EC%B9%98-big2bz1i)
- [Kubernetes Doc](https://kubernetes.io/docs/setup/production-environment/tools/kubeadm/install-kubeadm/)

![image](https://github.com/user-attachments/assets/8585f5eb-c154-4be3-8c70-2c83520216e3)

Kubernetes 구성 요약
- 1개의 마스터 노드 (control-plane)
  - version: v1.32.3
- 2개의 워커 노드
  - version: v1.32.3
  - 역할(Roles)은 현재 지정되지 않았으며, 일반 워커 노드로 동작

구성요소
- 설치 방식: kubeadm
- 컨테이너 런타임: containerd
- CNI(Network Plugin): Calico (Pod 간 네트워크 및 정책 지원)
- 클러스터 상태: 모든 노드 Ready 상태로 정상 운영 중
- kubectl 사용: 마스터 노드에서만 CLI 제어 (워커 노드는 관리 권한 없음)

이 구조는 실습, 테스트, 소규모 서비스 운영을 위한 경량 클러스터 구성 예시로 최적화되어 있으며, Pod 배포, 네트워크 실습, 오토스케일링 등 다양한 기능 실험에 활용 가능함
