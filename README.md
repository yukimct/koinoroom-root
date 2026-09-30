# koinoroom.com (최상위 도메인)

**이 저장소가 있는 이유는 `app-ads.txt` 하나 때문입니다.**

AdMob은 스토어에 적힌 개발자 URL의 **최상위 도메인**에서 `app-ads.txt`를 찾습니다.
App Store에는 `privacy.koinoroom.com`이 적혀 있지만, 크롤러가 보는 곳은 뿌리인
`koinoroom.com`입니다. 하위 도메인에만 올려 두면 「앱을 확인할 수 없습니다」가
계속 뜨고 **광고 게재가 제한된 채로 남습니다.**

## 도메인 배치

| 도메인 | 저장소 | 무엇 |
|---|---|---|
| `koinoroom.com` | 여기 | app-ads.txt, 안내 한 장 |
| `privacy.koinoroom.com` | `yukimct/koinoroom` | 개인정보처리방침·데이터 삭제 |
| `go.koinoroom.com` | `yukimct/go` | 딥링크(`/vs/*`)·설치 안내(`/get`) |
| `dogadm.koinoroom.com` | `yukimct/docAdmin` | 관리자 페이지 |

⚠️ **공개 저장소입니다.** GitHub Pages 무료 플랜은 공개여야 서비스됩니다.
**비공개로 바꾸면 사이트가 죽고 광고 인증도 같이 풀립니다.**

## DNS

Cloudflare에서 최상위 도메인에 `yukimct.github.io`를 가리키는 CNAME을 둡니다.
Cloudflare가 평탄화(flattening)해서 A 레코드처럼 응답합니다.
