# 🔍 개미
- 설계 시간 : 55분
- 구현 시간 : 217분

---

# 💡 아이디어
- 시간 제한이 0.15초로 효율성을 무조건 고려해야됨을 파악
- 개미의 이동을 x좌표와 y좌표로 따로 구하는 것이 합리적이라 판단
- 너비 * 2, 높이 * 2 마다 위치가 초기화되는 점을 이용해 빠르게 계산 가능
  - 개미의 초기 위치를 0, 0으로 바꿔주고 그만큼 이동할 시간을 늘려준다
  - 이후 % 연산으로 반복을 제외한 나머지 거리를 구해준다
  - 나머지 거리가 너비와 높이를 초과할 경우와 그렇지 않은 경우로 나눠서 해결한다

---

# 🧠 어려웠던 점
- 처음에 그냥 한칸씩 이동하는 식으로 구현
  - 광탈
- 벽에 부딪힐 때마다 방향이 바뀌는 걸 한번에 이동하도록 구현
  - 광탈 -> 여기서 멘탈 나감
- 기하학적 대칭을 이용해서 구해보려고 함
  - 이건 안될 듯 싶었음
- 좌표를 분리해서 각각 % 연산으로 나머지를 활용해 구함
  - 광탈 -> 진짜 개 에바였음
- Java 11로 채점하던거 설정 바꿔서 Java 8로 바꾸고 통과함
  - 백준에서 패스 안되면 언어 한번 바꿔보는거 추천

---

# 🧐 좋은 풀이
- 그냥 내꺼가 완벽함