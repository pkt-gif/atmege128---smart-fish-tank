# Smart Fish Tank

> ATmega128A 기반 스마트 어항 관리 자동화 시스템

조도 센서를 이용한 수질 상태 확인, 예약 먹이 배급, 레일 청소 및 어항 상태 표시 기능을 통합한 임베디드 팀 프로젝트입니다.

## 프로젝트 정보

- 개발 기간: 2026.05.08 ~ 2026.05.13
- 개발 형태: 4인 팀 프로젝트
- 담당 역할:
  - 조도 센서 기반 수질 관리 기능 구현
  - 프로젝트 발표자료 제작 및 발표

## 주요 기능

- 조도 센서를 이용한 탁도 판정 및 수질 상태 표시
- RTC 기준 설정 시간에 서보모터로 먹이 자동 배급
- DC 모터를 이용한 레일 왕복 청소
- RGB LED를 이용한 수질 상태 알림
- I2C LCD를 통한 어항 상태 출력

## 시스템 구성

```text
조도 센서 · RTC 시간 정보
            ↓
        ATmega128A
            ↓
 수질 판정 · 먹이 배급 · 레일 청소
            ↓
RGB LED · 서보모터 · DC 모터 · I2C LCD
```

## 담당 구현

조도 센서의 측정값을 기준으로 어항의 수질 상태를 판정하고, 결과를 RGB LED와 I2C LCD로 확인할 수 있도록 구현했습니다.

## 기술 스택

`ATmega128A` · `C` · `AVR Studio` · `ADC` · `I2C` · `RTC` · `PWM` · `DC Motor` · `Servo Motor`

## 프로젝트 결과

🎬 [유튜브(YouTube) 스마트 어항 영상](https://www.youtube.com/watch?v=u2zzdcHJl2s)

📊 [프로젝트 발표 PPT](https://docs.google.com/presentation/d/148J36PkVOABS_IdUh0nViSP8VyKp4w8m8m-7FM9RXnw/edit?slide=id.g3e0b0b0bd8e_16_2#slide=id.g3e0b0b0bd8e_16_2)
