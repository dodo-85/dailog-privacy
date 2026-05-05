# DaiLog 계정 및 데이터 삭제 안내

**앱 이름**: DaiLog (데일로그)
**개발자**: 이도현
**문의 이메일**: gandiz23@gmail.com

DaiLog는 사용자가 언제든 계정과 모든 데이터를 삭제할 수 있도록 안내합니다.

---

## 1. 앱 내에서 직접 삭제 (권장)

가장 빠른 방법입니다. 즉시 모든 데이터가 삭제됩니다.

1. DaiLog 앱 실행 후 로그인
2. 하단 탭에서 **설정** 선택
3. **계정** 섹션의 **회원 탈퇴** 항목 탭
4. 안내 문구 확인 후 **탈퇴** 버튼 탭
5. 계정과 모든 데이터가 즉시 삭제됨

## 2. 이메일로 요청

앱에 접근할 수 없는 경우 이메일로 요청 가능합니다.

- **수신자**: gandiz23@gmail.com
- **제목**: DaiLog 계정 삭제 요청
- **본문에 포함할 내용**: 가입 시 사용한 Google 계정의 이메일 주소
- **처리 기한**: 요청 확인 후 10일 이내 처리

---

## 삭제되는 데이터

회원 탈퇴 시 아래 모든 데이터가 **즉시 영구 삭제**됩니다.

| 데이터 | 저장 위치 | 삭제 시점 |
|---|---|---|
| 이메일, 이름, 프로필 사진 URL | Firebase Authentication | 탈퇴 즉시 |
| 활동 기록(블럭), 라벨, 목표, 설정값 | Firestore | 탈퇴 즉시 |
| FCM 푸시 알림 토큰 | Firestore | 탈퇴 즉시 |

## 보관되는 데이터

회원 탈퇴 후 추가로 보관되는 데이터는 **없습니다**. 백업 또는 별도 보관 정책을 운용하지 않습니다.

분석 도구(Firebase Analytics, Crashlytics, Microsoft Clarity)에서 수집된 데이터는 **개인 식별이 불가능한 익명 통계**로 처리되며, 이는 개인 데이터에 해당하지 않습니다.

---

## English

### Account & Data Deletion for DaiLog

**App**: DaiLog
**Developer**: Dohyun Lee
**Contact**: gandiz23@gmail.com

#### Option 1 — Delete in-app (recommended)
1. Open DaiLog and sign in
2. Go to **Settings** tab
3. Tap **Delete Account** under the Account section
4. Confirm the deletion
5. Account and all data are deleted immediately

#### Option 2 — Email request
- **Send to**: gandiz23@gmail.com
- **Subject**: DaiLog Account Deletion Request
- **Include**: Email address used for sign-up
- **Processed within**: 10 days of receipt

#### Data Deleted
All user data is permanently deleted upon account deletion: email, name, profile photo URL, activity records (blocks), labels, goals, settings, and FCM tokens.

#### Data Retained
**None.** No backup or separate retention is maintained after deletion. Analytics data (Firebase Analytics, Crashlytics, Microsoft Clarity) is anonymized aggregate data that does not constitute personal data.
