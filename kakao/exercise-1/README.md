2017년도 카카오 그룹의 블라인드 채용 모의고사 문제풀이입니다.
모의고사 채점을 통과한 코드일 뿐, 정답은 아닐 수 있습니다.
설명은 자세히 하지않고 간단한 힌트만 알려드립니다. 코드를 보고 분석해보는 걸 추천합니다.

## 1번, 2번, 3번
간단한 구현이므로 설명은 생략합니다.

## 4번
N과 M이 1000 제한이기 때문에 N\*M = 100만이므로, 추가 복잡도가 100배 이상 되지
않아야 효율성 테스트를 통과할 가능성이 있습니다. (1억미만)
정사각형의 내부가 모두 가득차야하는 조건을 고려하면 됩니다.
배열의 (i,j)마다 각각 정사각형을 가득채울 수 있는 가로, 세로, 대각선의 최댓값을 저장하면
쉽게 풀 수 있습니다.

## 5번
배열 ARR[N][M][2]를 통해 각 위치 (i,j)별로 문제 설명 그대로 구현하면 됩니다.
ARR[N][M][0]는 내 칸을 밟지 않았을 때이며, ARR[N][M][1]은 내 칸을 밟았을 경우로 생각하면
쉽게 풀 수 있습니다.

## 6번
역시나 간단한 메모이제이션 + Divide and Conquer 문제입니다.
그냥 내 위치를 떼는 경우/안 떼는 경우 2가지를 반복하면 됩니다.

## 7번
처음부터 차례대로 현재 위치까지 만들 수 있는 방법의 최솟값을 저장하면 쉽게 풀 수 있습니다.
