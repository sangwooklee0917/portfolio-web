<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>클라우드 인프라 엔지니어 포트폴리오</title>
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      margin: 0;
      padding: 0;
      background: #f4f4f4;
      color: #333;
    }
    header {
      background-color: #222;
      color: white;
      padding: 20px;
      text-align: center;
    }
    section {
      max-width: 1000px;
      margin: 40px auto;
      background: white;
      padding: 30px;
      border-radius: 8px;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
    }
    h2 {
      color: #444;
      border-bottom: 2px solid #ccc;
      padding-bottom: 6px;
    }
    img.diagram {
      width: 100%;
      max-width: 960px;
      margin: 20px 0;
      border: 1px solid #ddd;
      border-radius: 4px;
    }
    ul {
      padding-left: 20px;
    }
    .highlight {
      background: #eef;
      padding: 4px 8px;
      border-radius: 4px;
    }
  </style>
</head>
<body>
  <header>
    <h1>클라우드 인프라 엔지니어 포트폴리오</h1>
    <p>쿠버네티스 기반 OpenStack 운영 및 자동화 경험 중심</p>
  </header>

  <section>
    <h2>👨‍💻 프로필 요약</h2>
    <ul>
      <li>클라우드 인프라 엔지니어 (SK 기반 CloudPC 운영)</li>
      <li>Kubernetes v1.30.3, Helm v3.14.2, containerd v1.7.16</li>
      <li>주요 경험: OpenStack-Helm 기반 배포, Ceph/NetApp 스토리지, RabbitMQ, 인증서 자동화</li>
    </ul>
  </section>

  <section>
    <h2>📌 주요 프로젝트: CloudPC 사용자 로그인 흐름</h2>
    <p>아래 다이어그램은 사용자가 VM에 접속할 때의 전체 인증 및 제어 흐름입니다.</p>
    <img src="./625b7402-592c-42cb-9bed-21c30b503fac.png" alt="CloudPC Login Flow" class="diagram" />

    <p class="highlight">핵심 처리 흐름 설명:</p>
    <ul>
      <li><strong>1~2단계:</strong> Client에서 API Gateway를 통해 접속 시도</li>
      <li><strong>3~4단계:</strong> plat-ms-sm이 정책 정보 및 VM 상태 조회</li>
      <li><strong>5~6단계:</strong> plat-ci-handler가 정책 기반 VM 제어</li>
      <li><strong>7~8단계:</strong> 접속 정보를 API Gateway 통해 Client로 전달</li>
      <li><strong>9단계:</strong> 최종 VM 접속 (TLS 인증 포함)</li>
    </ul>
  </section>

  <section>
    <h2>🔧 인프라 운영 및 자동화 경험</h2>
    <ul>
      <li>OpenStack-Helm 기반 구성 자동화 (Ansible + Shell)</li>
      <li>Kubernetes 기반 pod 로그 수집 정책 수립 (네임스페이스/노드 단위)</li>
      <li>컨트롤 노드 부하 분석 및 자원 분산 전략 적용</li>
      <li>RabbitMQ Queue consumer 수집률 이상 감지 및 자동 복구</li>
      <li>SPICE 인증서 자동 갱신 실패 대응 (libvirt 연동)</li>
    </ul>
  </section>

  <section>
    <h2>📈 자동화 성과</h2>
    <ul>
      <li>배포 자동화 스크립트 도입으로 <strong>운영 시간 60% 단축</strong></li>
      <li>Health Check 자동화로 <strong>일일 점검 누락률 0%</strong> 유지</li>
      <li>로그 기반 알림 개선으로 <strong>장애 대응 평균 시간 35% 감소</strong></li>
    </ul>
  </section>

  <section>
    <h2>📞 연락처</h2>
    <p>이메일: <strong>skyasu@domain.com</strong></p>
    <p>GitHub: <strong>github.com/skyasu2</strong></p>
  </section>
</body>
</html>
