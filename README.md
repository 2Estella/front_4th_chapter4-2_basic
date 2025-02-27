# 바닐라 JS 프로젝트 성능 개선
- url: https://d2cvvqmbjry9rr.cloudfront.net/
  
---
   
## 성능 개선 사후 보고서

### 1. **개선 이유**

웹사이트의 성능이 사용자 경험과 검색 엔진 최적화(SEO)에 중요한 영향을 미친다는 점을 고려하여 성능 개선 작업을 진행하였습니다. 주된 목표는 **사이트 로딩 시간**을 단축하고, **모바일 사용자 경험**을 개선하며, **SEO** 점수를 향상시키는 것이었습니다. 특히 **Core Web Vitals**의 개선을 통해 페이지 로딩 속도 및 안정성을 높이고, **Lighthouse** 점수를 향상시켜 사용자 경험과 사이트의 검색 엔진 순위를 개선하고자 했습니다.

### 2. **개선 방법**

성능 개선을 위해 여러 가지 최적화 기법을 적용했습니다. 주요 개선 방법은 다음과 같습니다:

- **이미지 최적화**: 이미지 크기를 줄이고, 적절한 포맷(예: WebP)을 사용하여 이미지 로딩 속도를 개선했습니다.
- **JavaScript 최적화**: 불필요한 JavaScript 파일을 제거하거나 비동기/지연 로딩을 사용하여 초기 로딩 시간을 단축시켰습니다.
- **CSS 및 HTML 최적화**: CSS 파일을 압축하고, 불필요한 스타일을 제거하여 페이지 렌더링 속도를 개선했습니다.
- **서버 응답 시간 최적화**: 서버 응답 시간을 단축하고, 캐싱 전략을 개선하여 리소스 로딩 속도를 개선했습니다.
- **Lazy Load 적용**: 페이지에서 필요한 리소스만을 우선 로드하고, 나머지 리소스는 사용자가 필요할 때 로드되는 방식으로 최적화했습니다.
- **SEO 최적화**: 메타 태그, 이미지 alt 태그, 구조화된 데이터(Structured Data) 등을 개선하여 검색 엔진 최적화를 강화했습니다.
- **PWA 기능 고려**: 아직 PWA 점수는 0%로 남아 있지만, 향후 **오프라인 지원** 및 **푸시 알림** 등의 기능을 추가로 해결할 수 있을 것입니다.

### 3. **개선 후 향상된 지표**
성능 개선 전후의 Lighthouse 점수 및 Core Web Vitals 지표를 아래 표로 비교해보았습니다.

| **항목** | **개선 전 점수** | **개선 후 점수** | **변경 사항** |
| --- | --- | --- | --- |
| **Performance** | 72% (🟠) | 94% (🟢) | 크게 향상됨 |
| **Accessibility** | 82% (🟠) | 96% (🟢) | 향상됨 |
| **Best Practices** | 75% (🟠) | 71% (🟠) | 소폭 하락 |
| **SEO** | 82% (🟠) | 100% (🟢) | 완벽한 개선 |
| **PWA** | 0% (🔴) | 0% (🔴) | 변동 없음 |

### **Core Web Vitals 비교**

| **메트릭** | **개선 전 측정값** | **개선 후 측정값** | **변경 사항** |
| --- | --- | --- | --- |
| **LCP (Largest Contentful Paint)** | 14.48s (🔴) | 3.01s (🟠) | 크게 개선됨 |
| **INP (Interaction to Next Paint)** | N/A (🟢) | N/A (🟢) | 변화 없음 |
| **CLS (Cumulative Layout Shift)** | 0.011 (🟢) | 0.001 (🟢) | 개선됨 |

이러한 개선은 사이트의 **로딩 속도**와 **반응성**, **사용자 경험**을 크게 향상시켰습니다. 
특히 **LCP**의 개선은 사용자에게 빠른 콘텐츠 로딩을 제공하며, **CLS**의 개선은 페이지 로딩 중 레이아웃이 안정적으로 유지되도록 하여 불편함을 최소화합니다.

### 4. **기타**

- **성능 모니터링 및 지속적인 개선**: 성능 개선 작업은 일회성으로 끝나는 것이 아니라 지속적으로 모니터링하고 개선해야 합니다. 웹사이트의 성능은 새로운 콘텐츠 추가나 외부 서비스 통합 등 다양한 이유로 언제든지 영향을 받을 수 있기 때문에, **주기적인 성능 점검**을 통해 문제를 사전에 예방할 수 있습니다.
  
- **PWA 구현 계획**: 현재 PWA 점수는 여전히 0%로 개선되지 않았습니다. 사용자에게 좋은 경험을 주기 위해 개선 방안을 모색해 볼 예정입니다.

- **배포 후 Lighthouse 점수**: 아래 이미지는 S3 + cloudFront로 배포 및 최적화 후 페이지 성능 측정 결과 입니다.
  ![image](https://github.com/user-attachments/assets/8b8017ba-1823-4a92-adb0-68e5c7e89282)


### 5. **결론**

성능 개선 작업을 통해 웹사이트는 **로딩 속도**, **반응성**, **SEO** 점수에서 상당한 향상을 이루었습니다. **Core Web Vitals**와 **Lighthouse** 점수가 개선되어 사용자 경험과 검색 엔진 최적화가 강화되었습니다. 
앞으로도 지속적인 성능 모니터링과 PWA 기능 도입을 통해 웹사이트의 성능을 더욱 향상시킬 수 있도록 노력할 것입니다.
