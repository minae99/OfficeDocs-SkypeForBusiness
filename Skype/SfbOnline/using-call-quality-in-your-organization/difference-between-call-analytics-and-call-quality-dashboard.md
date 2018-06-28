---
title: "통화 분석과 통화품질 대시보드"
ms.author: lolaj
author: LolaJacobsen
manager: serdars
ms.reviewer: mikedav, wlooney
ms.topic: article
ms.assetid: 4cd5fe35-8463-4996-a252-086cd3ca2d9a
ms.tgt.pltfrm: cloud
ms.service: skype-for-business-online
ms.collection: Adm_Skype4B_Online
ms.audience: Admin
appliesto:
- Skype for Business 
- Microsoft Teams
localization_priority: Normal
f1keywords: None
ms.custom:
- Reporting
description: "Learn about Call Analytics and Call Quality Dashboard and when to use them to monitor and troubleshoot call-quality problems in Skype for Business."
---

# 통화 분석과 통화품질 대시보드

Skype for Business는 통화 품질 문제를 모니터링하고 문제를 해결하기 위해 두가지 방법을 제공합니다: Call Analytics 와 Call Quality Dashboard 이 문서는 두가지 기술을 설명하고 그것을 사용할 경우를 안내합니다
  
> [!NOTE]
> Call Analytics is currently in preview. Text and images described here may not match your experience. 
> Only last 30 days of data is available in Call Analytics.
  
## 통화 분석은 무엇이고 언제 그것을 사용합니까?

통화 분석은 Skype for Business 계정의 각 사용자에 대한 특정적인 통화와 회의에 관련된 기기, 네트워크 및 연결상태에 대한 자세한 정보를 표시합니다 만약 당신이 Skype for Business 관리자라면 Skype for Business의 통화품질과 연결상태의 문제를 해결하기 위해 통화분석을 사용할 수 있습니다
  
만약 관리자를 대신해 헬프데스크 담당자가 통화 분석을 사용하고자 한다면 권한을 위임할 수 있습니다 위임받은 직원은 Skype for Business 관리자센터에서 해당 기능For more details, see을 제외한 다른 기능은 제한됩니다
  
- 티어1 헬프데스크 담당자 : 해당직원은 통화분석에서 제한된 데이터셋과 개인식별정보 PII를 볼수있습니다 그들은 통화문제를 해결할 수 있지만 미팅에 관련된 문제는 티어2 직원에게 전달하게 됩니다
    
- 티어2 헬프데스크 담당자 : 해당직원은 통화분석에서 가능한 모든 데이터를 보고 통화와 미팅 모든 문제를 해결합니다 그들은 통화로그와 사용자 정보에 모두 접근할 수 있습니다
    
통화 분석 설정에 대한 자세한 내용은 [Set up Skype for Business Call Analytics](set-up-call-analytics.md) 참조하세요

헬프데스크 직원이 통화 분석 기술로 작업하는 방법에 대한 자세한 내용은 [Use Call Analytics to troubleshoot poor call quality](use-call-analytics-to-troubleshoot-poor-call-quality.md) 참조하세요
  
## 통화품질 대시보드는 무엇이고 언제 그것을 사용합니까?

통화 분석은 사용자의 통화 품질에 대한 상세하고 구체적인 정보를 제공합니다 예를 들어 홍길동님의 오늘 오후 통화 상태가 안좋은 이유는 무엇일까요? 통화 분석을 사용하면 Skype for Business 관리자나 헬프데스크 직원은 장치, 네트워크, 연결상태 및 홍길동씨의 통화와 관련된 다른 요소를 조사 할 수 있습니다
  
CA-통화 분석-은 관리자 및 헬프데스크 직원이 특정 통화로 인한 통화 품질 문제를 해결할 수 있도록 설계되어 있으며 CQD-통화 품질 대시보드-는 Skype for Business 관리자 및 네트워크 엔지니어가 네트워크 상태를 최적화 할 수 있도록 설계되어 Skype for Business 전체 조직 정보를 집계합니다 
  
만약 홍길동님의 통화품질 저하가 네트워크 문제에서 발생했다면 다른 사용자들도 영향을 받게 됩니다. 홍길동님의 개별적인 통화이력은 CQD에서 볼 수 없지만 Skype for Business를 사용하여 작성된 전체 통화 품질이 캡처되어 전반적인 통화 품질 패턴을 확인할 수 있으므로 네트워크 엔지니어는 통화 품질에 대한 정보에 근거해 평가할 수 있습니다 CQD는 전체 통화 품질, 서버-클라이언트 및 클라이언트-클라이언트 스트리밍, 음성품질 [SLA](https://go.microsoft.com/fwlink/p/?linkid=846252) 에 대한 통찰력을 제공하는 '통화 품질 메트릭스 보고서'를 제공합니다
  
![Screenshot of Call Quality Dashboard in the Skype for Business Admin Center. Tabs shown are Overall Call Quality, Server - Client, Client - Client, and View Quality SLA.](../images/6eaccf99-8ee8-4f99-bdf2-ba1c72471cb9.png)
  
 [Features of the Call Quality Dashboard for Skype for Business Online](turning-on-and-using-call-quality-dashboard.md#BKMKFeaturesOfTheCQD) 에 대한  추가정보를 확인하세요
  
CA와 CQD는 병렬로 실행해 독립적 또는 동시에 사용할 수 있습니다 예를 들어 티어1 상담원이 통화 문제를 해결하는 데 추가 도움이 필요하다고 판단한 경우 티어1 상담원은 그들보다 CA 통화분석에서 더 많은 정보에 접근할 수있는 티어2 상담원에게 전달합니다 순차적으로 티어2 상담원은 네트워크 엔지니어에게 문제를 알릴수있습니다 네트워크 엔지니어는 전체 사이트 관련 문제가 통화 문제의 원인이 될 수 있는지 확인하기 위해 CQD를 확인할 수 있습니다
  
CQD에 대한 자세한 정보를 얻기위해서는 추가 사이트를 방문하세요  

[Turning on and using Call Quality Dashboard for Microsoft Teams and Skype for Business Online](turning-on-and-using-call-quality-dashboard.md) 
[Dimensions and measures available in Call Quality Dashboard for Microsoft Teams and Skype for Business Online](dimensions-and-measures-available-in-call-quality-dashboard.md).
  
## Related topics
[Set up Skype for Business Call Analytics](set-up-call-analytics.md)

[Use Call Analytics to troubleshoot poor Skype for Business call quality](use-call-analytics-to-troubleshoot-poor-call-quality.md)

  
 
