# 6주차 실습 기록

## 사용한 에셋
 - 이미지: (player.png, https://ansimuz.itch.io/spaceship-shooter-environment)
 - 사운드: (spaceshipshooter.wav, https://ansimuz.itch.io/spaceship-shooter-environment)

## 사용한 AI 프롬프트
 1. (sprite_basics.py)이 코드에 convert_alpha()가 없으면 어떻게 되는지 설명해줘
   - convert_alpha() 없으면 PNG 투명 영역이 깨지고 성능도 느려진다.
 2.효과음이 재생 중일 때 다시 누르면 처음부터 재생되게 해줘
   - shoot_sound.stop() 후 play()를 호출하면 재생 중인 효과음을 중단하고 처음부터 다시 재생한다.

## AI 답변에서 도움이 된 것
 - convert_alpha()이 하는 역할을 알았다.
 - 효과음을 다시 재생하는 방법을 알았다.

## AI 답변을 수정하거나 버린 것
 - 코드를 이상하게 넣어서 올바르게 바꿔서 넣음

## 적용 결과
 - 정상적으로 이미지가 나오고 소리도 잘 나옴
