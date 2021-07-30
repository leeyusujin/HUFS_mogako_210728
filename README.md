### HUFS_mogako_210728


----


#### 활동 내용


신찬수 교수님의 분할정복방법 파트를 배웠다. 분할정복방법의 강의로는 분할정복방법의 소개, 이를 활용한 이진탐색/피보나치 수/하노이 탑 문제와 큰 정수 곱셈하기, 분할정복법과 점화식이 있다. 활동 시간을 고려하여 오늘은 분할정복방법의 소개부터 큰 정수 곱셈하기까지 수강하고 점화식파트는 각자 필요한 사람만 따로 수강하기로 정하였다. 분할정복밥업의 내용으로는 아래의 사진과 같다.


이 방법을 활용하여 이진탐색, 피보나치 수, 하노이 탑 문제를 풀 수 있다. 먼저 이진탐색의 경우 오름차순으로 정렬된 수가 n개 있을 때, 그 숫자들이 저장된 리스트 A에서 x라는 값이 A에 존재하는지 알아내는 탐색법이다. 이때 이진탐색은 시간복잡도가 O(log n)이다. 먼저 A가 i부터 j번째 수가 있다고 가정한다. 이 가운데 값은 (i+j)/2번째 값인데 이 가운데 값과 x라는 값을 비교하여 다음 비교할 범위를 줄이는 것이다. 가운데 값보다 x가 더 크다면 A에서 가운데 값보다 큰 값들만 다음 비교에 사용하면 되고 만약 가운데 값보다 x가 더 작다면 그 반대 범위의 값들만 다음 비교에 사용하면 되므로 비교할 때마다 범위가 절반으로 줄어들게 된다. 따라서 범위가 반으로 줄어들기에 log(n+1) 번 이하의 비교로 x가 존재하는지를 판단할 수 있다.


피보나치 수는 n번째 수를 계산하는 문제이다. n번째 피보나치 수를 구하는 방법은 여러 가지가 있다. 첫 번째 방법은 피보나치 수의 정의인 F(n) = F(n-1) + F(n-2) (단, F(0) = 0, F(1) = 1)을 재귀함수로 구현하는 것이다. 간단하지만 수행시간은 O(G^n) 지수시간이 걸리는것이 문제이다. 두 번째 방법으로는 세 가지 변수를 이용해서 구하고자하는 n번째 값을 계산하는 방법인데 O(n)의 시간이 걸려 비교적 적은 시간에 가능하다. 다른 방법으로는 for루프를 사용하여 0번째 수부터 n번째 수까지 차례로 배열에 채우는 방법인데 방법도 쉽고 시간도 O(n)시간이라 적게 걸린다.

----


#### 느낀점


강의를 듣다가 하노이 탑 부분에 제대로 집중하지 못한 것 같아 한 번 더 들어야겠다는 생각을 했다. 오늘 풀 문제는 구름의 '큰 수 곱셈 알고리즘 구현' 실습문제였다. 처음에는 강의를 듣다가 그냥 실습문제를 풀어보려고 보았는데 문제가 영어로 되어있어 바로 강의로 돌아왔다. 다행히 강의에서 교수님께서 문제에 관해 설명해주셔서 접근할 수 있게 되었다. 다 풀고나서는 그냥 같은 문제인데 영어라는 이유로 왜 못풀었을까라는 생각이 들었다. 앞으로 많은 영어 문제들을 접하게 될 것인데 영어라는 이유만으로 어렵게 생각하는 습관을 버려야겠다.
